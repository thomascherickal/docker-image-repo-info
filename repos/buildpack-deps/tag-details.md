<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `buildpack-deps`

-	[`buildpack-deps:18.04`](#buildpack-deps1804)
-	[`buildpack-deps:18.04-curl`](#buildpack-deps1804-curl)
-	[`buildpack-deps:18.04-scm`](#buildpack-deps1804-scm)
-	[`buildpack-deps:20.04`](#buildpack-deps2004)
-	[`buildpack-deps:20.04-curl`](#buildpack-deps2004-curl)
-	[`buildpack-deps:20.04-scm`](#buildpack-deps2004-scm)
-	[`buildpack-deps:22.04`](#buildpack-deps2204)
-	[`buildpack-deps:22.04-curl`](#buildpack-deps2204-curl)
-	[`buildpack-deps:22.04-scm`](#buildpack-deps2204-scm)
-	[`buildpack-deps:22.10`](#buildpack-deps2210)
-	[`buildpack-deps:22.10-curl`](#buildpack-deps2210-curl)
-	[`buildpack-deps:22.10-scm`](#buildpack-deps2210-scm)
-	[`buildpack-deps:23.04`](#buildpack-deps2304)
-	[`buildpack-deps:23.04-curl`](#buildpack-deps2304-curl)
-	[`buildpack-deps:23.04-scm`](#buildpack-deps2304-scm)
-	[`buildpack-deps:bionic`](#buildpack-depsbionic)
-	[`buildpack-deps:bionic-curl`](#buildpack-depsbionic-curl)
-	[`buildpack-deps:bionic-scm`](#buildpack-depsbionic-scm)
-	[`buildpack-deps:bookworm`](#buildpack-depsbookworm)
-	[`buildpack-deps:bookworm-curl`](#buildpack-depsbookworm-curl)
-	[`buildpack-deps:bookworm-scm`](#buildpack-depsbookworm-scm)
-	[`buildpack-deps:bullseye`](#buildpack-depsbullseye)
-	[`buildpack-deps:bullseye-curl`](#buildpack-depsbullseye-curl)
-	[`buildpack-deps:bullseye-scm`](#buildpack-depsbullseye-scm)
-	[`buildpack-deps:buster`](#buildpack-depsbuster)
-	[`buildpack-deps:buster-curl`](#buildpack-depsbuster-curl)
-	[`buildpack-deps:buster-scm`](#buildpack-depsbuster-scm)
-	[`buildpack-deps:curl`](#buildpack-depscurl)
-	[`buildpack-deps:focal`](#buildpack-depsfocal)
-	[`buildpack-deps:focal-curl`](#buildpack-depsfocal-curl)
-	[`buildpack-deps:focal-scm`](#buildpack-depsfocal-scm)
-	[`buildpack-deps:jammy`](#buildpack-depsjammy)
-	[`buildpack-deps:jammy-curl`](#buildpack-depsjammy-curl)
-	[`buildpack-deps:jammy-scm`](#buildpack-depsjammy-scm)
-	[`buildpack-deps:kinetic`](#buildpack-depskinetic)
-	[`buildpack-deps:kinetic-curl`](#buildpack-depskinetic-curl)
-	[`buildpack-deps:kinetic-scm`](#buildpack-depskinetic-scm)
-	[`buildpack-deps:latest`](#buildpack-depslatest)
-	[`buildpack-deps:lunar`](#buildpack-depslunar)
-	[`buildpack-deps:lunar-curl`](#buildpack-depslunar-curl)
-	[`buildpack-deps:lunar-scm`](#buildpack-depslunar-scm)
-	[`buildpack-deps:oldstable`](#buildpack-depsoldstable)
-	[`buildpack-deps:oldstable-curl`](#buildpack-depsoldstable-curl)
-	[`buildpack-deps:oldstable-scm`](#buildpack-depsoldstable-scm)
-	[`buildpack-deps:scm`](#buildpack-depsscm)
-	[`buildpack-deps:sid`](#buildpack-depssid)
-	[`buildpack-deps:sid-curl`](#buildpack-depssid-curl)
-	[`buildpack-deps:sid-scm`](#buildpack-depssid-scm)
-	[`buildpack-deps:stable`](#buildpack-depsstable)
-	[`buildpack-deps:stable-curl`](#buildpack-depsstable-curl)
-	[`buildpack-deps:stable-scm`](#buildpack-depsstable-scm)
-	[`buildpack-deps:testing`](#buildpack-depstesting)
-	[`buildpack-deps:testing-curl`](#buildpack-depstesting-curl)
-	[`buildpack-deps:testing-scm`](#buildpack-depstesting-scm)
-	[`buildpack-deps:unstable`](#buildpack-depsunstable)
-	[`buildpack-deps:unstable-curl`](#buildpack-depsunstable-curl)
-	[`buildpack-deps:unstable-scm`](#buildpack-depsunstable-scm)

## `buildpack-deps:18.04`

```console
$ docker pull buildpack-deps@sha256:a838d98f78f15e4a283ba7ee24e0e7d5944ea6ef8ef6ad8746f48f9529578c52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:18.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:112ea54e20cdb539d74c1aea7d6ea6a943707a9ac2040c39de69943b7a436ee1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221416802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec5bb581fc632486d061a5fad946b21eecd24ac60745e89393352da7e836934`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:39:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:40:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:43:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b21d603a94f829dcf240f93489b3359deed997929b46f2bf66146926bd3ef9f`  
		Last Modified: Tue, 31 Jan 2023 18:00:44 GMT  
		Size: 6.6 MB (6617506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b155ce8564683071c961a173c72705932177495f976f405ab77696ac5cd17b75`  
		Last Modified: Tue, 31 Jan 2023 18:00:43 GMT  
		Size: 3.0 MB (3026069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb0ace4785a8addeddef7444ff5ff46d73774811c1192c979da490211bc50fe`  
		Last Modified: Tue, 31 Jan 2023 18:01:01 GMT  
		Size: 45.5 MB (45511626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ef02d81da19db2c47cb556e459a01501941d27afa51e04bac07cd66b41f902`  
		Last Modified: Tue, 31 Jan 2023 18:01:28 GMT  
		Size: 139.6 MB (139550007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bec2c066b06674351fa26f2f2c118cd93d869499d5c199ea9cc9322a81ac1e72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.7 MB (188669200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b22bc5658b828766b7f163910d113d4cbebff818e724f292cf4a3e55cebf274`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:39:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:40:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:43:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c138257d410403a2127c08e269ac8467b8f2001b22a102934861b65b2f49bc1a`  
		Last Modified: Thu, 26 Jan 2023 10:12:17 GMT  
		Size: 21.4 MB (21395113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47096fe89b773c1646429c4d0b72c616d52ad8e417f6b22a7fffacbf9e543330`  
		Last Modified: Wed, 01 Mar 2023 03:12:33 GMT  
		Size: 5.7 MB (5680777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1cbacc1eb0f2444d8fe8e626335b90e377dba26148c5b1ba67d69a9966df71`  
		Last Modified: Wed, 01 Mar 2023 03:12:32 GMT  
		Size: 2.6 MB (2586738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a752d641cb559708d7e030aae9c70190dbf469ce25759b21c2c34db03cca6ac`  
		Last Modified: Wed, 01 Mar 2023 03:12:52 GMT  
		Size: 40.7 MB (40714103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c6952ec819332449a056dd110221540c0eaa7c31291b042cf53e83555dbe40`  
		Last Modified: Wed, 01 Mar 2023 03:13:20 GMT  
		Size: 118.3 MB (118292469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:298975d24d02a6a27d8263539396799ce83b4a046332e9fe63ec881252ce8b85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (206001361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e8924e0b5645090142a50844e7727c9105cfe493c3b778a52c744e07c792aea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:12:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:12:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:12:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:15:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c3db86e75ada5398a2d9a556625e3e0a4b73c36ab79cf21ccd1ffd35dd43fc`  
		Last Modified: Tue, 31 Jan 2023 18:33:13 GMT  
		Size: 6.1 MB (6055914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cd619a1ebf49880ce75b505030f48c0ab5b4904c5418bbc0145052802eaa63`  
		Last Modified: Tue, 31 Jan 2023 18:33:12 GMT  
		Size: 2.8 MB (2790620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6ed5bf2278606c14e4380d7510535f5bdad7a4e6b5bd6dddff29b256521546`  
		Last Modified: Tue, 31 Jan 2023 18:33:26 GMT  
		Size: 43.3 MB (43313944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ea3f5323e959f3e723895c9550a68aa58401d733f4c29eca854ca8251fb00e`  
		Last Modified: Tue, 31 Jan 2023 18:33:48 GMT  
		Size: 130.1 MB (130105353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a113ee21f105490a147fb85ab0e68054570c5079969b6ddd3731a9db03fab1e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.6 MB (217639452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d20118b6fa4a93abb79434f72311d8fc10725e107f4bb7b89b55504f388af0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:01 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:03 GMT
ADD file:b9b814a7d1e7611a2c531fac3419a48c733c622470d3f275ce29f9ba8764eaeb in / 
# Thu, 26 Jan 2023 10:03:04 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:16:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:16:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:17:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:20:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57a4d5aed2cd4a1f596f693a8fe5e135bd66dbf401ec169b1848d2316bdcfb2c`  
		Last Modified: Thu, 26 Jan 2023 10:12:23 GMT  
		Size: 26.1 MB (26096513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7a01875a8f61110b8a3987b128629884aa645fef18557175a3c73a79ecda62`  
		Last Modified: Wed, 01 Mar 2023 02:27:41 GMT  
		Size: 6.9 MB (6907847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9185b0869254fbcd22a9fab4d7b047d37171dc5b322e61abf872fcc068ecf472`  
		Last Modified: Wed, 01 Mar 2023 02:27:40 GMT  
		Size: 3.3 MB (3255765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79adfdfb2c964ed95f76337267ac66d2871db2f52647fd6f502bca4a71e16a92`  
		Last Modified: Wed, 01 Mar 2023 02:28:00 GMT  
		Size: 47.1 MB (47097285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab3618597de62189ed2023f7cbac7de859932f1d67c09ddb53229e02c8e04b8`  
		Last Modified: Wed, 01 Mar 2023 02:28:37 GMT  
		Size: 134.3 MB (134282042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:31341a141691d55d1f2cca4b84192f7e18716d953c51ddda04a8ee7bf1a65b08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246429217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0f820148ce5933d66e53b71b484a8a2897804ccd2f60c2e2fda8f33a574d90a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:47 GMT
ADD file:108aadd723beb46031bfaca610c036aea506955578347dda4a01cfb0c6bdc135 in / 
# Thu, 26 Jan 2023 09:55:48 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:41:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:42:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:46:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15579125cdf95166fecb7637769c3c9eb2551401759fb21f44848947ead59cbd`  
		Last Modified: Tue, 31 Jan 2023 18:13:22 GMT  
		Size: 30.4 MB (30442586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fea2fabde99e916cabf483638fbf3a31420ac919854738215aa0a52bf39fa`  
		Last Modified: Tue, 31 Jan 2023 18:13:16 GMT  
		Size: 7.0 MB (7035605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428b8a67c5ee9117982087fd7c1be5b763a8286ea404e24144bc6b0042fff348`  
		Last Modified: Tue, 31 Jan 2023 18:13:15 GMT  
		Size: 3.7 MB (3740488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491ab9254ea85bdf063c540c3096b71d4039f2039cf028e624dca83dec8a051f`  
		Last Modified: Tue, 31 Jan 2023 18:13:47 GMT  
		Size: 53.7 MB (53737946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758dd9eee269cf33fbdde212adb77691074569f92a1d01ba62bac008278f4857`  
		Last Modified: Tue, 31 Jan 2023 18:14:35 GMT  
		Size: 151.5 MB (151472592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4f6241dbfc40151e66aea2c355461bbef78034983413e2b41b6832aeb22c35e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205756217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff50765f6a19cc4d538eb4fac2111f73e78e74d036b73805fb2ee671ce87354`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:41 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:43 GMT
ADD file:04d4137c9183cee18560fc26a092e288ff403f3dde266237eab245bd38eb9b3a in / 
# Thu, 26 Jan 2023 09:55:43 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:35:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:38:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4727db5881c26ec0d79df6d172cfc50624c09ca7869b8146052e0692734d2cac`  
		Last Modified: Tue, 31 Jan 2023 17:53:57 GMT  
		Size: 25.4 MB (25371457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e060d5ddd88a52d0a10b103bf4210855c9cc2daac45756f960fd90365af6542`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 6.3 MB (6308650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4883942b852e1bd875f58749e4c99070639db9ac02867dfd13770796b06c8687`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 3.0 MB (2976626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a824cce0d3d1e891d7b4b44e056c1b33ba9f719ad78192a3664800de0d266cd`  
		Last Modified: Tue, 31 Jan 2023 17:54:09 GMT  
		Size: 45.0 MB (45038632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d798a29e5e355ed223ecaefa81f44f8f602cd06432fcdb23e38a81ab93a7137a`  
		Last Modified: Tue, 31 Jan 2023 17:54:36 GMT  
		Size: 126.1 MB (126060852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-curl`

```console
$ docker pull buildpack-deps@sha256:686d709db13d50f30787c0276226d7cdedcf95628c7c106691f693e66b7f5fa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:18.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:eefb4a7c8e274ca65671f877f62a858f8fd0844f35fd6d8cab3be4ab9381518a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36355169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09e8e203a6674cdf500bddc5275d68fb9a2bcc4fb09aef4179d4cb0031dd23f2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:39:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b21d603a94f829dcf240f93489b3359deed997929b46f2bf66146926bd3ef9f`  
		Last Modified: Tue, 31 Jan 2023 18:00:44 GMT  
		Size: 6.6 MB (6617506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b155ce8564683071c961a173c72705932177495f976f405ab77696ac5cd17b75`  
		Last Modified: Tue, 31 Jan 2023 18:00:43 GMT  
		Size: 3.0 MB (3026069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:87c3947ab27b7395c340fdb40be0b232cf4881d24ed4e45a3d4bf5f6e3daa1cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29662628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86602b4d6ae57581dc9d6a308905bf10c1ef8a8b8030b5432cfcae3553ac031b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:39:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c138257d410403a2127c08e269ac8467b8f2001b22a102934861b65b2f49bc1a`  
		Last Modified: Thu, 26 Jan 2023 10:12:17 GMT  
		Size: 21.4 MB (21395113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47096fe89b773c1646429c4d0b72c616d52ad8e417f6b22a7fffacbf9e543330`  
		Last Modified: Wed, 01 Mar 2023 03:12:33 GMT  
		Size: 5.7 MB (5680777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1cbacc1eb0f2444d8fe8e626335b90e377dba26148c5b1ba67d69a9966df71`  
		Last Modified: Wed, 01 Mar 2023 03:12:32 GMT  
		Size: 2.6 MB (2586738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3ca6d0747171417678ed64f5386ecb852fcde4e72a1461446a931f6a09ed6846
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32582064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e54f779279d1503cb962c0a72b798187b208e7b91f6bfa1507768b86cbefd709`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:12:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:12:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c3db86e75ada5398a2d9a556625e3e0a4b73c36ab79cf21ccd1ffd35dd43fc`  
		Last Modified: Tue, 31 Jan 2023 18:33:13 GMT  
		Size: 6.1 MB (6055914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cd619a1ebf49880ce75b505030f48c0ab5b4904c5418bbc0145052802eaa63`  
		Last Modified: Tue, 31 Jan 2023 18:33:12 GMT  
		Size: 2.8 MB (2790620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9c66348aba08cf56330bef73e31d204b066c48c9233586ead80480b01725c030
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbd5750801a877aad4b07a19fbca8b18b3267b49caf30dd0b5bfd0fcba07bdf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:01 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:03 GMT
ADD file:b9b814a7d1e7611a2c531fac3419a48c733c622470d3f275ce29f9ba8764eaeb in / 
# Thu, 26 Jan 2023 10:03:04 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:16:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:16:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:57a4d5aed2cd4a1f596f693a8fe5e135bd66dbf401ec169b1848d2316bdcfb2c`  
		Last Modified: Thu, 26 Jan 2023 10:12:23 GMT  
		Size: 26.1 MB (26096513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7a01875a8f61110b8a3987b128629884aa645fef18557175a3c73a79ecda62`  
		Last Modified: Wed, 01 Mar 2023 02:27:41 GMT  
		Size: 6.9 MB (6907847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9185b0869254fbcd22a9fab4d7b047d37171dc5b322e61abf872fcc068ecf472`  
		Last Modified: Wed, 01 Mar 2023 02:27:40 GMT  
		Size: 3.3 MB (3255765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9f86ff85ce09457dbf0f1f65da193c6aeff8cfc85fbb30dc0a6162051eeeacf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41218679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1c204ad4d256ee762cc2bb63546a154b975ead673362bb7cc0c6779857e4d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:47 GMT
ADD file:108aadd723beb46031bfaca610c036aea506955578347dda4a01cfb0c6bdc135 in / 
# Thu, 26 Jan 2023 09:55:48 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:41:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:15579125cdf95166fecb7637769c3c9eb2551401759fb21f44848947ead59cbd`  
		Last Modified: Tue, 31 Jan 2023 18:13:22 GMT  
		Size: 30.4 MB (30442586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fea2fabde99e916cabf483638fbf3a31420ac919854738215aa0a52bf39fa`  
		Last Modified: Tue, 31 Jan 2023 18:13:16 GMT  
		Size: 7.0 MB (7035605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428b8a67c5ee9117982087fd7c1be5b763a8286ea404e24144bc6b0042fff348`  
		Last Modified: Tue, 31 Jan 2023 18:13:15 GMT  
		Size: 3.7 MB (3740488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c86ef5326c34545c4f4f53fea242951a4457f014933db0817669765075d68c87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34656733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8846013a5b74eb1fd3072a9091d0e1ad91f04a48853e4d84d2c77d240414725`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:41 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:43 GMT
ADD file:04d4137c9183cee18560fc26a092e288ff403f3dde266237eab245bd38eb9b3a in / 
# Thu, 26 Jan 2023 09:55:43 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:35:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4727db5881c26ec0d79df6d172cfc50624c09ca7869b8146052e0692734d2cac`  
		Last Modified: Tue, 31 Jan 2023 17:53:57 GMT  
		Size: 25.4 MB (25371457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e060d5ddd88a52d0a10b103bf4210855c9cc2daac45756f960fd90365af6542`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 6.3 MB (6308650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4883942b852e1bd875f58749e4c99070639db9ac02867dfd13770796b06c8687`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 3.0 MB (2976626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-scm`

```console
$ docker pull buildpack-deps@sha256:ba36fe023887a6023026eae58d6bba3447a045a77a4261c1a1f6db373cedac91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:18.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e7df5351980a3dfe768ac04e0c53fa513d73027ea35485119db202f58ebc8a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81866795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc13147b59defbe2f266c1e16966187b3351b15e4260038e87564d6134d946c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:39:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:40:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b21d603a94f829dcf240f93489b3359deed997929b46f2bf66146926bd3ef9f`  
		Last Modified: Tue, 31 Jan 2023 18:00:44 GMT  
		Size: 6.6 MB (6617506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b155ce8564683071c961a173c72705932177495f976f405ab77696ac5cd17b75`  
		Last Modified: Tue, 31 Jan 2023 18:00:43 GMT  
		Size: 3.0 MB (3026069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb0ace4785a8addeddef7444ff5ff46d73774811c1192c979da490211bc50fe`  
		Last Modified: Tue, 31 Jan 2023 18:01:01 GMT  
		Size: 45.5 MB (45511626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2acd0deb7308e5597b2b9d3b593ae7ea6e8f7fc346ce2d08ebddb9fbe54baad9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70376731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9373357a8aec9ae1e9d9f45f397ff6c4a97a3beec687935474c737e6d687df`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:39:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:40:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c138257d410403a2127c08e269ac8467b8f2001b22a102934861b65b2f49bc1a`  
		Last Modified: Thu, 26 Jan 2023 10:12:17 GMT  
		Size: 21.4 MB (21395113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47096fe89b773c1646429c4d0b72c616d52ad8e417f6b22a7fffacbf9e543330`  
		Last Modified: Wed, 01 Mar 2023 03:12:33 GMT  
		Size: 5.7 MB (5680777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1cbacc1eb0f2444d8fe8e626335b90e377dba26148c5b1ba67d69a9966df71`  
		Last Modified: Wed, 01 Mar 2023 03:12:32 GMT  
		Size: 2.6 MB (2586738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a752d641cb559708d7e030aae9c70190dbf469ce25759b21c2c34db03cca6ac`  
		Last Modified: Wed, 01 Mar 2023 03:12:52 GMT  
		Size: 40.7 MB (40714103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0f7454305ad71cc1618ddc501c963f107e9e1ca383a9dc2e1f1d31db83de8952
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75896008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c594dd26e7b2f1c31896b626cffe79c629fcfd41f75e722dd4626f2f4088e64e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:12:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:12:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:12:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c3db86e75ada5398a2d9a556625e3e0a4b73c36ab79cf21ccd1ffd35dd43fc`  
		Last Modified: Tue, 31 Jan 2023 18:33:13 GMT  
		Size: 6.1 MB (6055914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cd619a1ebf49880ce75b505030f48c0ab5b4904c5418bbc0145052802eaa63`  
		Last Modified: Tue, 31 Jan 2023 18:33:12 GMT  
		Size: 2.8 MB (2790620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6ed5bf2278606c14e4380d7510535f5bdad7a4e6b5bd6dddff29b256521546`  
		Last Modified: Tue, 31 Jan 2023 18:33:26 GMT  
		Size: 43.3 MB (43313944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8ca4f8a2693cdd7aff210955c3bbc8be8eef544578cac7e64a5908ab4a5aee1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83357410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4862a954bb62d0211b2e1de96a09b28b9c636bad9ecc51c55eda533a9b12b23`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:01 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:03 GMT
ADD file:b9b814a7d1e7611a2c531fac3419a48c733c622470d3f275ce29f9ba8764eaeb in / 
# Thu, 26 Jan 2023 10:03:04 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:16:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:16:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:17:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57a4d5aed2cd4a1f596f693a8fe5e135bd66dbf401ec169b1848d2316bdcfb2c`  
		Last Modified: Thu, 26 Jan 2023 10:12:23 GMT  
		Size: 26.1 MB (26096513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7a01875a8f61110b8a3987b128629884aa645fef18557175a3c73a79ecda62`  
		Last Modified: Wed, 01 Mar 2023 02:27:41 GMT  
		Size: 6.9 MB (6907847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9185b0869254fbcd22a9fab4d7b047d37171dc5b322e61abf872fcc068ecf472`  
		Last Modified: Wed, 01 Mar 2023 02:27:40 GMT  
		Size: 3.3 MB (3255765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79adfdfb2c964ed95f76337267ac66d2871db2f52647fd6f502bca4a71e16a92`  
		Last Modified: Wed, 01 Mar 2023 02:28:00 GMT  
		Size: 47.1 MB (47097285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:98b56b01409cca65eb0051a74814eca3788d5a98d541104a5653f00cd973c18d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94956625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ea247b997209a79cca6c45dfbc04979886790d6040979527e616c8e89d7185`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:47 GMT
ADD file:108aadd723beb46031bfaca610c036aea506955578347dda4a01cfb0c6bdc135 in / 
# Thu, 26 Jan 2023 09:55:48 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:41:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:42:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15579125cdf95166fecb7637769c3c9eb2551401759fb21f44848947ead59cbd`  
		Last Modified: Tue, 31 Jan 2023 18:13:22 GMT  
		Size: 30.4 MB (30442586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fea2fabde99e916cabf483638fbf3a31420ac919854738215aa0a52bf39fa`  
		Last Modified: Tue, 31 Jan 2023 18:13:16 GMT  
		Size: 7.0 MB (7035605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428b8a67c5ee9117982087fd7c1be5b763a8286ea404e24144bc6b0042fff348`  
		Last Modified: Tue, 31 Jan 2023 18:13:15 GMT  
		Size: 3.7 MB (3740488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491ab9254ea85bdf063c540c3096b71d4039f2039cf028e624dca83dec8a051f`  
		Last Modified: Tue, 31 Jan 2023 18:13:47 GMT  
		Size: 53.7 MB (53737946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ed5d0d1582ec32919d5650c6af855db2fc9de89b856a8e10fc4d226e285d1449
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79695365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737e17d3b58cd146e26376e8cc717a07041a325ff66cc553302b964fe2f1e252`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:41 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:43 GMT
ADD file:04d4137c9183cee18560fc26a092e288ff403f3dde266237eab245bd38eb9b3a in / 
# Thu, 26 Jan 2023 09:55:43 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:35:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4727db5881c26ec0d79df6d172cfc50624c09ca7869b8146052e0692734d2cac`  
		Last Modified: Tue, 31 Jan 2023 17:53:57 GMT  
		Size: 25.4 MB (25371457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e060d5ddd88a52d0a10b103bf4210855c9cc2daac45756f960fd90365af6542`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 6.3 MB (6308650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4883942b852e1bd875f58749e4c99070639db9ac02867dfd13770796b06c8687`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 3.0 MB (2976626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a824cce0d3d1e891d7b4b44e056c1b33ba9f719ad78192a3664800de0d266cd`  
		Last Modified: Tue, 31 Jan 2023 17:54:09 GMT  
		Size: 45.0 MB (45038632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04`

```console
$ docker pull buildpack-deps@sha256:a11f66d3c0fa48068548afb9f0f6267d91c30c0978f7188baecddf4633ce1bc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b6044fe0ea91b2cd36ee16c377c20c075edb706ba5be48540aa2fccf4169ff31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245768017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0a701ccabc26fb680af02d6d5484e65e2f848b7c60b7dcfabd456bb4e567dc4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:04:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:10:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a237f683deeaa2a1c0890df8ef39ae4992942dd5f941568e877d152a4122aeff`  
		Last Modified: Wed, 01 Feb 2023 18:22:50 GMT  
		Size: 7.7 MB (7735535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84750871be6cfbe4bb1ca3e7384e8526de5f7b7b8f49b37bbc0d94287db639f5`  
		Last Modified: Wed, 01 Feb 2023 18:22:49 GMT  
		Size: 3.6 MB (3627183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3056067387e475581218929338f5478a109fa03d224f88cef9f5ba3a22fbc800`  
		Last Modified: Wed, 01 Feb 2023 18:23:08 GMT  
		Size: 60.7 MB (60742597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258c66296219a7b7f41beceb4f3979c1dd30fb4a55f596c75335276bb34d88d3`  
		Last Modified: Wed, 01 Feb 2023 18:23:36 GMT  
		Size: 145.1 MB (145084818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f4ee369710a84cb660402bee1c73209a428f764fda46b673feec3f37e2190801
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211782702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0351a6ec07f5b3af00d6ced3b1f89da1250782ef25e86ba929626bb6b0552836`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:44:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:45:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:46:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfec9140f00308d23390b191044e2a19bc136e489c813d5449af91bce5b0fe91`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 6.7 MB (6726028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322177715419d97a5871a54f1c8b6fe075220a62dbc72bf41c6dc026440d5e77`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 3.1 MB (3104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33af114797df1d06812900ae5107eeafe4a319eb59a0e0388b6727ec52388a`  
		Last Modified: Wed, 01 Mar 2023 03:13:52 GMT  
		Size: 55.4 MB (55434564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d2ed515ae4a65ad774d2b63208aab21556b5bbae0dbca4126eb26d47e5fbcc`  
		Last Modified: Wed, 01 Mar 2023 03:14:20 GMT  
		Size: 121.9 MB (121931243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b4cc7c24edb74db1d3026fde36d7f4446fd8f4c3b25754916267437eb4ae9253
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235991864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f505c560cb68d89c057dd93202d11b7d6c7e1c58b8cc78793c3e2024e0915d6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:06:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:08:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5cdb9cef850190bebb21cad6356c74e592895e595965cc2791e2ef2e3fe489`  
		Last Modified: Wed, 01 Feb 2023 18:15:45 GMT  
		Size: 7.6 MB (7598155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8388998b5fb9689298ae466de71dd61e6152fe5f0af22c8bef8f73143bacbe`  
		Last Modified: Wed, 01 Feb 2023 18:15:44 GMT  
		Size: 3.6 MB (3616397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758f847d5fa3aeb24a4166e14afe827f2c45890b91333846af93d79830b11e52`  
		Last Modified: Wed, 01 Feb 2023 18:16:01 GMT  
		Size: 60.8 MB (60817045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c190fb00c9b4804425a4c226157db47db90c06ebb209ce79bffd3f87905464`  
		Last Modified: Wed, 01 Feb 2023 18:16:24 GMT  
		Size: 136.8 MB (136766530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:debd6713520a08db50ed1f8da42e4bb8e64256ff314855e17f38e90446516066
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269615848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895823ff50fad310667fb8ab0c42d6f19c33db62519e3d9b21d71a03b38ef2db`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:30 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:31 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:34 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Wed, 01 Feb 2023 11:27:34 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:06:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:10:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c2f997991bfe2ed920105bb595c3662038cc90a08c6db9888fffdfa8c673b16`  
		Last Modified: Tue, 31 Jan 2023 18:14:55 GMT  
		Size: 33.3 MB (33300341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade8a91aca205fdfb604595f12435c45449780688c97c002034b3480b4d6e2f`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 8.7 MB (8689144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d265fb7cba3184708a8658bbe28f6d6d9211befbded0f8b5cfeb9ffa0ba5450`  
		Last Modified: Wed, 01 Feb 2023 18:20:40 GMT  
		Size: 4.5 MB (4486791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a9987c53440b65f7504e1d2c125e138e961fb52b5bddc2d0867140186bf880`  
		Last Modified: Wed, 01 Feb 2023 18:21:16 GMT  
		Size: 69.5 MB (69549088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62134bdf1c65d5122d7110f6b1b984c70adc7fd07c674647a66c826e82bb4db`  
		Last Modified: Wed, 01 Feb 2023 18:22:05 GMT  
		Size: 153.6 MB (153590484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c95b6aae122f7f76230ddda12ca65b704361cbe8e9494b2361443a8eb10fcf5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226361958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4911e269a7ec2a84ce69826ff10b45db58595afe5b4e7e8597412cc3d7b80c7b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 12:00:21 GMT
ARG RELEASE
# Wed, 01 Feb 2023 12:00:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 12:00:23 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Wed, 01 Feb 2023 12:00:24 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:12:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:14:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbc0e1117f61ba365a9a02263b82c04f704d5d162aa31b25a9326797dd1c7084`  
		Last Modified: Tue, 31 Jan 2023 17:54:46 GMT  
		Size: 27.0 MB (27016130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc2216ece6dadf4da9b635d2395de116381e0d77d88f239e2440d4b3bd4786c`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 7.4 MB (7375308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d74c38d5b135b15d3f891f4092219a28a69ce6738a9f6f36d1e2a5797d17ae6`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 3.5 MB (3542223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c45bf4caa5f11965d7b2ffce3e1020b2c76ddf1303186de98cb306ca4dedb2`  
		Last Modified: Wed, 01 Feb 2023 18:21:22 GMT  
		Size: 60.0 MB (60013452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1303d755910ead728efff8974e64e475b681de3250682a0aa8d0a19094c85b`  
		Last Modified: Wed, 01 Feb 2023 18:21:45 GMT  
		Size: 128.4 MB (128414845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:49e6eaf11041a83345b2d88f3989f933e331423be807bf41d12ac9ec19510376
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:139902f730347058d9c1a1601cedbd51c4a2656bda19472be86e9ce88d1b09b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39940602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65cdd40989a1f01db8064bf6f6ab912f1a303f06e61425eb6a86136c09a67435`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:04:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a237f683deeaa2a1c0890df8ef39ae4992942dd5f941568e877d152a4122aeff`  
		Last Modified: Wed, 01 Feb 2023 18:22:50 GMT  
		Size: 7.7 MB (7735535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84750871be6cfbe4bb1ca3e7384e8526de5f7b7b8f49b37bbc0d94287db639f5`  
		Last Modified: Wed, 01 Feb 2023 18:22:49 GMT  
		Size: 3.6 MB (3627183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5fdcbea172ca3a8d6a3c1f8e79956915271ef25a450e23c0f8d002d8a40cbf58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34416895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f121c3293b2153a65dc0914441f3c0ce8cdfd71bfe9ffd405a153dc811bce5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:44:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:45:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfec9140f00308d23390b191044e2a19bc136e489c813d5449af91bce5b0fe91`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 6.7 MB (6726028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322177715419d97a5871a54f1c8b6fe075220a62dbc72bf41c6dc026440d5e77`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 3.1 MB (3104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d25ee52ef857785d1cf3704c3ea1d271d3dd3131c3f4d8c46187ce62e02a24e3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38408289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026010a0d29289f441533dfb0918a2ec67e947cf80f38369b4be824ebd761abd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5cdb9cef850190bebb21cad6356c74e592895e595965cc2791e2ef2e3fe489`  
		Last Modified: Wed, 01 Feb 2023 18:15:45 GMT  
		Size: 7.6 MB (7598155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8388998b5fb9689298ae466de71dd61e6152fe5f0af22c8bef8f73143bacbe`  
		Last Modified: Wed, 01 Feb 2023 18:15:44 GMT  
		Size: 3.6 MB (3616397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f12fd21739b9805f915c8a8fcd95f77440c2ade1713eb864f3e9a9cd8f2e1aa0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46476276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e576a3c65f45877574e6fd14bf5613665e5df7b810945d8f29cfb3e32788d488`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:30 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:31 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:34 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Wed, 01 Feb 2023 11:27:34 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0c2f997991bfe2ed920105bb595c3662038cc90a08c6db9888fffdfa8c673b16`  
		Last Modified: Tue, 31 Jan 2023 18:14:55 GMT  
		Size: 33.3 MB (33300341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade8a91aca205fdfb604595f12435c45449780688c97c002034b3480b4d6e2f`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 8.7 MB (8689144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d265fb7cba3184708a8658bbe28f6d6d9211befbded0f8b5cfeb9ffa0ba5450`  
		Last Modified: Wed, 01 Feb 2023 18:20:40 GMT  
		Size: 4.5 MB (4486791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ead28fd5276dd6d06beead5edda1c5465fdaf1102c638d302804abdbf3ab8112
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37933661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf5e6c104c73bfc12b1098e513fdac7cd8818362937b3180a7671a449699f116`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 12:00:21 GMT
ARG RELEASE
# Wed, 01 Feb 2023 12:00:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 12:00:23 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Wed, 01 Feb 2023 12:00:24 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cbc0e1117f61ba365a9a02263b82c04f704d5d162aa31b25a9326797dd1c7084`  
		Last Modified: Tue, 31 Jan 2023 17:54:46 GMT  
		Size: 27.0 MB (27016130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc2216ece6dadf4da9b635d2395de116381e0d77d88f239e2440d4b3bd4786c`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 7.4 MB (7375308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d74c38d5b135b15d3f891f4092219a28a69ce6738a9f6f36d1e2a5797d17ae6`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 3.5 MB (3542223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:97a93de68bfcd86027cb9660aca032ff8201aad2d56677e8db2d49ab799bac95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b001233b50ee9b078a84543d8d08551ff93f4c47c841cd89924c557fda980084
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100683199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508dc825343263364ae968240e3719932e52f5f5de5216a5d2ba307191056546`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:04:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a237f683deeaa2a1c0890df8ef39ae4992942dd5f941568e877d152a4122aeff`  
		Last Modified: Wed, 01 Feb 2023 18:22:50 GMT  
		Size: 7.7 MB (7735535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84750871be6cfbe4bb1ca3e7384e8526de5f7b7b8f49b37bbc0d94287db639f5`  
		Last Modified: Wed, 01 Feb 2023 18:22:49 GMT  
		Size: 3.6 MB (3627183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3056067387e475581218929338f5478a109fa03d224f88cef9f5ba3a22fbc800`  
		Last Modified: Wed, 01 Feb 2023 18:23:08 GMT  
		Size: 60.7 MB (60742597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bc5573a38cb133e8647d1a65a0af37d38f7dea0fa4c9c8f35396e4d80c48cfb5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89851459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a7185ef92eae1a4d52e27855dab33ccee9eabf97d62256082b958d573f92bd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:44:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:45:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:46:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfec9140f00308d23390b191044e2a19bc136e489c813d5449af91bce5b0fe91`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 6.7 MB (6726028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322177715419d97a5871a54f1c8b6fe075220a62dbc72bf41c6dc026440d5e77`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 3.1 MB (3104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33af114797df1d06812900ae5107eeafe4a319eb59a0e0388b6727ec52388a`  
		Last Modified: Wed, 01 Mar 2023 03:13:52 GMT  
		Size: 55.4 MB (55434564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:31b0c3a25fb4a67287257afd0dbc7ca11f85f0635bf2fa3e746e580c7d79e3ba
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99225334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d3534946432eb97d22d0b303eeaf07846380627bceb09c91f522e5b2b7715b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:06:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5cdb9cef850190bebb21cad6356c74e592895e595965cc2791e2ef2e3fe489`  
		Last Modified: Wed, 01 Feb 2023 18:15:45 GMT  
		Size: 7.6 MB (7598155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8388998b5fb9689298ae466de71dd61e6152fe5f0af22c8bef8f73143bacbe`  
		Last Modified: Wed, 01 Feb 2023 18:15:44 GMT  
		Size: 3.6 MB (3616397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758f847d5fa3aeb24a4166e14afe827f2c45890b91333846af93d79830b11e52`  
		Last Modified: Wed, 01 Feb 2023 18:16:01 GMT  
		Size: 60.8 MB (60817045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ddf4f10cc043ec41a872de8194f92e5c44dbcad6de965cb6be6449dc9bf70425
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116025364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438a5c02f5081ad8934e225034c0bcde18e4aadc08fc556957740a6ee39f4313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:30 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:31 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:34 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Wed, 01 Feb 2023 11:27:34 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:06:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c2f997991bfe2ed920105bb595c3662038cc90a08c6db9888fffdfa8c673b16`  
		Last Modified: Tue, 31 Jan 2023 18:14:55 GMT  
		Size: 33.3 MB (33300341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade8a91aca205fdfb604595f12435c45449780688c97c002034b3480b4d6e2f`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 8.7 MB (8689144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d265fb7cba3184708a8658bbe28f6d6d9211befbded0f8b5cfeb9ffa0ba5450`  
		Last Modified: Wed, 01 Feb 2023 18:20:40 GMT  
		Size: 4.5 MB (4486791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a9987c53440b65f7504e1d2c125e138e961fb52b5bddc2d0867140186bf880`  
		Last Modified: Wed, 01 Feb 2023 18:21:16 GMT  
		Size: 69.5 MB (69549088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7206163a36b7760c9efdbd29a434acc8b1990718675a8ca5f045f76507a5cd08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97947113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f3b12ede6075af4413052ec568fae6e5c908e6e17e9df7d596293718a962c7b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 12:00:21 GMT
ARG RELEASE
# Wed, 01 Feb 2023 12:00:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 12:00:23 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Wed, 01 Feb 2023 12:00:24 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:12:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbc0e1117f61ba365a9a02263b82c04f704d5d162aa31b25a9326797dd1c7084`  
		Last Modified: Tue, 31 Jan 2023 17:54:46 GMT  
		Size: 27.0 MB (27016130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc2216ece6dadf4da9b635d2395de116381e0d77d88f239e2440d4b3bd4786c`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 7.4 MB (7375308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d74c38d5b135b15d3f891f4092219a28a69ce6738a9f6f36d1e2a5797d17ae6`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 3.5 MB (3542223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c45bf4caa5f11965d7b2ffce3e1020b2c76ddf1303186de98cb306ca4dedb2`  
		Last Modified: Wed, 01 Feb 2023 18:21:22 GMT  
		Size: 60.0 MB (60013452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04`

```console
$ docker pull buildpack-deps@sha256:7934746af260757ca2bd84afbc1df916b3fadde6cb3a3a2e8dd09782ec81ae27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e902a5ede3335b40edf720db97f0f318f2f014bf34395671c61dd7c554c38967
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (250046286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6288482ed9f9138697941e4e8d8adbccf0abf3881591a8a78034ce0bcb07033a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:48:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:48:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:51:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec15466900398b5d701c68ab4f91684333cee7a531fee222d5fcb8a8a7b20d`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.8 MB (3788240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91ea6918177a2aa7ef5f879923eaccfb2e1ddaca74cc714d50e7132ffe71309`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.6 MB (3561486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a44fd0db0640850be18488f070ec215526d9623b7ae525fac72b3f7e3c8efe2`  
		Last Modified: Tue, 31 Jan 2023 18:02:55 GMT  
		Size: 39.4 MB (39353567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df80616fdd7c890e62484c7b02ed89709cb73ab849066978bdfed12211de1893`  
		Last Modified: Tue, 31 Jan 2023 18:03:27 GMT  
		Size: 172.9 MB (172913989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7f1d248f07fb9e2219f7db6f6f1eb23066ceaed4aaac404d9a2e522827dc4508
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218684697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae1e90e96a16ea3fb4fcef9e7eb2c23dfb79daab0d2a3f6479a3b11527335b5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:50:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:51:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:55:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d0210273e3495988f639f6164118a5bba55666799ba86ac3e60a001cf7be3b31`  
		Last Modified: Thu, 26 Jan 2023 18:27:33 GMT  
		Size: 27.0 MB (27022323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adb291ac80bc7a7317277f7bf249ff5cee81ed669a710b5737232792791a9f`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.5 MB (3539082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba7d9da50e7339baf72675e0901adcd0e2dfd5d11fe2d97e09d1847f81f5ec`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.7 MB (3713370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896e49ffa5a98b69e4cc86adad3458a6aeb57fd62d4c77c9346d8ae519a7b34e`  
		Last Modified: Wed, 01 Mar 2023 03:14:50 GMT  
		Size: 41.9 MB (41907099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34997242b6cd858fe662b73826646cda831aab2e426f7100e4bea8e85873b8a`  
		Last Modified: Wed, 01 Mar 2023 03:15:21 GMT  
		Size: 142.5 MB (142502823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:caf791e40ac6f0b770478b2a972bb61566b61055bec3c490602002e692e5a750
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241354172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62b8f09e6592d8a2cb59c6daf4d3893cb9f79a786eacb03714fc9684d6668bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:19:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:19:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:19:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:22:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157508d48eacd7b747f0b9c99ce627da62dd75af25ef8cae0d4a18512f51295`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.8 MB (3761409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53567c3f9bdfe731ccd25b9ed68fb667d0fcde2958e4503859e5d2ad3373d169`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.5 MB (3537451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0d60d77f4f4af1d086be5423a3022abc995163617875e8e23be1474f4e24e1`  
		Last Modified: Tue, 31 Jan 2023 18:35:00 GMT  
		Size: 39.2 MB (39245555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717de65a0562bcf94ca5d94a5fb666ddf872d7dd4266e8185585926c9456b276`  
		Last Modified: Tue, 31 Jan 2023 18:35:26 GMT  
		Size: 166.4 MB (166424783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b6ae80b9fadb3a70f3c443d6a93e07d84d9e9d175e9dd6783e47306ca302f375
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271852926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a05dbe2e0f04dd5f4e8161ff88cec0291770a4b2525078673aa8040c1038b68`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:53:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:54:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:58:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b919bd9d6c8a596b3ac4fb9ee1cc6727efdd1f1b05e5c130efec5deaae53ae60`  
		Last Modified: Tue, 31 Jan 2023 17:52:02 GMT  
		Size: 35.7 MB (35708930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59507b6d89bb36f24882056a420b04435132767ba96bd9396f58bc20ed960488`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.3 MB (4261748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc075be4c307553b270bec14a982c75e55b12a8be0e1232b459d394d27745b9`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.2 MB (4234708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e937188d1ea78ae620a3bc6d078cc63b62a04652da54f26e500081c9d671513`  
		Last Modified: Tue, 31 Jan 2023 18:16:58 GMT  
		Size: 43.8 MB (43763369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92d97251e9f8900abcc79cb6a6dd50f43fb01c99e9b1fd976faa362de19c103`  
		Last Modified: Tue, 31 Jan 2023 18:17:52 GMT  
		Size: 183.9 MB (183884171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bb62bc850242365646a2809a31ec247d0fcde4025c4455a9e1b2c9a8e012d4a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223700429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3bcc113c5afc55cc232bf30c91750911ed6bc45e2a5e111b279a87548ec789`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:42:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:43:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:45:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d244ff6bc0f1d8aab1af2badfb1f1ea2f619ca2316288c519afed909e08b35`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.8 MB (3792000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165dd3ed55b51c4b79b3be0051fe345d5b7e6bedbac65941ff7793e50e07420f`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.5 MB (3472764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bdc26d335cd59059e8429dd773b96bf895a6a3ba4f780d1f01410bfcc95406`  
		Last Modified: Tue, 31 Jan 2023 17:55:46 GMT  
		Size: 39.3 MB (39281842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc1cc2e9a60306dacea281a04f4ce4c694dd1f337848c27c007323cd75c2d3a`  
		Last Modified: Tue, 31 Jan 2023 17:56:09 GMT  
		Size: 148.5 MB (148511897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-curl`

```console
$ docker pull buildpack-deps@sha256:77593d112e66c76bcb5a721c77ab1800fc5b926a98ad0f371ef477d1f59fafdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f5e6509df320f7774bd73272759602386e5d645fe971116c7dbed0f38e5fdd9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37778730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2441c30f4b69d5096de28028237f2028653245ec5675b95f2d0ba43db75d04bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:48:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec15466900398b5d701c68ab4f91684333cee7a531fee222d5fcb8a8a7b20d`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.8 MB (3788240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91ea6918177a2aa7ef5f879923eaccfb2e1ddaca74cc714d50e7132ffe71309`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.6 MB (3561486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:81c8f547fdd0f4bf9a2ca2f8f03a7269c827b263ce8a97f9fa154ff0c238a49b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34274775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c2f1e2b1fdc4443fba9a9bf00e489d2d7af1f3e886c967e6d9ad67efcb8888e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:50:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d0210273e3495988f639f6164118a5bba55666799ba86ac3e60a001cf7be3b31`  
		Last Modified: Thu, 26 Jan 2023 18:27:33 GMT  
		Size: 27.0 MB (27022323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adb291ac80bc7a7317277f7bf249ff5cee81ed669a710b5737232792791a9f`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.5 MB (3539082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba7d9da50e7339baf72675e0901adcd0e2dfd5d11fe2d97e09d1847f81f5ec`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.7 MB (3713370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:32acc0bceb4b1c5c72adca26c93d797456c8c103acfbd50cd2eda82ee7dbb3f9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35683834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bdaf7c5d9feef034d451541b098820f1836d948fcfe9d0503d7eecc5f27526`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:19:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:19:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157508d48eacd7b747f0b9c99ce627da62dd75af25ef8cae0d4a18512f51295`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.8 MB (3761409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53567c3f9bdfe731ccd25b9ed68fb667d0fcde2958e4503859e5d2ad3373d169`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.5 MB (3537451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b739e985cfa01beb77701e6fda59cbee4cac87054300d98a262a007bc00307fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44205386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f056e39bef72c9a8e678fd7d9cf620857f579ef83f6b5249fddeb1b5edaec956`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:53:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b919bd9d6c8a596b3ac4fb9ee1cc6727efdd1f1b05e5c130efec5deaae53ae60`  
		Last Modified: Tue, 31 Jan 2023 17:52:02 GMT  
		Size: 35.7 MB (35708930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59507b6d89bb36f24882056a420b04435132767ba96bd9396f58bc20ed960488`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.3 MB (4261748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc075be4c307553b270bec14a982c75e55b12a8be0e1232b459d394d27745b9`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.2 MB (4234708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:64c9f347cc5b6931002286f26b60966f7c186b2cde74c1a07cf6a9fbf4d4377d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35906690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e80805a3881c6a17e1e4319a43ce51e28dd9e4c9c2d2fe2e6264526e9a854082`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:42:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d244ff6bc0f1d8aab1af2badfb1f1ea2f619ca2316288c519afed909e08b35`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.8 MB (3792000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165dd3ed55b51c4b79b3be0051fe345d5b7e6bedbac65941ff7793e50e07420f`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.5 MB (3472764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-scm`

```console
$ docker pull buildpack-deps@sha256:3c5a7f839c140e03c5210ed96ff4431a338cedf298fe76f68826c4f7e8f6314d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:454e170619b5a1fb45cef7bdc6018f456604aecc3a666421048f3b3634964fff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77132297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4fe1d95d55417c7a0fa773212bafbad5fd48a1289f797a988afa9f6ba146653`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:48:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:48:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec15466900398b5d701c68ab4f91684333cee7a531fee222d5fcb8a8a7b20d`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.8 MB (3788240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91ea6918177a2aa7ef5f879923eaccfb2e1ddaca74cc714d50e7132ffe71309`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.6 MB (3561486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a44fd0db0640850be18488f070ec215526d9623b7ae525fac72b3f7e3c8efe2`  
		Last Modified: Tue, 31 Jan 2023 18:02:55 GMT  
		Size: 39.4 MB (39353567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:14b4d1303ec69612ce0d88d0010e45653d7be25d82d48b970925729d826d978d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76181874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a08f78865a253a9d8a65f0544013cf8ddd7c3013aa999a473a82dabc4c5e02`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:50:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:51:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d0210273e3495988f639f6164118a5bba55666799ba86ac3e60a001cf7be3b31`  
		Last Modified: Thu, 26 Jan 2023 18:27:33 GMT  
		Size: 27.0 MB (27022323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adb291ac80bc7a7317277f7bf249ff5cee81ed669a710b5737232792791a9f`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.5 MB (3539082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba7d9da50e7339baf72675e0901adcd0e2dfd5d11fe2d97e09d1847f81f5ec`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.7 MB (3713370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896e49ffa5a98b69e4cc86adad3458a6aeb57fd62d4c77c9346d8ae519a7b34e`  
		Last Modified: Wed, 01 Mar 2023 03:14:50 GMT  
		Size: 41.9 MB (41907099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b6bd1a02efc77bf123fcae7c5524a04f64b272c6a10a3331bdcad862a4fd9d83
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74929389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd560f6d4173dc6a3a41c956564e75c8ad5aa0ff7772f15509939d87cb2c831`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:19:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:19:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:19:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157508d48eacd7b747f0b9c99ce627da62dd75af25ef8cae0d4a18512f51295`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.8 MB (3761409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53567c3f9bdfe731ccd25b9ed68fb667d0fcde2958e4503859e5d2ad3373d169`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.5 MB (3537451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0d60d77f4f4af1d086be5423a3022abc995163617875e8e23be1474f4e24e1`  
		Last Modified: Tue, 31 Jan 2023 18:35:00 GMT  
		Size: 39.2 MB (39245555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:78a62961a5c701ae4bb9459ad0c52261017b9f3b55272c5e4bb4a0796cb3decf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87968755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78a2a507eba7bb61c03b0fd5655bd066d3b7169c709e287b5dc6e1976413cbe9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:53:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:54:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b919bd9d6c8a596b3ac4fb9ee1cc6727efdd1f1b05e5c130efec5deaae53ae60`  
		Last Modified: Tue, 31 Jan 2023 17:52:02 GMT  
		Size: 35.7 MB (35708930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59507b6d89bb36f24882056a420b04435132767ba96bd9396f58bc20ed960488`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.3 MB (4261748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc075be4c307553b270bec14a982c75e55b12a8be0e1232b459d394d27745b9`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.2 MB (4234708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e937188d1ea78ae620a3bc6d078cc63b62a04652da54f26e500081c9d671513`  
		Last Modified: Tue, 31 Jan 2023 18:16:58 GMT  
		Size: 43.8 MB (43763369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:42d39982209dec20dda4c1a0eb82aa5f7965e10ddf4762b57d79d8a32dc0ad5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75188532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92676457c8f951741aa984be933cefc329a160a810bc49d61775949c32487a82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:42:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:43:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d244ff6bc0f1d8aab1af2badfb1f1ea2f619ca2316288c519afed909e08b35`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.8 MB (3792000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165dd3ed55b51c4b79b3be0051fe345d5b7e6bedbac65941ff7793e50e07420f`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.5 MB (3472764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bdc26d335cd59059e8429dd773b96bf895a6a3ba4f780d1f01410bfcc95406`  
		Last Modified: Tue, 31 Jan 2023 17:55:46 GMT  
		Size: 39.3 MB (39281842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10`

```console
$ docker pull buildpack-deps@sha256:7d4d71ac75f26b243c8409094b796b8f0a8cc231241262f5babe6d5e7b10309e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.10` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3a758ae57c8a7346ba305b53acd626f697ff9eb9f0a1bc2e35ed8aa0fd4090cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.7 MB (258713730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9ffcea5f1bfb263a26234b8ad41d79b047fde2acbf3c33f0f64f7d3e7a27f0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:51:12 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:51:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:51:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:51:13 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:51:14 GMT
ADD file:e886423892b371751386c0ce7147599acb72d8fb528eaaa78092b879d9ff58ce in / 
# Thu, 26 Jan 2023 11:51:15 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:52:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:52:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:55:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62a5d402f83137154c8e54f4f370e9f9f70b5a6892f6ec8cc2fae7be0fd8ae91`  
		Last Modified: Tue, 31 Jan 2023 18:03:39 GMT  
		Size: 27.5 MB (27479169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f8f31e97bc8f200f610260668952e0a909150c1e95f494e3165edd6a4e74d`  
		Last Modified: Tue, 31 Jan 2023 18:03:36 GMT  
		Size: 6.8 MB (6764654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddf4e3936d1208458d4e3e5395b8b86da6f3f7ef3b30242decd50ee0403f1e9`  
		Last Modified: Tue, 31 Jan 2023 18:03:35 GMT  
		Size: 3.6 MB (3635171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b0d398ef08d48d4f39203eb13897978a42e2aa1da1465591c472c03f5975ec`  
		Last Modified: Tue, 31 Jan 2023 18:03:53 GMT  
		Size: 39.7 MB (39740240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01848c64b150b130ec1ae2bc4551ec1f49701b2de7a636fb9197ed2381f48a9`  
		Last Modified: Tue, 31 Jan 2023 18:04:26 GMT  
		Size: 181.1 MB (181094496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:07ca08046c135432af3c0105454a2cb893bf741d6c9275bd43a1fa73d344ae15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.0 MB (221026709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04a755b1a8dff6a40b4cd35245c8f32599ccad2ef814341f3843a5c84ce63d57`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:52:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:52:03 GMT
ADD file:d35c57b0dc2840a8b1ef40f7f6cfd826da68611f1ba37a89a382618c8612b52c in / 
# Thu, 26 Jan 2023 11:52:03 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:56:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:57:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:00:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:697d38f8dfe625e3e751c0b01ddeaaeeff6e8d6f594dd7da227aea3974a49ce1`  
		Last Modified: Thu, 26 Jan 2023 12:14:16 GMT  
		Size: 25.1 MB (25066997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404f4cb6d67c78771ca841794019841127207d81397dddc44c0de7b2a042428`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 5.9 MB (5940499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fa0889fdc983e7d5186fd6c7c7d65241a345cd87db62b962cc1ac632edba88`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 3.8 MB (3800405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cfdc6c62b64f7606245b4e8a795a610e9495fee93fe702f9b6d05ad773b238`  
		Last Modified: Wed, 01 Mar 2023 03:15:50 GMT  
		Size: 42.6 MB (42606983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4061239f68932a6818d689fc46f2f9e4b67bda3c98c4f57d7665d86b78c8c4`  
		Last Modified: Wed, 01 Mar 2023 03:16:21 GMT  
		Size: 143.6 MB (143611825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:75712c8314b8699bf216ddf2252b05b7650004e43c3f63f261d00feb65a3b6a9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.7 MB (246697214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a2c33d0062a7f8588a0cb9df7c0fdd2f82dde2c2faa4468870ad8b74412aa2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:18 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:20 GMT
ADD file:f61617371f6963c6be2852e2b94d04e8507feb8f77e3484c94aa8b9d0ac67f76 in / 
# Thu, 26 Jan 2023 12:08:20 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:23:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:24:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:27:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44d97c2a5ae0fb5d56de8a6242583e80e9265c58a742eb1e52d40264d9f034e9`  
		Last Modified: Tue, 31 Jan 2023 18:35:38 GMT  
		Size: 26.7 MB (26699721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3b285ead03b32399f7eb21eb63769c45b64c8b1731dfc244904cc2e9a8262a`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 6.6 MB (6595500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855afc623fecc9cad347ac6e791b5bb08dd8331201f22400b2764672b1e9a48c`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 3.6 MB (3602406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8fe5b73117b2d29e76fe2d924c4310d621681b761a3e4efcce5bd6842cb3e`  
		Last Modified: Tue, 31 Jan 2023 18:35:51 GMT  
		Size: 39.5 MB (39523097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a13a0356c3c1fefb6afeae0373f345a4200ce0ef8d8c9e383948efc6d1c22d`  
		Last Modified: Tue, 31 Jan 2023 18:36:20 GMT  
		Size: 170.3 MB (170276490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:39314d421779e71395dbf25c5a7c7a6ef6515a692304a576870c50b83b208938
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281283945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1378e98d0d7fb14e25257a0ba00eb60fc2e01ca1b97ceaa7a95eef16b9248db6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:57:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:57:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:57:03 GMT
ADD file:3c2bc98d283cce5149d7992233f5fe644b7239417045faf3f93750b92de5f68e in / 
# Thu, 26 Jan 2023 11:57:04 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:59:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:04:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a06c15ccb04b9b73efad888bdc885d26bd74537d9322b6629f3b3ef906c0756`  
		Last Modified: Tue, 31 Jan 2023 18:18:11 GMT  
		Size: 32.1 MB (32109752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ee7c83faf85e0ce7383151d494b3fbc177d548f264c95b2dcbf49dca2d06d2`  
		Last Modified: Tue, 31 Jan 2023 18:18:05 GMT  
		Size: 7.7 MB (7741886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e688b449cdca40b587631310483952ae87bf319f0b7d13251a6a085f60c05db4`  
		Last Modified: Tue, 31 Jan 2023 18:18:04 GMT  
		Size: 4.4 MB (4362437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecff49481c045e5964caf1cd33337e518465376e603f708da227d433ae19a74c`  
		Last Modified: Tue, 31 Jan 2023 18:18:35 GMT  
		Size: 44.1 MB (44142262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbb04761be0c3739265acca2d4d506ca2d2a045b958a8b9c295a0c33484a051`  
		Last Modified: Tue, 31 Jan 2023 18:19:33 GMT  
		Size: 192.9 MB (192927608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4d1b7f50c9f545d3504d52d8a1cd6dd4a15ce64ab075d2f1955dcef467fc3a47
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228596958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81d546f7822fba9006d358b9d186652f2af4a869ec2464c6c390bd1dd2ef6c9c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:47 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:50 GMT
ADD file:a83afd93816f868be76d243df85b87a66b39d5ef0497c3cb8d0bba2bd4a27c40 in / 
# Thu, 26 Jan 2023 12:08:50 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:45:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:46:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:48:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5bec5e5b1f8afd82addaa8ef129ee5026d804c474c34ca3e565dfa18fa5f877`  
		Last Modified: Tue, 31 Jan 2023 17:56:19 GMT  
		Size: 26.0 MB (26029773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888884268a5ab3f78486597366fa902253286ebe039958a9950d8ab78853d5c5`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 6.5 MB (6457669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7aa7ab93554822a6ee5149dc403f0ba1aa47ed227911574510630a9383bf8f`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 3.6 MB (3625074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173761a853e728963d055e12ba7bf5951b85d93c0ac60955fa793be53aa69f57`  
		Last Modified: Tue, 31 Jan 2023 17:56:31 GMT  
		Size: 39.6 MB (39552159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2930464a0032aa36dbe69f2c0b3faceaa7a67f8de234438b28d703357998a09c`  
		Last Modified: Tue, 31 Jan 2023 17:56:55 GMT  
		Size: 152.9 MB (152932283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-curl`

```console
$ docker pull buildpack-deps@sha256:d446c39e8b9aa2eb7699b23def524d291bdc0d5c0fc50556d2123633348b658e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.10-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:aee83996c48b86aeb5b790a31fe66a215e9925a3476a210d23b74f1ed7217bc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37878994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154ba55bc0e297c9fb12b70cceafd72e5fb510e6be0838aeac5e673ba3eb83b0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:51:12 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:51:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:51:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:51:13 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:51:14 GMT
ADD file:e886423892b371751386c0ce7147599acb72d8fb528eaaa78092b879d9ff58ce in / 
# Thu, 26 Jan 2023 11:51:15 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:52:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:52:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:62a5d402f83137154c8e54f4f370e9f9f70b5a6892f6ec8cc2fae7be0fd8ae91`  
		Last Modified: Tue, 31 Jan 2023 18:03:39 GMT  
		Size: 27.5 MB (27479169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f8f31e97bc8f200f610260668952e0a909150c1e95f494e3165edd6a4e74d`  
		Last Modified: Tue, 31 Jan 2023 18:03:36 GMT  
		Size: 6.8 MB (6764654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddf4e3936d1208458d4e3e5395b8b86da6f3f7ef3b30242decd50ee0403f1e9`  
		Last Modified: Tue, 31 Jan 2023 18:03:35 GMT  
		Size: 3.6 MB (3635171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:138bf1078343221e08092695ceb35b3b4786103d589ba18af108a037e5f2fb02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34807901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3a38c11fedc1ac56d6be15d7180635f23c3420b28e4c6174b521908a0083a1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:52:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:52:03 GMT
ADD file:d35c57b0dc2840a8b1ef40f7f6cfd826da68611f1ba37a89a382618c8612b52c in / 
# Thu, 26 Jan 2023 11:52:03 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:56:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:697d38f8dfe625e3e751c0b01ddeaaeeff6e8d6f594dd7da227aea3974a49ce1`  
		Last Modified: Thu, 26 Jan 2023 12:14:16 GMT  
		Size: 25.1 MB (25066997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404f4cb6d67c78771ca841794019841127207d81397dddc44c0de7b2a042428`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 5.9 MB (5940499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fa0889fdc983e7d5186fd6c7c7d65241a345cd87db62b962cc1ac632edba88`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 3.8 MB (3800405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:459333d1097d8ab2a535f9c41fd9eff41b7f5820d2c47c0d962e093657486976
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36897627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9f0ccf2c259d8726bab173cdcb0552efa2ef70239be80ab1d4ec8c83bd6a86e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:18 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:20 GMT
ADD file:f61617371f6963c6be2852e2b94d04e8507feb8f77e3484c94aa8b9d0ac67f76 in / 
# Thu, 26 Jan 2023 12:08:20 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:23:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:44d97c2a5ae0fb5d56de8a6242583e80e9265c58a742eb1e52d40264d9f034e9`  
		Last Modified: Tue, 31 Jan 2023 18:35:38 GMT  
		Size: 26.7 MB (26699721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3b285ead03b32399f7eb21eb63769c45b64c8b1731dfc244904cc2e9a8262a`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 6.6 MB (6595500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855afc623fecc9cad347ac6e791b5bb08dd8331201f22400b2764672b1e9a48c`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 3.6 MB (3602406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:055376708ea1867e94b93cf561f8cef6c53ee9ef58b8b61cd47ead6df152da8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44214075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6297083ca03c278a01cf0c0652d9765e62bcb400e73228e55692cf5c25319c77`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:57:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:57:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:57:03 GMT
ADD file:3c2bc98d283cce5149d7992233f5fe644b7239417045faf3f93750b92de5f68e in / 
# Thu, 26 Jan 2023 11:57:04 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:59:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6a06c15ccb04b9b73efad888bdc885d26bd74537d9322b6629f3b3ef906c0756`  
		Last Modified: Tue, 31 Jan 2023 18:18:11 GMT  
		Size: 32.1 MB (32109752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ee7c83faf85e0ce7383151d494b3fbc177d548f264c95b2dcbf49dca2d06d2`  
		Last Modified: Tue, 31 Jan 2023 18:18:05 GMT  
		Size: 7.7 MB (7741886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e688b449cdca40b587631310483952ae87bf319f0b7d13251a6a085f60c05db4`  
		Last Modified: Tue, 31 Jan 2023 18:18:04 GMT  
		Size: 4.4 MB (4362437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:832891dce637dd6a45a4d5349c2792f04ad3f518c1596702561171552b5eb5fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36112516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4326242fb08207106428f6944530b3e0d79c30fcfb112b958bcf78cf90ad2b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:47 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:50 GMT
ADD file:a83afd93816f868be76d243df85b87a66b39d5ef0497c3cb8d0bba2bd4a27c40 in / 
# Thu, 26 Jan 2023 12:08:50 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:45:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a5bec5e5b1f8afd82addaa8ef129ee5026d804c474c34ca3e565dfa18fa5f877`  
		Last Modified: Tue, 31 Jan 2023 17:56:19 GMT  
		Size: 26.0 MB (26029773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888884268a5ab3f78486597366fa902253286ebe039958a9950d8ab78853d5c5`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 6.5 MB (6457669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7aa7ab93554822a6ee5149dc403f0ba1aa47ed227911574510630a9383bf8f`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 3.6 MB (3625074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-scm`

```console
$ docker pull buildpack-deps@sha256:9054ceda293660bef628525b88aa77598174bc7a55d364ca2be3c855d7cb69cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.10-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5d4e37dd49baaa117ef3d71a175e2b65793fb2ccb4df8a9e401c9b8ee1905393
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77619234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a378bfcf3067410dc87bed8f89e0c492ceb4927beca11af10ffc6f972865637`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:51:12 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:51:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:51:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:51:13 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:51:14 GMT
ADD file:e886423892b371751386c0ce7147599acb72d8fb528eaaa78092b879d9ff58ce in / 
# Thu, 26 Jan 2023 11:51:15 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:52:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:52:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62a5d402f83137154c8e54f4f370e9f9f70b5a6892f6ec8cc2fae7be0fd8ae91`  
		Last Modified: Tue, 31 Jan 2023 18:03:39 GMT  
		Size: 27.5 MB (27479169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f8f31e97bc8f200f610260668952e0a909150c1e95f494e3165edd6a4e74d`  
		Last Modified: Tue, 31 Jan 2023 18:03:36 GMT  
		Size: 6.8 MB (6764654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddf4e3936d1208458d4e3e5395b8b86da6f3f7ef3b30242decd50ee0403f1e9`  
		Last Modified: Tue, 31 Jan 2023 18:03:35 GMT  
		Size: 3.6 MB (3635171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b0d398ef08d48d4f39203eb13897978a42e2aa1da1465591c472c03f5975ec`  
		Last Modified: Tue, 31 Jan 2023 18:03:53 GMT  
		Size: 39.7 MB (39740240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:df9482f8aafc2f7b4abf8e2fff63de1427eae9c4e93ef78925b89c7207497450
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.4 MB (77414884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27db2823f44839863528aacd8914aa05e7f260dbb2373b0ffab72dcc1f60457f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:52:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:52:03 GMT
ADD file:d35c57b0dc2840a8b1ef40f7f6cfd826da68611f1ba37a89a382618c8612b52c in / 
# Thu, 26 Jan 2023 11:52:03 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:56:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:57:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:697d38f8dfe625e3e751c0b01ddeaaeeff6e8d6f594dd7da227aea3974a49ce1`  
		Last Modified: Thu, 26 Jan 2023 12:14:16 GMT  
		Size: 25.1 MB (25066997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404f4cb6d67c78771ca841794019841127207d81397dddc44c0de7b2a042428`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 5.9 MB (5940499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fa0889fdc983e7d5186fd6c7c7d65241a345cd87db62b962cc1ac632edba88`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 3.8 MB (3800405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cfdc6c62b64f7606245b4e8a795a610e9495fee93fe702f9b6d05ad773b238`  
		Last Modified: Wed, 01 Mar 2023 03:15:50 GMT  
		Size: 42.6 MB (42606983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7122957b9251055a81faead01a15fbd23d457f0f694320c75c72e167bae939c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76420724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1a7465b31ec6c65ee04ea8cd0b6fcb28a729ef78f9c54f094a85d16eb4d7e84`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:18 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:20 GMT
ADD file:f61617371f6963c6be2852e2b94d04e8507feb8f77e3484c94aa8b9d0ac67f76 in / 
# Thu, 26 Jan 2023 12:08:20 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:23:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:24:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44d97c2a5ae0fb5d56de8a6242583e80e9265c58a742eb1e52d40264d9f034e9`  
		Last Modified: Tue, 31 Jan 2023 18:35:38 GMT  
		Size: 26.7 MB (26699721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3b285ead03b32399f7eb21eb63769c45b64c8b1731dfc244904cc2e9a8262a`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 6.6 MB (6595500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855afc623fecc9cad347ac6e791b5bb08dd8331201f22400b2764672b1e9a48c`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 3.6 MB (3602406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8fe5b73117b2d29e76fe2d924c4310d621681b761a3e4efcce5bd6842cb3e`  
		Last Modified: Tue, 31 Jan 2023 18:35:51 GMT  
		Size: 39.5 MB (39523097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a92b717633421c919c8437841cec0c8fe13b56c6c1448937c07a7f37c01a7ebb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88356337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c053aa26c6dbf33d593218945dffc872660a52734291c7d1b459c175ecdcfb05`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:57:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:57:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:57:03 GMT
ADD file:3c2bc98d283cce5149d7992233f5fe644b7239417045faf3f93750b92de5f68e in / 
# Thu, 26 Jan 2023 11:57:04 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:59:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a06c15ccb04b9b73efad888bdc885d26bd74537d9322b6629f3b3ef906c0756`  
		Last Modified: Tue, 31 Jan 2023 18:18:11 GMT  
		Size: 32.1 MB (32109752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ee7c83faf85e0ce7383151d494b3fbc177d548f264c95b2dcbf49dca2d06d2`  
		Last Modified: Tue, 31 Jan 2023 18:18:05 GMT  
		Size: 7.7 MB (7741886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e688b449cdca40b587631310483952ae87bf319f0b7d13251a6a085f60c05db4`  
		Last Modified: Tue, 31 Jan 2023 18:18:04 GMT  
		Size: 4.4 MB (4362437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecff49481c045e5964caf1cd33337e518465376e603f708da227d433ae19a74c`  
		Last Modified: Tue, 31 Jan 2023 18:18:35 GMT  
		Size: 44.1 MB (44142262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8aa73932942674acc171a5ab84eec601e912cf168a5949af6fbbd9b42e1b0114
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75664675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f39289322452926c88ff808fa932fca05a4903be6317283d1fe28e26c0fc154`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:47 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:50 GMT
ADD file:a83afd93816f868be76d243df85b87a66b39d5ef0497c3cb8d0bba2bd4a27c40 in / 
# Thu, 26 Jan 2023 12:08:50 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:45:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:46:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5bec5e5b1f8afd82addaa8ef129ee5026d804c474c34ca3e565dfa18fa5f877`  
		Last Modified: Tue, 31 Jan 2023 17:56:19 GMT  
		Size: 26.0 MB (26029773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888884268a5ab3f78486597366fa902253286ebe039958a9950d8ab78853d5c5`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 6.5 MB (6457669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7aa7ab93554822a6ee5149dc403f0ba1aa47ed227911574510630a9383bf8f`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 3.6 MB (3625074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173761a853e728963d055e12ba7bf5951b85d93c0ac60955fa793be53aa69f57`  
		Last Modified: Tue, 31 Jan 2023 17:56:31 GMT  
		Size: 39.6 MB (39552159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04`

```console
$ docker pull buildpack-deps@sha256:b6c8f6bfaf6ebc9ffa3ac4a7f91829fd0b1040f3fb14d470c045c693ddec41e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6afd26c62d559b4fa71aa25b11d68f20128236eba753b8c8b78c82048a01ee7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.3 MB (258330292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44a9ffc7d1ca5998e864650d5669556b2dd055296fb3a8a33b7a2c8f13aff074`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:15:52 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:15:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:15:54 GMT
ADD file:915f1a27db0a8b9a9dd58d40086cb7d45b2722e8ceb29ed8bcb306d4dcd3688e in / 
# Sat, 28 Jan 2023 05:15:54 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:12:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:21:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7610e15a5bf822d71b65f5f7c7d873b70f585cebc9b4bfd76dedd61997f9e1c2`  
		Last Modified: Wed, 01 Feb 2023 18:23:55 GMT  
		Size: 27.4 MB (27419700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc4589b98247ebd93b0b4ca6c08ebf74c1fcb7fe81d1ee3a00ddd0381b99aaa`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 6.6 MB (6635143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c87abeb95cddddf017930e8ffec58593bd520216c779b25e710376682a56c6`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 3.7 MB (3690296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b97131389bee769ba93a32a51aee8b1f6fa2936b506cd9be1296fe2e9ef3d`  
		Last Modified: Wed, 01 Feb 2023 18:24:10 GMT  
		Size: 40.9 MB (40948895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dba4cd6fa73d5141eb96b8088c1a0ab5efb6125eb26b9aab86cca0e7f172ec`  
		Last Modified: Wed, 01 Feb 2023 18:24:44 GMT  
		Size: 179.6 MB (179636258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4c79aad28f82a6612c1d9a32df92cce9c2e7498061c8c485b2fe2554f851e965
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.7 MB (244651591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f73b6dab560b07c846121f5172e0c5f76c67989f848e3ec9d236d0d695dd93`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:25 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:31 GMT
ADD file:c0ac354f01ba9deb72bda06f4368650e0cc3ad5c3425ce0eb452561b56a1734a in / 
# Sat, 28 Jan 2023 05:11:32 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 03:01:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:01:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:02:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:05:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2cf733a376b355703d852c37fb66314a9d27adeb140641f229bd7d5b089c8ef7`  
		Last Modified: Sat, 28 Jan 2023 05:21:37 GMT  
		Size: 25.1 MB (25086001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8391c317b70a65f7c7d5bf15686f27d06e2c79b286c3a86cb70987de2acdc4`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 5.8 MB (5808831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd77c8b93dd4f4c7b1af018a1de3fc89606fac50a049b8ee85bd1ccd0335294`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 3.9 MB (3851906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9367c233564b3534a29ad60c3843f0bbd6a4105cc65519f48f91cf119358142`  
		Last Modified: Wed, 01 Mar 2023 03:16:51 GMT  
		Size: 48.6 MB (48602279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c639059702b5fc046342922b5b562597eb8ec1d3fa1484357d33845656e117`  
		Last Modified: Wed, 01 Mar 2023 03:17:23 GMT  
		Size: 161.3 MB (161302574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:914aa413772a5b51585daf8e054b1c90924bb20dcbdb32ef75d72152a9944578
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.4 MB (248385791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16afca163301c787bfd70226721890aa01ca555f65875af6e8202e1d5747985`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:24 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:29 GMT
ADD file:c6e9b4142d0eef696dbc592460bdbd505f41a98d02ba1c7a84caedbb5f84ea1b in / 
# Sat, 28 Jan 2023 05:11:29 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:09:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:10:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:10:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:14:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86b4004853063d73760cb92de14cb3a62665a38c8761227cbb1afdd83e3c2463`  
		Last Modified: Wed, 01 Feb 2023 18:16:40 GMT  
		Size: 26.8 MB (26755970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabf667a5a78f05803b7cfc5334c39586cc72c5e9f5c4b3d057eeaeae60adab9`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 6.5 MB (6468704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f5bbd1102042fd3e0960b145074562a58c2191adc81cbc46fe1f667ee5e5c`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 3.6 MB (3649392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c999a4e8e593fbc5591306b84b879ccd3dede542421a341ded4ce652345c0`  
		Last Modified: Wed, 01 Feb 2023 18:16:53 GMT  
		Size: 40.8 MB (40753202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c74342ec10c904450e8a7bee3d119d1a5124a8e306607a703ca2006f59e5d7`  
		Last Modified: Wed, 01 Feb 2023 18:17:20 GMT  
		Size: 170.8 MB (170758523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:863b48e351486104089d5665e2d2889a5c29940e2995df5037567c62cac0ee36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (282968437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3738e6e9ee8b954e2cb450930080810a2d809f552328fbfddf8a9ad3ee09e2c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:09:15 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:09:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:09:19 GMT
ADD file:1c6ae50eb1e182a9aa8f750f61a615d5b3578b7c2f94e58678359bf1f43d3780 in / 
# Sat, 28 Jan 2023 05:09:19 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:17:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5151cf1d3445f8b719163cb88c8ee7f7f2368e309dd1d14016546804fc05126`  
		Last Modified: Wed, 01 Feb 2023 18:22:34 GMT  
		Size: 32.0 MB (31980199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337c3408ba6fc96792e39145bb0a122a3f04a96a5571d97c3f265402359009c`  
		Last Modified: Wed, 01 Feb 2023 18:22:28 GMT  
		Size: 7.6 MB (7605406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1579dbb09dc76707e4839919fcec93b48be4479e103cb1aeed1a50194d1724e8`  
		Last Modified: Wed, 01 Feb 2023 18:22:27 GMT  
		Size: 4.4 MB (4408979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f651ad714aac8d2542de9fc23ff6b10701efb943ac6c9538ea45be37d726bf0e`  
		Last Modified: Wed, 01 Feb 2023 18:22:57 GMT  
		Size: 45.7 MB (45720315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd9b71849d33f1ac6239db3ee29c7575dcc37fb97cfb76c27f3f0ef8754c45f`  
		Last Modified: Wed, 01 Feb 2023 18:23:55 GMT  
		Size: 193.3 MB (193253538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5a1dac520bcbb95170725e4974c5d3e58177a10b865930b4b7e3fd2f0289b52f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (229954138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:461ca2b8a46d2de7d07b24d64eb0ab47dea82cf2629e45bf12fb050bc95c69f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:10:10 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:10:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:10:12 GMT
ADD file:b85f8b675931991dc4361ad29563c508e8cdd381491f1da64b998d7742f72c42 in / 
# Sat, 28 Jan 2023 05:10:12 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:15:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:16:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:18:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ec11bba63863786b2862fe78b2d89ce7f2cf2ab178c9abc17064e250fc6a07b`  
		Last Modified: Wed, 01 Feb 2023 18:22:06 GMT  
		Size: 26.0 MB (26014630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50701e4538cb519cc258f9f917c69bd16c143f281ac369a90c6aba3f40dcff3`  
		Last Modified: Wed, 01 Feb 2023 18:22:04 GMT  
		Size: 6.3 MB (6318048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c474c2328ae2c175dbac9c35c888383f82da2ae100c9197db0e3a1912be9dd3e`  
		Last Modified: Wed, 01 Feb 2023 18:22:03 GMT  
		Size: 3.7 MB (3674786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eabce57ad05a030ae2bc38b37ffdb539eef43109d4503a2b66e82f71391c9bb`  
		Last Modified: Wed, 01 Feb 2023 18:22:20 GMT  
		Size: 40.7 MB (40730894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b71b0b4891fc62494cfff677b3e282387e98f36b19733cec13dccdae9ab15`  
		Last Modified: Wed, 01 Feb 2023 18:22:49 GMT  
		Size: 153.2 MB (153215780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-curl`

```console
$ docker pull buildpack-deps@sha256:f1e3051d65bd5ac55c65d52254eba29ff0f754b0e6bced73d7224f3e8ea2e3bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:537eea6319443a5bc614bfb7b4e5cdbcfc9e13586c211abcc852eea86d07d663
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37745139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed4daa4196e32ecf36c1e23528d2d324d3d143e881960c908c9b58ddf0fc25f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:15:52 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:15:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:15:54 GMT
ADD file:915f1a27db0a8b9a9dd58d40086cb7d45b2722e8ceb29ed8bcb306d4dcd3688e in / 
# Sat, 28 Jan 2023 05:15:54 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:12:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7610e15a5bf822d71b65f5f7c7d873b70f585cebc9b4bfd76dedd61997f9e1c2`  
		Last Modified: Wed, 01 Feb 2023 18:23:55 GMT  
		Size: 27.4 MB (27419700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc4589b98247ebd93b0b4ca6c08ebf74c1fcb7fe81d1ee3a00ddd0381b99aaa`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 6.6 MB (6635143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c87abeb95cddddf017930e8ffec58593bd520216c779b25e710376682a56c6`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 3.7 MB (3690296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:83263b17a9332b259200af03feb6a20687800485d75e356abdd7e5b2fbb00e5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34746738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f4d40d7a0e65028a158d83cba12d690f50604a982fdde14ea99f2ce6fdf4f3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:25 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:31 GMT
ADD file:c0ac354f01ba9deb72bda06f4368650e0cc3ad5c3425ce0eb452561b56a1734a in / 
# Sat, 28 Jan 2023 05:11:32 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 03:01:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:01:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2cf733a376b355703d852c37fb66314a9d27adeb140641f229bd7d5b089c8ef7`  
		Last Modified: Sat, 28 Jan 2023 05:21:37 GMT  
		Size: 25.1 MB (25086001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8391c317b70a65f7c7d5bf15686f27d06e2c79b286c3a86cb70987de2acdc4`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 5.8 MB (5808831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd77c8b93dd4f4c7b1af018a1de3fc89606fac50a049b8ee85bd1ccd0335294`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 3.9 MB (3851906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c3edb731722f1b63d480271e6f2aaebf090d64c312181d330c9cd0a0e59ca25a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36874066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba32c939dfad52832eb293c54966c05a6b6d0096a74522b05bb10a2b9e0794fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:24 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:29 GMT
ADD file:c6e9b4142d0eef696dbc592460bdbd505f41a98d02ba1c7a84caedbb5f84ea1b in / 
# Sat, 28 Jan 2023 05:11:29 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:09:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:10:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:86b4004853063d73760cb92de14cb3a62665a38c8761227cbb1afdd83e3c2463`  
		Last Modified: Wed, 01 Feb 2023 18:16:40 GMT  
		Size: 26.8 MB (26755970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabf667a5a78f05803b7cfc5334c39586cc72c5e9f5c4b3d057eeaeae60adab9`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 6.5 MB (6468704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f5bbd1102042fd3e0960b145074562a58c2191adc81cbc46fe1f667ee5e5c`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 3.6 MB (3649392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2689fc68d1712090df249e5b92394fd8e147aa8e4b4f419a4849f377c21814cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43994584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:706de3f8b9b6b3b56436cd6c5541d09d59ab09b125fc6596f1b13d0ca35e3c3a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:09:15 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:09:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:09:19 GMT
ADD file:1c6ae50eb1e182a9aa8f750f61a615d5b3578b7c2f94e58678359bf1f43d3780 in / 
# Sat, 28 Jan 2023 05:09:19 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a5151cf1d3445f8b719163cb88c8ee7f7f2368e309dd1d14016546804fc05126`  
		Last Modified: Wed, 01 Feb 2023 18:22:34 GMT  
		Size: 32.0 MB (31980199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337c3408ba6fc96792e39145bb0a122a3f04a96a5571d97c3f265402359009c`  
		Last Modified: Wed, 01 Feb 2023 18:22:28 GMT  
		Size: 7.6 MB (7605406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1579dbb09dc76707e4839919fcec93b48be4479e103cb1aeed1a50194d1724e8`  
		Last Modified: Wed, 01 Feb 2023 18:22:27 GMT  
		Size: 4.4 MB (4408979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ade0a2429605778da48e86e85150f3bde89379b8572cc40bc9e5b466ddfe2d4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36007464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f4f980c08a961d5e32890459371417c50d867990d96e3ba9fbf9de7ce406ea8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:10:10 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:10:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:10:12 GMT
ADD file:b85f8b675931991dc4361ad29563c508e8cdd381491f1da64b998d7742f72c42 in / 
# Sat, 28 Jan 2023 05:10:12 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:15:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2ec11bba63863786b2862fe78b2d89ce7f2cf2ab178c9abc17064e250fc6a07b`  
		Last Modified: Wed, 01 Feb 2023 18:22:06 GMT  
		Size: 26.0 MB (26014630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50701e4538cb519cc258f9f917c69bd16c143f281ac369a90c6aba3f40dcff3`  
		Last Modified: Wed, 01 Feb 2023 18:22:04 GMT  
		Size: 6.3 MB (6318048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c474c2328ae2c175dbac9c35c888383f82da2ae100c9197db0e3a1912be9dd3e`  
		Last Modified: Wed, 01 Feb 2023 18:22:03 GMT  
		Size: 3.7 MB (3674786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-scm`

```console
$ docker pull buildpack-deps@sha256:606403063d0774c59bdfdf8cec41792762059428f2335758b767a8a6419d131e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f4779bb631cc96f8c601cb3cb2d4d19fc819689d534b0ec2049fb2aeb96b7e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.7 MB (78694034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90cccf588560d124231ebdcf5f275b4e27dbb214d9bf110989c70b375d2885f9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:15:52 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:15:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:15:54 GMT
ADD file:915f1a27db0a8b9a9dd58d40086cb7d45b2722e8ceb29ed8bcb306d4dcd3688e in / 
# Sat, 28 Jan 2023 05:15:54 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:12:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7610e15a5bf822d71b65f5f7c7d873b70f585cebc9b4bfd76dedd61997f9e1c2`  
		Last Modified: Wed, 01 Feb 2023 18:23:55 GMT  
		Size: 27.4 MB (27419700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc4589b98247ebd93b0b4ca6c08ebf74c1fcb7fe81d1ee3a00ddd0381b99aaa`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 6.6 MB (6635143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c87abeb95cddddf017930e8ffec58593bd520216c779b25e710376682a56c6`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 3.7 MB (3690296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b97131389bee769ba93a32a51aee8b1f6fa2936b506cd9be1296fe2e9ef3d`  
		Last Modified: Wed, 01 Feb 2023 18:24:10 GMT  
		Size: 40.9 MB (40948895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:049d82e7a50c297020943bab44d6ae17ffc80d524d72a34544bdffde74443213
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83349017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbaabfc7bbbedab1780b20eaee19155a1c5b9ebf58df1fc9f4f1df55b732b84e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:25 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:31 GMT
ADD file:c0ac354f01ba9deb72bda06f4368650e0cc3ad5c3425ce0eb452561b56a1734a in / 
# Sat, 28 Jan 2023 05:11:32 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 03:01:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:01:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:02:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2cf733a376b355703d852c37fb66314a9d27adeb140641f229bd7d5b089c8ef7`  
		Last Modified: Sat, 28 Jan 2023 05:21:37 GMT  
		Size: 25.1 MB (25086001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8391c317b70a65f7c7d5bf15686f27d06e2c79b286c3a86cb70987de2acdc4`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 5.8 MB (5808831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd77c8b93dd4f4c7b1af018a1de3fc89606fac50a049b8ee85bd1ccd0335294`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 3.9 MB (3851906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9367c233564b3534a29ad60c3843f0bbd6a4105cc65519f48f91cf119358142`  
		Last Modified: Wed, 01 Mar 2023 03:16:51 GMT  
		Size: 48.6 MB (48602279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:42463b1fa0a388d9801a062d9dd40ea8d72b288e886e5dd7ace63d7c8e99274a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77627268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9d5f1d5f2a4e64bbe95c49ca9314c9030fdcc07106445d0f6c7fa7d59d897a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:24 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:29 GMT
ADD file:c6e9b4142d0eef696dbc592460bdbd505f41a98d02ba1c7a84caedbb5f84ea1b in / 
# Sat, 28 Jan 2023 05:11:29 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:09:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:10:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:10:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86b4004853063d73760cb92de14cb3a62665a38c8761227cbb1afdd83e3c2463`  
		Last Modified: Wed, 01 Feb 2023 18:16:40 GMT  
		Size: 26.8 MB (26755970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabf667a5a78f05803b7cfc5334c39586cc72c5e9f5c4b3d057eeaeae60adab9`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 6.5 MB (6468704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f5bbd1102042fd3e0960b145074562a58c2191adc81cbc46fe1f667ee5e5c`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 3.6 MB (3649392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c999a4e8e593fbc5591306b84b879ccd3dede542421a341ded4ce652345c0`  
		Last Modified: Wed, 01 Feb 2023 18:16:53 GMT  
		Size: 40.8 MB (40753202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a805a109b7caa13d3e7983ef1c11492c18454c10000ddc6c90fc09528e3427ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89714899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76476df3dde3cb0032f781c70db091e82cc22df5fee40845b4036edc34bda10d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:09:15 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:09:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:09:19 GMT
ADD file:1c6ae50eb1e182a9aa8f750f61a615d5b3578b7c2f94e58678359bf1f43d3780 in / 
# Sat, 28 Jan 2023 05:09:19 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5151cf1d3445f8b719163cb88c8ee7f7f2368e309dd1d14016546804fc05126`  
		Last Modified: Wed, 01 Feb 2023 18:22:34 GMT  
		Size: 32.0 MB (31980199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337c3408ba6fc96792e39145bb0a122a3f04a96a5571d97c3f265402359009c`  
		Last Modified: Wed, 01 Feb 2023 18:22:28 GMT  
		Size: 7.6 MB (7605406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1579dbb09dc76707e4839919fcec93b48be4479e103cb1aeed1a50194d1724e8`  
		Last Modified: Wed, 01 Feb 2023 18:22:27 GMT  
		Size: 4.4 MB (4408979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f651ad714aac8d2542de9fc23ff6b10701efb943ac6c9538ea45be37d726bf0e`  
		Last Modified: Wed, 01 Feb 2023 18:22:57 GMT  
		Size: 45.7 MB (45720315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:288d9bb7ed13a2a668f51e523fa6f73bb6cd8611fb7903414940a9b02618f78d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.7 MB (76738358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5814b74a158bb3239700bd17ecef82d37a7e245364d85b0f074b6e447ba0d37a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:10:10 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:10:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:10:12 GMT
ADD file:b85f8b675931991dc4361ad29563c508e8cdd381491f1da64b998d7742f72c42 in / 
# Sat, 28 Jan 2023 05:10:12 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:15:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:16:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ec11bba63863786b2862fe78b2d89ce7f2cf2ab178c9abc17064e250fc6a07b`  
		Last Modified: Wed, 01 Feb 2023 18:22:06 GMT  
		Size: 26.0 MB (26014630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50701e4538cb519cc258f9f917c69bd16c143f281ac369a90c6aba3f40dcff3`  
		Last Modified: Wed, 01 Feb 2023 18:22:04 GMT  
		Size: 6.3 MB (6318048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c474c2328ae2c175dbac9c35c888383f82da2ae100c9197db0e3a1912be9dd3e`  
		Last Modified: Wed, 01 Feb 2023 18:22:03 GMT  
		Size: 3.7 MB (3674786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eabce57ad05a030ae2bc38b37ffdb539eef43109d4503a2b66e82f71391c9bb`  
		Last Modified: Wed, 01 Feb 2023 18:22:20 GMT  
		Size: 40.7 MB (40730894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:a838d98f78f15e4a283ba7ee24e0e7d5944ea6ef8ef6ad8746f48f9529578c52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:112ea54e20cdb539d74c1aea7d6ea6a943707a9ac2040c39de69943b7a436ee1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221416802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec5bb581fc632486d061a5fad946b21eecd24ac60745e89393352da7e836934`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:39:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:40:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:43:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b21d603a94f829dcf240f93489b3359deed997929b46f2bf66146926bd3ef9f`  
		Last Modified: Tue, 31 Jan 2023 18:00:44 GMT  
		Size: 6.6 MB (6617506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b155ce8564683071c961a173c72705932177495f976f405ab77696ac5cd17b75`  
		Last Modified: Tue, 31 Jan 2023 18:00:43 GMT  
		Size: 3.0 MB (3026069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb0ace4785a8addeddef7444ff5ff46d73774811c1192c979da490211bc50fe`  
		Last Modified: Tue, 31 Jan 2023 18:01:01 GMT  
		Size: 45.5 MB (45511626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ef02d81da19db2c47cb556e459a01501941d27afa51e04bac07cd66b41f902`  
		Last Modified: Tue, 31 Jan 2023 18:01:28 GMT  
		Size: 139.6 MB (139550007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bec2c066b06674351fa26f2f2c118cd93d869499d5c199ea9cc9322a81ac1e72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.7 MB (188669200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b22bc5658b828766b7f163910d113d4cbebff818e724f292cf4a3e55cebf274`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:39:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:40:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:43:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c138257d410403a2127c08e269ac8467b8f2001b22a102934861b65b2f49bc1a`  
		Last Modified: Thu, 26 Jan 2023 10:12:17 GMT  
		Size: 21.4 MB (21395113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47096fe89b773c1646429c4d0b72c616d52ad8e417f6b22a7fffacbf9e543330`  
		Last Modified: Wed, 01 Mar 2023 03:12:33 GMT  
		Size: 5.7 MB (5680777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1cbacc1eb0f2444d8fe8e626335b90e377dba26148c5b1ba67d69a9966df71`  
		Last Modified: Wed, 01 Mar 2023 03:12:32 GMT  
		Size: 2.6 MB (2586738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a752d641cb559708d7e030aae9c70190dbf469ce25759b21c2c34db03cca6ac`  
		Last Modified: Wed, 01 Mar 2023 03:12:52 GMT  
		Size: 40.7 MB (40714103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c6952ec819332449a056dd110221540c0eaa7c31291b042cf53e83555dbe40`  
		Last Modified: Wed, 01 Mar 2023 03:13:20 GMT  
		Size: 118.3 MB (118292469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:298975d24d02a6a27d8263539396799ce83b4a046332e9fe63ec881252ce8b85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (206001361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e8924e0b5645090142a50844e7727c9105cfe493c3b778a52c744e07c792aea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:12:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:12:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:12:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:15:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c3db86e75ada5398a2d9a556625e3e0a4b73c36ab79cf21ccd1ffd35dd43fc`  
		Last Modified: Tue, 31 Jan 2023 18:33:13 GMT  
		Size: 6.1 MB (6055914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cd619a1ebf49880ce75b505030f48c0ab5b4904c5418bbc0145052802eaa63`  
		Last Modified: Tue, 31 Jan 2023 18:33:12 GMT  
		Size: 2.8 MB (2790620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6ed5bf2278606c14e4380d7510535f5bdad7a4e6b5bd6dddff29b256521546`  
		Last Modified: Tue, 31 Jan 2023 18:33:26 GMT  
		Size: 43.3 MB (43313944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ea3f5323e959f3e723895c9550a68aa58401d733f4c29eca854ca8251fb00e`  
		Last Modified: Tue, 31 Jan 2023 18:33:48 GMT  
		Size: 130.1 MB (130105353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a113ee21f105490a147fb85ab0e68054570c5079969b6ddd3731a9db03fab1e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.6 MB (217639452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d20118b6fa4a93abb79434f72311d8fc10725e107f4bb7b89b55504f388af0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:01 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:03 GMT
ADD file:b9b814a7d1e7611a2c531fac3419a48c733c622470d3f275ce29f9ba8764eaeb in / 
# Thu, 26 Jan 2023 10:03:04 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:16:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:16:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:17:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:20:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57a4d5aed2cd4a1f596f693a8fe5e135bd66dbf401ec169b1848d2316bdcfb2c`  
		Last Modified: Thu, 26 Jan 2023 10:12:23 GMT  
		Size: 26.1 MB (26096513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7a01875a8f61110b8a3987b128629884aa645fef18557175a3c73a79ecda62`  
		Last Modified: Wed, 01 Mar 2023 02:27:41 GMT  
		Size: 6.9 MB (6907847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9185b0869254fbcd22a9fab4d7b047d37171dc5b322e61abf872fcc068ecf472`  
		Last Modified: Wed, 01 Mar 2023 02:27:40 GMT  
		Size: 3.3 MB (3255765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79adfdfb2c964ed95f76337267ac66d2871db2f52647fd6f502bca4a71e16a92`  
		Last Modified: Wed, 01 Mar 2023 02:28:00 GMT  
		Size: 47.1 MB (47097285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab3618597de62189ed2023f7cbac7de859932f1d67c09ddb53229e02c8e04b8`  
		Last Modified: Wed, 01 Mar 2023 02:28:37 GMT  
		Size: 134.3 MB (134282042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:31341a141691d55d1f2cca4b84192f7e18716d953c51ddda04a8ee7bf1a65b08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246429217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0f820148ce5933d66e53b71b484a8a2897804ccd2f60c2e2fda8f33a574d90a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:47 GMT
ADD file:108aadd723beb46031bfaca610c036aea506955578347dda4a01cfb0c6bdc135 in / 
# Thu, 26 Jan 2023 09:55:48 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:41:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:42:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:46:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15579125cdf95166fecb7637769c3c9eb2551401759fb21f44848947ead59cbd`  
		Last Modified: Tue, 31 Jan 2023 18:13:22 GMT  
		Size: 30.4 MB (30442586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fea2fabde99e916cabf483638fbf3a31420ac919854738215aa0a52bf39fa`  
		Last Modified: Tue, 31 Jan 2023 18:13:16 GMT  
		Size: 7.0 MB (7035605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428b8a67c5ee9117982087fd7c1be5b763a8286ea404e24144bc6b0042fff348`  
		Last Modified: Tue, 31 Jan 2023 18:13:15 GMT  
		Size: 3.7 MB (3740488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491ab9254ea85bdf063c540c3096b71d4039f2039cf028e624dca83dec8a051f`  
		Last Modified: Tue, 31 Jan 2023 18:13:47 GMT  
		Size: 53.7 MB (53737946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758dd9eee269cf33fbdde212adb77691074569f92a1d01ba62bac008278f4857`  
		Last Modified: Tue, 31 Jan 2023 18:14:35 GMT  
		Size: 151.5 MB (151472592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4f6241dbfc40151e66aea2c355461bbef78034983413e2b41b6832aeb22c35e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205756217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff50765f6a19cc4d538eb4fac2111f73e78e74d036b73805fb2ee671ce87354`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:41 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:43 GMT
ADD file:04d4137c9183cee18560fc26a092e288ff403f3dde266237eab245bd38eb9b3a in / 
# Thu, 26 Jan 2023 09:55:43 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:35:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:38:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4727db5881c26ec0d79df6d172cfc50624c09ca7869b8146052e0692734d2cac`  
		Last Modified: Tue, 31 Jan 2023 17:53:57 GMT  
		Size: 25.4 MB (25371457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e060d5ddd88a52d0a10b103bf4210855c9cc2daac45756f960fd90365af6542`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 6.3 MB (6308650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4883942b852e1bd875f58749e4c99070639db9ac02867dfd13770796b06c8687`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 3.0 MB (2976626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a824cce0d3d1e891d7b4b44e056c1b33ba9f719ad78192a3664800de0d266cd`  
		Last Modified: Tue, 31 Jan 2023 17:54:09 GMT  
		Size: 45.0 MB (45038632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d798a29e5e355ed223ecaefa81f44f8f602cd06432fcdb23e38a81ab93a7137a`  
		Last Modified: Tue, 31 Jan 2023 17:54:36 GMT  
		Size: 126.1 MB (126060852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:686d709db13d50f30787c0276226d7cdedcf95628c7c106691f693e66b7f5fa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:eefb4a7c8e274ca65671f877f62a858f8fd0844f35fd6d8cab3be4ab9381518a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36355169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09e8e203a6674cdf500bddc5275d68fb9a2bcc4fb09aef4179d4cb0031dd23f2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:39:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b21d603a94f829dcf240f93489b3359deed997929b46f2bf66146926bd3ef9f`  
		Last Modified: Tue, 31 Jan 2023 18:00:44 GMT  
		Size: 6.6 MB (6617506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b155ce8564683071c961a173c72705932177495f976f405ab77696ac5cd17b75`  
		Last Modified: Tue, 31 Jan 2023 18:00:43 GMT  
		Size: 3.0 MB (3026069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:87c3947ab27b7395c340fdb40be0b232cf4881d24ed4e45a3d4bf5f6e3daa1cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29662628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86602b4d6ae57581dc9d6a308905bf10c1ef8a8b8030b5432cfcae3553ac031b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:39:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c138257d410403a2127c08e269ac8467b8f2001b22a102934861b65b2f49bc1a`  
		Last Modified: Thu, 26 Jan 2023 10:12:17 GMT  
		Size: 21.4 MB (21395113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47096fe89b773c1646429c4d0b72c616d52ad8e417f6b22a7fffacbf9e543330`  
		Last Modified: Wed, 01 Mar 2023 03:12:33 GMT  
		Size: 5.7 MB (5680777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1cbacc1eb0f2444d8fe8e626335b90e377dba26148c5b1ba67d69a9966df71`  
		Last Modified: Wed, 01 Mar 2023 03:12:32 GMT  
		Size: 2.6 MB (2586738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3ca6d0747171417678ed64f5386ecb852fcde4e72a1461446a931f6a09ed6846
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32582064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e54f779279d1503cb962c0a72b798187b208e7b91f6bfa1507768b86cbefd709`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:12:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:12:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c3db86e75ada5398a2d9a556625e3e0a4b73c36ab79cf21ccd1ffd35dd43fc`  
		Last Modified: Tue, 31 Jan 2023 18:33:13 GMT  
		Size: 6.1 MB (6055914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cd619a1ebf49880ce75b505030f48c0ab5b4904c5418bbc0145052802eaa63`  
		Last Modified: Tue, 31 Jan 2023 18:33:12 GMT  
		Size: 2.8 MB (2790620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9c66348aba08cf56330bef73e31d204b066c48c9233586ead80480b01725c030
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbd5750801a877aad4b07a19fbca8b18b3267b49caf30dd0b5bfd0fcba07bdf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:01 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:03 GMT
ADD file:b9b814a7d1e7611a2c531fac3419a48c733c622470d3f275ce29f9ba8764eaeb in / 
# Thu, 26 Jan 2023 10:03:04 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:16:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:16:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:57a4d5aed2cd4a1f596f693a8fe5e135bd66dbf401ec169b1848d2316bdcfb2c`  
		Last Modified: Thu, 26 Jan 2023 10:12:23 GMT  
		Size: 26.1 MB (26096513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7a01875a8f61110b8a3987b128629884aa645fef18557175a3c73a79ecda62`  
		Last Modified: Wed, 01 Mar 2023 02:27:41 GMT  
		Size: 6.9 MB (6907847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9185b0869254fbcd22a9fab4d7b047d37171dc5b322e61abf872fcc068ecf472`  
		Last Modified: Wed, 01 Mar 2023 02:27:40 GMT  
		Size: 3.3 MB (3255765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9f86ff85ce09457dbf0f1f65da193c6aeff8cfc85fbb30dc0a6162051eeeacf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41218679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1c204ad4d256ee762cc2bb63546a154b975ead673362bb7cc0c6779857e4d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:47 GMT
ADD file:108aadd723beb46031bfaca610c036aea506955578347dda4a01cfb0c6bdc135 in / 
# Thu, 26 Jan 2023 09:55:48 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:41:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:15579125cdf95166fecb7637769c3c9eb2551401759fb21f44848947ead59cbd`  
		Last Modified: Tue, 31 Jan 2023 18:13:22 GMT  
		Size: 30.4 MB (30442586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fea2fabde99e916cabf483638fbf3a31420ac919854738215aa0a52bf39fa`  
		Last Modified: Tue, 31 Jan 2023 18:13:16 GMT  
		Size: 7.0 MB (7035605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428b8a67c5ee9117982087fd7c1be5b763a8286ea404e24144bc6b0042fff348`  
		Last Modified: Tue, 31 Jan 2023 18:13:15 GMT  
		Size: 3.7 MB (3740488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c86ef5326c34545c4f4f53fea242951a4457f014933db0817669765075d68c87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34656733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8846013a5b74eb1fd3072a9091d0e1ad91f04a48853e4d84d2c77d240414725`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:41 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:43 GMT
ADD file:04d4137c9183cee18560fc26a092e288ff403f3dde266237eab245bd38eb9b3a in / 
# Thu, 26 Jan 2023 09:55:43 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:35:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4727db5881c26ec0d79df6d172cfc50624c09ca7869b8146052e0692734d2cac`  
		Last Modified: Tue, 31 Jan 2023 17:53:57 GMT  
		Size: 25.4 MB (25371457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e060d5ddd88a52d0a10b103bf4210855c9cc2daac45756f960fd90365af6542`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 6.3 MB (6308650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4883942b852e1bd875f58749e4c99070639db9ac02867dfd13770796b06c8687`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 3.0 MB (2976626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:ba36fe023887a6023026eae58d6bba3447a045a77a4261c1a1f6db373cedac91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e7df5351980a3dfe768ac04e0c53fa513d73027ea35485119db202f58ebc8a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81866795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc13147b59defbe2f266c1e16966187b3351b15e4260038e87564d6134d946c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:39:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:40:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b21d603a94f829dcf240f93489b3359deed997929b46f2bf66146926bd3ef9f`  
		Last Modified: Tue, 31 Jan 2023 18:00:44 GMT  
		Size: 6.6 MB (6617506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b155ce8564683071c961a173c72705932177495f976f405ab77696ac5cd17b75`  
		Last Modified: Tue, 31 Jan 2023 18:00:43 GMT  
		Size: 3.0 MB (3026069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb0ace4785a8addeddef7444ff5ff46d73774811c1192c979da490211bc50fe`  
		Last Modified: Tue, 31 Jan 2023 18:01:01 GMT  
		Size: 45.5 MB (45511626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2acd0deb7308e5597b2b9d3b593ae7ea6e8f7fc346ce2d08ebddb9fbe54baad9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70376731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9373357a8aec9ae1e9d9f45f397ff6c4a97a3beec687935474c737e6d687df`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:39:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:40:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c138257d410403a2127c08e269ac8467b8f2001b22a102934861b65b2f49bc1a`  
		Last Modified: Thu, 26 Jan 2023 10:12:17 GMT  
		Size: 21.4 MB (21395113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47096fe89b773c1646429c4d0b72c616d52ad8e417f6b22a7fffacbf9e543330`  
		Last Modified: Wed, 01 Mar 2023 03:12:33 GMT  
		Size: 5.7 MB (5680777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1cbacc1eb0f2444d8fe8e626335b90e377dba26148c5b1ba67d69a9966df71`  
		Last Modified: Wed, 01 Mar 2023 03:12:32 GMT  
		Size: 2.6 MB (2586738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a752d641cb559708d7e030aae9c70190dbf469ce25759b21c2c34db03cca6ac`  
		Last Modified: Wed, 01 Mar 2023 03:12:52 GMT  
		Size: 40.7 MB (40714103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0f7454305ad71cc1618ddc501c963f107e9e1ca383a9dc2e1f1d31db83de8952
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75896008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c594dd26e7b2f1c31896b626cffe79c629fcfd41f75e722dd4626f2f4088e64e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:12:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:12:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:12:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c3db86e75ada5398a2d9a556625e3e0a4b73c36ab79cf21ccd1ffd35dd43fc`  
		Last Modified: Tue, 31 Jan 2023 18:33:13 GMT  
		Size: 6.1 MB (6055914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cd619a1ebf49880ce75b505030f48c0ab5b4904c5418bbc0145052802eaa63`  
		Last Modified: Tue, 31 Jan 2023 18:33:12 GMT  
		Size: 2.8 MB (2790620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6ed5bf2278606c14e4380d7510535f5bdad7a4e6b5bd6dddff29b256521546`  
		Last Modified: Tue, 31 Jan 2023 18:33:26 GMT  
		Size: 43.3 MB (43313944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8ca4f8a2693cdd7aff210955c3bbc8be8eef544578cac7e64a5908ab4a5aee1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83357410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4862a954bb62d0211b2e1de96a09b28b9c636bad9ecc51c55eda533a9b12b23`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:01 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:03 GMT
ADD file:b9b814a7d1e7611a2c531fac3419a48c733c622470d3f275ce29f9ba8764eaeb in / 
# Thu, 26 Jan 2023 10:03:04 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:16:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:16:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:17:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57a4d5aed2cd4a1f596f693a8fe5e135bd66dbf401ec169b1848d2316bdcfb2c`  
		Last Modified: Thu, 26 Jan 2023 10:12:23 GMT  
		Size: 26.1 MB (26096513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7a01875a8f61110b8a3987b128629884aa645fef18557175a3c73a79ecda62`  
		Last Modified: Wed, 01 Mar 2023 02:27:41 GMT  
		Size: 6.9 MB (6907847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9185b0869254fbcd22a9fab4d7b047d37171dc5b322e61abf872fcc068ecf472`  
		Last Modified: Wed, 01 Mar 2023 02:27:40 GMT  
		Size: 3.3 MB (3255765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79adfdfb2c964ed95f76337267ac66d2871db2f52647fd6f502bca4a71e16a92`  
		Last Modified: Wed, 01 Mar 2023 02:28:00 GMT  
		Size: 47.1 MB (47097285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:98b56b01409cca65eb0051a74814eca3788d5a98d541104a5653f00cd973c18d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94956625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ea247b997209a79cca6c45dfbc04979886790d6040979527e616c8e89d7185`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:47 GMT
ADD file:108aadd723beb46031bfaca610c036aea506955578347dda4a01cfb0c6bdc135 in / 
# Thu, 26 Jan 2023 09:55:48 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:41:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:42:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15579125cdf95166fecb7637769c3c9eb2551401759fb21f44848947ead59cbd`  
		Last Modified: Tue, 31 Jan 2023 18:13:22 GMT  
		Size: 30.4 MB (30442586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fea2fabde99e916cabf483638fbf3a31420ac919854738215aa0a52bf39fa`  
		Last Modified: Tue, 31 Jan 2023 18:13:16 GMT  
		Size: 7.0 MB (7035605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428b8a67c5ee9117982087fd7c1be5b763a8286ea404e24144bc6b0042fff348`  
		Last Modified: Tue, 31 Jan 2023 18:13:15 GMT  
		Size: 3.7 MB (3740488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491ab9254ea85bdf063c540c3096b71d4039f2039cf028e624dca83dec8a051f`  
		Last Modified: Tue, 31 Jan 2023 18:13:47 GMT  
		Size: 53.7 MB (53737946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ed5d0d1582ec32919d5650c6af855db2fc9de89b856a8e10fc4d226e285d1449
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79695365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737e17d3b58cd146e26376e8cc717a07041a325ff66cc553302b964fe2f1e252`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:41 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:43 GMT
ADD file:04d4137c9183cee18560fc26a092e288ff403f3dde266237eab245bd38eb9b3a in / 
# Thu, 26 Jan 2023 09:55:43 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:35:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:36:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4727db5881c26ec0d79df6d172cfc50624c09ca7869b8146052e0692734d2cac`  
		Last Modified: Tue, 31 Jan 2023 17:53:57 GMT  
		Size: 25.4 MB (25371457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e060d5ddd88a52d0a10b103bf4210855c9cc2daac45756f960fd90365af6542`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 6.3 MB (6308650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4883942b852e1bd875f58749e4c99070639db9ac02867dfd13770796b06c8687`  
		Last Modified: Tue, 31 Jan 2023 17:53:54 GMT  
		Size: 3.0 MB (2976626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a824cce0d3d1e891d7b4b44e056c1b33ba9f719ad78192a3664800de0d266cd`  
		Last Modified: Tue, 31 Jan 2023 17:54:09 GMT  
		Size: 45.0 MB (45038632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:6028d65928c1f2cc6fd1d75a1b33eed8a49da8b88d92a0d871a72b89128ca400
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bookworm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:195681bdeac6045bdaae7f1c8a3d555ef169b6200ef761cde689fd8e5ebc1544
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.7 MB (344673834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4434dc6ee1bad5f222d7d8e7ce697a1f5dc4fbc07f8f595bec3f1f7d3697ec47`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:21 GMT
ADD file:74b4e0fbcb9cb38344c32a0512a72d8179f885de4b7bb127215f8d96a6262664 in / 
# Wed, 01 Mar 2023 04:09:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:40:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d915a4248d2913bb8451eba978ac348a983990eca9186543367f5f44900e0fb`  
		Last Modified: Wed, 01 Mar 2023 04:13:25 GMT  
		Size: 49.2 MB (49237273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012774ea2ca6d41295cf7bc05a82ac4aa9183dd2ce4f4c0584b549d922ef6b2e`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 9.0 MB (9049510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871c0f2b6b6518e6675004eb4ccd8a8d77105f4f1d83d8f0d0168b16f544ffbe`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 11.4 MB (11405791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df7f0c3bf5351a2fa63ae6776d5565929b9afb539c689cadd1e415b1751f478`  
		Last Modified: Wed, 01 Mar 2023 04:49:31 GMT  
		Size: 64.1 MB (64094287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7b30ee362037144052a76832c9fb5838292f13214d0adcce12770da6ebef28`  
		Last Modified: Wed, 01 Mar 2023 04:50:05 GMT  
		Size: 210.9 MB (210886973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6020af7ec13e1b5c9b5a69273fee42ba9794d8fbebc5b1cd02cf1ee36c7fc9fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.4 MB (313404899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a30408ef722d243b15667eb01103cf5a198e0540e6c3dabf09a3068a7bf151`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:24 GMT
ADD file:1685939a153ab7a7aa03035565c60e99663abd3a416ef0d00bddaf24e0ae6f08 in / 
# Wed, 01 Mar 2023 01:48:25 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:15:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:17:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f7516928cdf57280d137bb31220dd9f0b6ca54e290189b42a68ab64d0d2065b7`  
		Last Modified: Wed, 01 Mar 2023 01:51:43 GMT  
		Size: 48.1 MB (48072838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402a03a1c745fc42a93ed0082abf13d52e0c961da496b7b2d7d9a60a1d8031f`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 8.5 MB (8496389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea6f1f01cbcb26c4e22bf2c443b3515e57d9267d84661daeb7ae809ff62ff82`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 11.1 MB (11051495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db38c030ddb0562da5b6a4ed2e4333299c295c785959c19faae6aecfee04f841`  
		Last Modified: Wed, 01 Mar 2023 02:24:07 GMT  
		Size: 61.5 MB (61520999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca85168741ee98a96b0dd356f399b344b82fee50e8e9efd731252ebe921ef5b`  
		Last Modified: Wed, 01 Mar 2023 02:24:43 GMT  
		Size: 184.3 MB (184263178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7bf5be439e3fda124e262e33b08707f2ca5141674cde6b7714cd35627da86d16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.8 MB (298825417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6e75b174f39ba61336f8b77fb439838425edd2ef79572e33b69628b8cff7060`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:26 GMT
ADD file:9f8ce83cf3e75c63cb351ec688378ffe29d7105ff8e8892b3cef95aeacbf6779 in / 
# Wed, 01 Mar 2023 01:57:27 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:28:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:29:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:31:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c5d14f15cd67359c9f8d5dbc636ce6ffee972aa4acbeb663e40e865b0dd7dee`  
		Last Modified: Wed, 01 Mar 2023 02:01:54 GMT  
		Size: 45.8 MB (45843301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925df4d36e5e8049cacb403582ac8832aed842417020be560ab0398e08c8fb67`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 8.1 MB (8140837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5921afe59294ea6e26c9a0c8c143bce276da4ba83ef2f7194b96d034a2b463d`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 10.7 MB (10687660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daffa30bd41618c0f8d8bc932ac6b2e541af6a12c3462963570690c046fb0eb`  
		Last Modified: Wed, 01 Mar 2023 03:08:25 GMT  
		Size: 59.2 MB (59228783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50887d27d71d122cc7300c13322d74bde98f553f7cf135b1505f230f518673f`  
		Last Modified: Wed, 01 Mar 2023 03:09:01 GMT  
		Size: 174.9 MB (174924836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d7ffe8d49a7b80dcc5663e150f752387a766b3b53160652991c0ab26d07643fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335767410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18c2cda0cb0dac04945795df83d91094f7b8f7a976279c2b80ccdd1a54abcd98`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:13 GMT
ADD file:5b81699b80066f9e3bc967bdf130a67f54ebe15cd80df6c952262d6132b1cabf in / 
# Wed, 01 Mar 2023 02:20:14 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:46:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:47:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:48:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf639a903cc04a00c81ac77b3b9f9a79644c51b7f515895fd60403c20ff34a80`  
		Last Modified: Wed, 01 Mar 2023 02:23:22 GMT  
		Size: 49.3 MB (49273990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42632d5ac93ac504d393018f5e0f56f02bedd9cd2df6e1d91da9fc0ef4806d9b`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 8.9 MB (8882130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c0a0685e10806d6ca5aac08337a76d9fd6a47f16f665f5d3a2e692eabfeb3f`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 11.4 MB (11371530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1ccc2a9c1e986768a01b08e1009a75262c8bac308f9c9d414685034ce162c1`  
		Last Modified: Wed, 01 Mar 2023 02:55:40 GMT  
		Size: 63.9 MB (63942296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6498018d1c1322fabda196170f7912e9dcca825fed9a4aec837be082b1b225fb`  
		Last Modified: Wed, 01 Mar 2023 02:56:09 GMT  
		Size: 202.3 MB (202297464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bfe43663f0657294ca025418f275e8e909e49dc6114c520c8c1b8c0f2bf064d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.1 MB (347082902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f9b45267606b6b6a34d9882904bfc4bd4fbaa171ab797bf69b5fd7109e2efbb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:38:40 GMT
ADD file:0ccdbb7b1f104c23abcf77c506eed771d5759d210c2284a95f85e558405a5390 in / 
# Wed, 01 Mar 2023 01:38:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:05:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:05:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b5ba6d7d02dd42cc6291ae5b4e129956756f664662a78db71f320107a1b6d189`  
		Last Modified: Wed, 01 Mar 2023 01:43:30 GMT  
		Size: 50.3 MB (50273396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f35c12f0528f81569a1c99e040f4d3527ee4391aa4079d740a4c6638bcece0`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 9.2 MB (9230996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319f35836381f914f3bbf4d55b955e9cf90a83165b64e829c72b52051b5e5c5`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 11.8 MB (11808790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a8ff813204e629160f019ffdb45960b87b39f586133418d3fd5f36323e5f03`  
		Last Modified: Wed, 01 Mar 2023 02:22:30 GMT  
		Size: 65.9 MB (65937993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8466c42e65a0d855e2465ff126267c143a76b83ccd4d4770213c0472a28557ae`  
		Last Modified: Wed, 01 Mar 2023 02:23:17 GMT  
		Size: 209.8 MB (209831727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c57a7f1ec7adfe8459654df4f071d8f4d79ec1a0316240f76409fc967eb537ba
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321227952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5849000d7db598292b11707a555bbb2b5de9bbd7035008cf9f52e0e35e9d58f0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:43:09 GMT
ADD file:bff5ae942e6561f2afffbbd0267d57706f7fdd71ebe43c64b369b20940d55f00 in / 
# Thu, 09 Feb 2023 02:43:14 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:31:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:32:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:33:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:39:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aa6addfe979ac43879ea9517851622f7a6c1516568fbd6a0c101c3b86cc1163`  
		Last Modified: Thu, 09 Feb 2023 02:51:51 GMT  
		Size: 49.1 MB (49063446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6db93799880bf6f9525fc696324e0d450fd37ebbb37d356955a9057236da38`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 8.4 MB (8399010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b19fed47eb69b023968097b12ef67cad0d7e15a03675cc16e3efc9b67a44e4`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 11.1 MB (11105521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7152f2a237e2d177c5dc02d27a4b1e0433902b36280eb92369c2a9e5620678e`  
		Last Modified: Thu, 09 Feb 2023 07:57:24 GMT  
		Size: 63.3 MB (63307246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7ff536332669177f30e959f391f586eaf9b5c716f81f9a50b31c0c1ce869d6`  
		Last Modified: Thu, 09 Feb 2023 07:59:38 GMT  
		Size: 189.4 MB (189352729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d5e1db6aed979d645af6fee7361c5a23b34c1d43584bf4db444cc8bfde6221a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.5 MB (358527778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe7a5c69cddd5f8e4e1b828ca19c143392e37b1cd9c29f6b9ae04774856707e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:46:00 GMT
ADD file:311d9174b941eeaaa2babe3a94b035ab7c3880d5908d630bdec420f42eff6a06 in / 
# Wed, 01 Mar 2023 04:46:05 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:18:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:18:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:20:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:24:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6b61b4a96c9a944bd44d67cc885cdb2ef5f9aa35a0a94dba6ea2b6372ad27e48`  
		Last Modified: Wed, 01 Mar 2023 04:52:26 GMT  
		Size: 53.3 MB (53250230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a057e1f93c20f3bf648ce49e3455619f0854aef331a7d297c7425e435adfcb8`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 9.6 MB (9631581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb4683b31216d30e252186c2c0cb6f06f69d737321cb3d95c8f1036adca0bea`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 12.2 MB (12168325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18e9322efa86ed752abe3ce6c6627d95fb158f9e6fc57b15a1dd5c4eeac07ae`  
		Last Modified: Wed, 01 Mar 2023 05:38:09 GMT  
		Size: 69.5 MB (69538650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0dfbe78692a54c80a5b039ccab3594a7e5bd520477c34ff0871e776ced27bb`  
		Last Modified: Wed, 01 Mar 2023 05:39:11 GMT  
		Size: 213.9 MB (213938992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2746edcd036ffa0e80571e197771eb53a1e7d407da3edb91126e6256b418c611
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313638662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d1cd40898cf919229eebdad2f4a408e5b37c0c37062ab7763759c8d26d4ae52`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:49:37 GMT
ADD file:55baf50ca3524103dfcb38a8784744d482a5cdb19f66a7baa92d44dc18483a58 in / 
# Wed, 01 Mar 2023 02:49:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:12:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e95e47ef2a5cde1145fe4af2db22dbfe40c09cf83dbb9ff00d400d23e6dd5331`  
		Last Modified: Wed, 01 Mar 2023 02:53:58 GMT  
		Size: 47.6 MB (47608102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf204e7b8be3c288518bf65a248e94d7d77b56c235d30b3eb93058f663337226`  
		Last Modified: Wed, 01 Mar 2023 03:21:19 GMT  
		Size: 8.7 MB (8684339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca66d3959e328f7d96d65cb0b1a3f79c9c7f949a2fefecdadb692344f6e8a5b`  
		Last Modified: Wed, 01 Mar 2023 03:21:18 GMT  
		Size: 11.3 MB (11268858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb5857b88499838945e97d7c6a6c6ebe9e8cedf2f9e53fd3969022b50bafb3c`  
		Last Modified: Wed, 01 Mar 2023 03:21:34 GMT  
		Size: 63.1 MB (63088618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7a497c30bac5956b1d898cc4c280377487b7b0abb58817eed64f480bb4fb69`  
		Last Modified: Wed, 01 Mar 2023 03:22:03 GMT  
		Size: 183.0 MB (182988745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:c8f091cd0bdf8be224eb2fe67d5861723a681b2a0aead26099000373f5bd2b9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bookworm-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d4b35a63544657e87fe7761075ad7fc9666a5d864314a5d931be9bd6c7f9ef54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69692574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3d26fafdceaae720d412163f42c2d209fac53ec665bc89ce3d048ebcbbe1f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:21 GMT
ADD file:74b4e0fbcb9cb38344c32a0512a72d8179f885de4b7bb127215f8d96a6262664 in / 
# Wed, 01 Mar 2023 04:09:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:40:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9d915a4248d2913bb8451eba978ac348a983990eca9186543367f5f44900e0fb`  
		Last Modified: Wed, 01 Mar 2023 04:13:25 GMT  
		Size: 49.2 MB (49237273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012774ea2ca6d41295cf7bc05a82ac4aa9183dd2ce4f4c0584b549d922ef6b2e`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 9.0 MB (9049510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871c0f2b6b6518e6675004eb4ccd8a8d77105f4f1d83d8f0d0168b16f544ffbe`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 11.4 MB (11405791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:62c8e4b2d3cb76df9cd0da0c61644cfd48542f5dcab0f8876ac5006f197b466b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67620722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302c483085eabc43b0bc26a0ec3388ba8bd6e850b6aaf90bee3067eb1b06e29d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:24 GMT
ADD file:1685939a153ab7a7aa03035565c60e99663abd3a416ef0d00bddaf24e0ae6f08 in / 
# Wed, 01 Mar 2023 01:48:25 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f7516928cdf57280d137bb31220dd9f0b6ca54e290189b42a68ab64d0d2065b7`  
		Last Modified: Wed, 01 Mar 2023 01:51:43 GMT  
		Size: 48.1 MB (48072838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402a03a1c745fc42a93ed0082abf13d52e0c961da496b7b2d7d9a60a1d8031f`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 8.5 MB (8496389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea6f1f01cbcb26c4e22bf2c443b3515e57d9267d84661daeb7ae809ff62ff82`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 11.1 MB (11051495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:89d5b8cad9b7628091dc315c80ac73032be23c33ffc20a54daa4494c2b869d0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64671798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4424c860db17396c58ff3e4f5cc348d934583867019f1491602086ce7f289e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:26 GMT
ADD file:9f8ce83cf3e75c63cb351ec688378ffe29d7105ff8e8892b3cef95aeacbf6779 in / 
# Wed, 01 Mar 2023 01:57:27 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:28:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4c5d14f15cd67359c9f8d5dbc636ce6ffee972aa4acbeb663e40e865b0dd7dee`  
		Last Modified: Wed, 01 Mar 2023 02:01:54 GMT  
		Size: 45.8 MB (45843301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925df4d36e5e8049cacb403582ac8832aed842417020be560ab0398e08c8fb67`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 8.1 MB (8140837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5921afe59294ea6e26c9a0c8c143bce276da4ba83ef2f7194b96d034a2b463d`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 10.7 MB (10687660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:de24f24c37e458d6b286a7c11bfa15cdcbc2c98af24cb1b5d4ca4d41fe220b93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69527650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1935824d13726e2507f35f1e2b012cdc815e6923d82f8ef0dad82ae11e50138`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:13 GMT
ADD file:5b81699b80066f9e3bc967bdf130a67f54ebe15cd80df6c952262d6132b1cabf in / 
# Wed, 01 Mar 2023 02:20:14 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:46:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cf639a903cc04a00c81ac77b3b9f9a79644c51b7f515895fd60403c20ff34a80`  
		Last Modified: Wed, 01 Mar 2023 02:23:22 GMT  
		Size: 49.3 MB (49273990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42632d5ac93ac504d393018f5e0f56f02bedd9cd2df6e1d91da9fc0ef4806d9b`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 8.9 MB (8882130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c0a0685e10806d6ca5aac08337a76d9fd6a47f16f665f5d3a2e692eabfeb3f`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 11.4 MB (11371530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0cd5d6206f9f4c2d947dad0bfb51b68944ebe17cf3baf558cc906cb8a3467117
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71313182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78a3dfaf671eb3aee58f8b6339b0f8dc5fcc24c896f58aded93920c474c13e83`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:38:40 GMT
ADD file:0ccdbb7b1f104c23abcf77c506eed771d5759d210c2284a95f85e558405a5390 in / 
# Wed, 01 Mar 2023 01:38:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:05:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b5ba6d7d02dd42cc6291ae5b4e129956756f664662a78db71f320107a1b6d189`  
		Last Modified: Wed, 01 Mar 2023 01:43:30 GMT  
		Size: 50.3 MB (50273396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f35c12f0528f81569a1c99e040f4d3527ee4391aa4079d740a4c6638bcece0`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 9.2 MB (9230996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319f35836381f914f3bbf4d55b955e9cf90a83165b64e829c72b52051b5e5c5`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 11.8 MB (11808790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2fbb3255f217e7530d462b4aacaaa94d13346677c94e5283617b6f03c701cf36
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68567977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:debaa28c7b7c6c9f25d29679aa12d4fcce59bc201a8da4940981fd15ac5ec342`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:43:09 GMT
ADD file:bff5ae942e6561f2afffbbd0267d57706f7fdd71ebe43c64b369b20940d55f00 in / 
# Thu, 09 Feb 2023 02:43:14 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:31:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:32:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9aa6addfe979ac43879ea9517851622f7a6c1516568fbd6a0c101c3b86cc1163`  
		Last Modified: Thu, 09 Feb 2023 02:51:51 GMT  
		Size: 49.1 MB (49063446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6db93799880bf6f9525fc696324e0d450fd37ebbb37d356955a9057236da38`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 8.4 MB (8399010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b19fed47eb69b023968097b12ef67cad0d7e15a03675cc16e3efc9b67a44e4`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 11.1 MB (11105521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:36f29f426e14bbe0de3f0f8ec7ca53855abbdbc9166223f63f386475adb95a3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75050136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca0a733a8ebc11612b7086f5d280d94b7bb2a33ff7f588e472fb573dca062ba0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:46:00 GMT
ADD file:311d9174b941eeaaa2babe3a94b035ab7c3880d5908d630bdec420f42eff6a06 in / 
# Wed, 01 Mar 2023 04:46:05 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:18:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:18:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6b61b4a96c9a944bd44d67cc885cdb2ef5f9aa35a0a94dba6ea2b6372ad27e48`  
		Last Modified: Wed, 01 Mar 2023 04:52:26 GMT  
		Size: 53.3 MB (53250230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a057e1f93c20f3bf648ce49e3455619f0854aef331a7d297c7425e435adfcb8`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 9.6 MB (9631581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb4683b31216d30e252186c2c0cb6f06f69d737321cb3d95c8f1036adca0bea`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 12.2 MB (12168325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f2a5b2e26281c3af1970a2678213fa7f844b2177a0acf92329b9ba345095af29
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67561299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be9d847d83a7f68910f5e39bea22c25f248156368cdfc6bb475d02073299fdc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:49:37 GMT
ADD file:55baf50ca3524103dfcb38a8784744d482a5cdb19f66a7baa92d44dc18483a58 in / 
# Wed, 01 Mar 2023 02:49:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:12:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e95e47ef2a5cde1145fe4af2db22dbfe40c09cf83dbb9ff00d400d23e6dd5331`  
		Last Modified: Wed, 01 Mar 2023 02:53:58 GMT  
		Size: 47.6 MB (47608102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf204e7b8be3c288518bf65a248e94d7d77b56c235d30b3eb93058f663337226`  
		Last Modified: Wed, 01 Mar 2023 03:21:19 GMT  
		Size: 8.7 MB (8684339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca66d3959e328f7d96d65cb0b1a3f79c9c7f949a2fefecdadb692344f6e8a5b`  
		Last Modified: Wed, 01 Mar 2023 03:21:18 GMT  
		Size: 11.3 MB (11268858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:6010adfdd68330d5cc75103f4204b81cbd0975c60b82d835e0bf7660febf6864
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bookworm-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7672703ae082615e986385b91c9fa35429dde626233955b38d57cd672e8220e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133786861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da1325778cc479069b68fd4bbf41083893a5ce9810f4735b36ddb24809bbcdcd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:21 GMT
ADD file:74b4e0fbcb9cb38344c32a0512a72d8179f885de4b7bb127215f8d96a6262664 in / 
# Wed, 01 Mar 2023 04:09:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:40:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d915a4248d2913bb8451eba978ac348a983990eca9186543367f5f44900e0fb`  
		Last Modified: Wed, 01 Mar 2023 04:13:25 GMT  
		Size: 49.2 MB (49237273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012774ea2ca6d41295cf7bc05a82ac4aa9183dd2ce4f4c0584b549d922ef6b2e`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 9.0 MB (9049510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871c0f2b6b6518e6675004eb4ccd8a8d77105f4f1d83d8f0d0168b16f544ffbe`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 11.4 MB (11405791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df7f0c3bf5351a2fa63ae6776d5565929b9afb539c689cadd1e415b1751f478`  
		Last Modified: Wed, 01 Mar 2023 04:49:31 GMT  
		Size: 64.1 MB (64094287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e368a980ce07d0d05c407f5f83fd7eaa214a94ab89a68fd65bcc72113d126c75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129141721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f1ccaedc02174ef64b93a8f0f326ec4ffec1458f1c54768a5da3d2e53c616d2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:24 GMT
ADD file:1685939a153ab7a7aa03035565c60e99663abd3a416ef0d00bddaf24e0ae6f08 in / 
# Wed, 01 Mar 2023 01:48:25 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:15:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f7516928cdf57280d137bb31220dd9f0b6ca54e290189b42a68ab64d0d2065b7`  
		Last Modified: Wed, 01 Mar 2023 01:51:43 GMT  
		Size: 48.1 MB (48072838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402a03a1c745fc42a93ed0082abf13d52e0c961da496b7b2d7d9a60a1d8031f`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 8.5 MB (8496389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea6f1f01cbcb26c4e22bf2c443b3515e57d9267d84661daeb7ae809ff62ff82`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 11.1 MB (11051495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db38c030ddb0562da5b6a4ed2e4333299c295c785959c19faae6aecfee04f841`  
		Last Modified: Wed, 01 Mar 2023 02:24:07 GMT  
		Size: 61.5 MB (61520999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9363999a5ced7319bb4e8233919bcf696a5ff06ce055f6ff25cddc125630fe82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123900581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14baa6809f04057f886b38600982f1e5bbe9c414e11e8a016f729d70ff9ded84`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:26 GMT
ADD file:9f8ce83cf3e75c63cb351ec688378ffe29d7105ff8e8892b3cef95aeacbf6779 in / 
# Wed, 01 Mar 2023 01:57:27 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:28:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:29:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c5d14f15cd67359c9f8d5dbc636ce6ffee972aa4acbeb663e40e865b0dd7dee`  
		Last Modified: Wed, 01 Mar 2023 02:01:54 GMT  
		Size: 45.8 MB (45843301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925df4d36e5e8049cacb403582ac8832aed842417020be560ab0398e08c8fb67`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 8.1 MB (8140837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5921afe59294ea6e26c9a0c8c143bce276da4ba83ef2f7194b96d034a2b463d`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 10.7 MB (10687660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daffa30bd41618c0f8d8bc932ac6b2e541af6a12c3462963570690c046fb0eb`  
		Last Modified: Wed, 01 Mar 2023 03:08:25 GMT  
		Size: 59.2 MB (59228783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:707d81e8f30e61d9f2aaa457f83a07eae8b2a592a62b58d3d7e9d83da5975f8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133469946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f6c7e35dd573abe7c4284cb4996d045b058236c5962edd7424453357d4c3c5a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:13 GMT
ADD file:5b81699b80066f9e3bc967bdf130a67f54ebe15cd80df6c952262d6132b1cabf in / 
# Wed, 01 Mar 2023 02:20:14 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:46:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:47:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf639a903cc04a00c81ac77b3b9f9a79644c51b7f515895fd60403c20ff34a80`  
		Last Modified: Wed, 01 Mar 2023 02:23:22 GMT  
		Size: 49.3 MB (49273990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42632d5ac93ac504d393018f5e0f56f02bedd9cd2df6e1d91da9fc0ef4806d9b`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 8.9 MB (8882130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c0a0685e10806d6ca5aac08337a76d9fd6a47f16f665f5d3a2e692eabfeb3f`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 11.4 MB (11371530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1ccc2a9c1e986768a01b08e1009a75262c8bac308f9c9d414685034ce162c1`  
		Last Modified: Wed, 01 Mar 2023 02:55:40 GMT  
		Size: 63.9 MB (63942296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ae8e961a9e40fd1cc67a16b2eeb562541342ae4bdaa1e6a49ac66fb1484f8e96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137251175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c2068c6e1d78739e77ceabcc05f5cb988caed03f0c045bd5c99279abfe372a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:38:40 GMT
ADD file:0ccdbb7b1f104c23abcf77c506eed771d5759d210c2284a95f85e558405a5390 in / 
# Wed, 01 Mar 2023 01:38:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:05:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:05:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b5ba6d7d02dd42cc6291ae5b4e129956756f664662a78db71f320107a1b6d189`  
		Last Modified: Wed, 01 Mar 2023 01:43:30 GMT  
		Size: 50.3 MB (50273396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f35c12f0528f81569a1c99e040f4d3527ee4391aa4079d740a4c6638bcece0`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 9.2 MB (9230996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319f35836381f914f3bbf4d55b955e9cf90a83165b64e829c72b52051b5e5c5`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 11.8 MB (11808790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a8ff813204e629160f019ffdb45960b87b39f586133418d3fd5f36323e5f03`  
		Last Modified: Wed, 01 Mar 2023 02:22:30 GMT  
		Size: 65.9 MB (65937993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:58f7776ae5802beb5ff95c124b893ff3a2ce121f93e98d305337e9feeeb340d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131875223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dde5105ffa4ba49e36c8a2afa67c343d1f83bde2ad9dde91a2a56b5056c6d4f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:43:09 GMT
ADD file:bff5ae942e6561f2afffbbd0267d57706f7fdd71ebe43c64b369b20940d55f00 in / 
# Thu, 09 Feb 2023 02:43:14 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:31:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:32:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:33:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aa6addfe979ac43879ea9517851622f7a6c1516568fbd6a0c101c3b86cc1163`  
		Last Modified: Thu, 09 Feb 2023 02:51:51 GMT  
		Size: 49.1 MB (49063446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6db93799880bf6f9525fc696324e0d450fd37ebbb37d356955a9057236da38`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 8.4 MB (8399010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b19fed47eb69b023968097b12ef67cad0d7e15a03675cc16e3efc9b67a44e4`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 11.1 MB (11105521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7152f2a237e2d177c5dc02d27a4b1e0433902b36280eb92369c2a9e5620678e`  
		Last Modified: Thu, 09 Feb 2023 07:57:24 GMT  
		Size: 63.3 MB (63307246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ebef91cd94f5561186fb0b696247790d031846171cfc5662c9592c36adce5858
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144588786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524c9ee0845a8c69cf6771af7edf1490f94ce4d0dda21968e413a26752e9b320`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:46:00 GMT
ADD file:311d9174b941eeaaa2babe3a94b035ab7c3880d5908d630bdec420f42eff6a06 in / 
# Wed, 01 Mar 2023 04:46:05 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:18:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:18:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:20:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6b61b4a96c9a944bd44d67cc885cdb2ef5f9aa35a0a94dba6ea2b6372ad27e48`  
		Last Modified: Wed, 01 Mar 2023 04:52:26 GMT  
		Size: 53.3 MB (53250230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a057e1f93c20f3bf648ce49e3455619f0854aef331a7d297c7425e435adfcb8`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 9.6 MB (9631581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb4683b31216d30e252186c2c0cb6f06f69d737321cb3d95c8f1036adca0bea`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 12.2 MB (12168325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18e9322efa86ed752abe3ce6c6627d95fb158f9e6fc57b15a1dd5c4eeac07ae`  
		Last Modified: Wed, 01 Mar 2023 05:38:09 GMT  
		Size: 69.5 MB (69538650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:70d660b84d8823209adb0b68ba88f2b2bec7a47b14c638270edbc9242cb64841
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130649917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e1f38dc04be68c2fbe7138cf87bcdf1c061ef8a1f11fb0e2353575347e48b18`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:49:37 GMT
ADD file:55baf50ca3524103dfcb38a8784744d482a5cdb19f66a7baa92d44dc18483a58 in / 
# Wed, 01 Mar 2023 02:49:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:12:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e95e47ef2a5cde1145fe4af2db22dbfe40c09cf83dbb9ff00d400d23e6dd5331`  
		Last Modified: Wed, 01 Mar 2023 02:53:58 GMT  
		Size: 47.6 MB (47608102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf204e7b8be3c288518bf65a248e94d7d77b56c235d30b3eb93058f663337226`  
		Last Modified: Wed, 01 Mar 2023 03:21:19 GMT  
		Size: 8.7 MB (8684339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca66d3959e328f7d96d65cb0b1a3f79c9c7f949a2fefecdadb692344f6e8a5b`  
		Last Modified: Wed, 01 Mar 2023 03:21:18 GMT  
		Size: 11.3 MB (11268858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb5857b88499838945e97d7c6a6c6ebe9e8cedf2f9e53fd3969022b50bafb3c`  
		Last Modified: Wed, 01 Mar 2023 03:21:34 GMT  
		Size: 63.1 MB (63088618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:6fc33b1f1bc5e9d66a7cbbaab3f0de66bcdfee49fc51cdd7a1abe8f9e93a1640
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bullseye` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1ab51e666d5331b2ca90421dc657968b50de8c4ea86e747b51f24b0ceac6ee20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322486156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f6175124be93225950f0f44661e6d04c099685b1c6cfdce98c94b6908a005ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:43:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:44:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cdcd4942ebc7445d8a70117a83ecbc77dcc5ffc72c4b6f8e24c0c76cfee15d`  
		Last Modified: Wed, 01 Mar 2023 04:50:33 GMT  
		Size: 54.6 MB (54585443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3bce705f6c47c25b6e7896b4da514bf271c5827b1d19f51611c4a149dd713c`  
		Last Modified: Wed, 01 Mar 2023 04:51:08 GMT  
		Size: 196.8 MB (196811476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d5ebd7b5044f44ae29cf2301dc9d211d4a91de578f8643d9447e2705c89e1fa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295543491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25085575e82e41137aadeab7abf493a22196af92d25adbdd636b34ea590b35b8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:18:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:20:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d373aa541f88e7c81c88d63aca3fd07f01c6220ca295915af87f489a6cb251`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 5.1 MB (5072694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c176fe3230b5050ab13f5cd081fa601f679459e28449694496136a73bddd175c`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 10.6 MB (10573876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04072817b27c20dd9a7f9a0b93816bd195f8675845e235c0291c0f935824f610`  
		Last Modified: Wed, 01 Mar 2023 02:25:18 GMT  
		Size: 52.3 MB (52338815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6353168632306a6374c103fef267a9c6d96bb6102c9ad2cf73bbcd81093088a0`  
		Last Modified: Wed, 01 Mar 2023 02:25:56 GMT  
		Size: 175.0 MB (175008286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:68a9f7cc0785c70372cb8a12f4c245fc83255dabf264e6be54ff359ed27e2a40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (283008511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0390df189979c07f1a2462cc444b49d2112865ac9a6a1631e580a27b55539b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:33:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e676c4187d9dd900add9c8dd4b9c906be40a2b8db6cabfdaf280ac2e83cdfca`  
		Last Modified: Wed, 01 Mar 2023 03:09:35 GMT  
		Size: 50.4 MB (50355863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df966bf734b2531648679fbd424ead324e0892e75539a7b995ac958175ebd568`  
		Last Modified: Wed, 01 Mar 2023 03:10:10 GMT  
		Size: 167.3 MB (167288237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8917040dd4bb6aedfddba59aa82d51536b6ec25930b6f06c9733532a61912af2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.1 MB (314133809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2780396f13c4cbb69cfd74d843bc7bf52d0e90e5d9d9802e537a1a9769446f3a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8747d4a988af1d119e668971a87213d5c7061fc04671ba6fcb7123a1c11507ac`  
		Last Modified: Wed, 01 Mar 2023 02:56:37 GMT  
		Size: 54.7 MB (54676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb701404a7a0229719104b05970d81ecf0a7dea50b3defe137088db6cc3c0d0c`  
		Last Modified: Wed, 01 Mar 2023 02:57:06 GMT  
		Size: 189.7 MB (189727959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:151857e29bb1821d712ec7cfd8e4d8a5d883f37adea2a83c01a48cc2ac69239f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.2 MB (328218457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:038aa1836a9a96ce7b81933a91fa4831e0ba0d768de322b4835e86368581db36`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:10:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471482ade37b25d9ec22336d057dd4ed265a030b98595eac314b56d5709bbdff`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 5.3 MB (5293673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a995bf7fa061158e93790e264fd3bc4a3340e75bf857b3c51814384b5f1344f5`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 11.2 MB (11249844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9955e6ae7dba34d1170876e13f1c83b049619255f38babb22074d26848658318`  
		Last Modified: Wed, 01 Mar 2023 02:23:54 GMT  
		Size: 55.9 MB (55922655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc50efa640196b1840993873638e42246a1137dc3e2ac3534d6cba803fef33f`  
		Last Modified: Wed, 01 Mar 2023 02:24:42 GMT  
		Size: 199.7 MB (199724209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5ea0d35f075afa10f4b0b4cc10b69f2acc8c18ce4089182ad36a944bc68e2d38
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.2 MB (301151652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0222370846c985596fd3058856c6c93024191a6b9fc9adfbf00825509403dfbd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:42:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:47:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791a92fb38ebf78f5ed530cc39361869dd25ce941ea09d0580b866204f0e8e1`  
		Last Modified: Thu, 09 Feb 2023 07:59:50 GMT  
		Size: 4.9 MB (4921594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c347eddc487950d631dca4e7c20c1165566e8418703435fad325a721c0e8d`  
		Last Modified: Thu, 09 Feb 2023 07:59:52 GMT  
		Size: 10.7 MB (10662160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9ee56dfe2667a1d6574684709026d72883d1af28301257038f732b76362e9a`  
		Last Modified: Thu, 09 Feb 2023 08:00:40 GMT  
		Size: 53.3 MB (53307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec8851fe07613cc20ef37a5c4e83efee0eba7c47c653df09be97f187753970`  
		Last Modified: Thu, 09 Feb 2023 08:02:44 GMT  
		Size: 179.0 MB (178993425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bc66949fb3e5bb8519171d6c99462250e7c90213077a00562f8da2ad7567fdd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330990552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e22aacee9f5e429288440511032e88b59ac9b6015c67ad2859a1549cfdc03f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:01 GMT
ADD file:40523b7b16ccf1ff245b11e11f92d24e9e6e9dfbdbc755d4361cf55c7ec26244 in / 
# Wed, 01 Mar 2023 04:47:11 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:25:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:26:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:30:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b7949e1acd104233f80137ab3a92a148b0d48e41b3075c70a2d636c3b4c60bf`  
		Last Modified: Wed, 01 Mar 2023 04:53:18 GMT  
		Size: 58.9 MB (58921304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b3574e90831068a9bd9f64e57da92a087d925f0a0e63c764ecf421b18d3a1`  
		Last Modified: Wed, 01 Mar 2023 05:39:22 GMT  
		Size: 5.4 MB (5415247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8bec1f2d073d24de5e7dd051bcada4f0a407fc713e38b49fc2d2a863bde38e`  
		Last Modified: Wed, 01 Mar 2023 05:39:23 GMT  
		Size: 11.6 MB (11629925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3bc8a98c359709356de5d552e69a43170d7f81b4ad5ac17cfbb0eb8d3da2b1`  
		Last Modified: Wed, 01 Mar 2023 05:39:53 GMT  
		Size: 58.9 MB (58863932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266ad73c7e2640ed2a8bd13bc5ae4a7289e4d94678b520531d6e6a4c628b4936`  
		Last Modified: Wed, 01 Mar 2023 05:40:52 GMT  
		Size: 196.2 MB (196160144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8ced439af7f8f74e519890670464e8a54d02445b50906c0a580cb23381403b74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296068375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be656e6f4f9d501e5be96387e4ee7f13eed0dda7e92ac3582f1ba01b78338d6b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:07 GMT
ADD file:e5f01d8f88c8134571e8998672a504ecad259a9a8322df73aed4a93ffac08ebd in / 
# Wed, 01 Mar 2023 02:50:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:14:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:16:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51f6de0debe6daa552b12c9951f6529a870979d923187c1ba62ff66cee3450ac`  
		Last Modified: Wed, 01 Mar 2023 02:54:25 GMT  
		Size: 53.3 MB (53277694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6404e912b557d72a71a982115ad4b92e1c23918b7f0c950f6f22c2ec775ff936`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 5.1 MB (5149110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0561ee66ff6ae2ce12d922c3d0fed94e18a801571a2add9e526e914cb30a3bab`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 10.8 MB (10765987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c7ccf7cb532de1600bce9245b8e167d6d644608677c26601c246c4e80cdbf`  
		Last Modified: Wed, 01 Mar 2023 03:22:28 GMT  
		Size: 54.1 MB (54060191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2854c5c8fd871ba1d0f27ad51f05fba4d434683959e10cbe9fc7fb3281ec3415`  
		Last Modified: Wed, 01 Mar 2023 03:22:56 GMT  
		Size: 172.8 MB (172815393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:ec811d02884e77b7756e199aa29b0865fbff832fdb1b5f9e510ab1ec7059fbe0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fcea8a2b5af99f3d6240c4f8eb6bd3c30893eef1187fdcee771094c9dff6ae15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71089237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b9d6ef1ff1378d683604cf4ba99f8836f7e2f16205f16d0feee677d899d5f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:be1997f59f6670c0a7fc280c3d6359c5d34415bc035eb076dfd4bd5f03501c85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68196390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e730b28fdc731ae3aaca7b8b139d87185e0c39a2bd20b42109b12e72aa0236c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d373aa541f88e7c81c88d63aca3fd07f01c6220ca295915af87f489a6cb251`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 5.1 MB (5072694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c176fe3230b5050ab13f5cd081fa601f679459e28449694496136a73bddd175c`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 10.6 MB (10573876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:18d2756e7bcd00b93725240b830db6fe1095fc56d99228add890da041da1f64d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65364411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f10eddb1560f07c7bcfb9aae4af0d2ea57813820d425be262f39715ac534f490`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b0704702833d7486169b32592de4d7068ee216859e8120201ea440fa4b09d0bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69729485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff94eb1fb8fbc51d7ca80c6fc3291cde8e30e0e72289b6f6eaf32f54a0c6bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d92dd1d966478b3c6c0071bda6a468cf1459f49477c797452577f15e8810419b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72571593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5754a4da25c3b4c118346601bc5c735071a21e432587b386aa113af8f5d0e31`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471482ade37b25d9ec22336d057dd4ed265a030b98595eac314b56d5709bbdff`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 5.3 MB (5293673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a995bf7fa061158e93790e264fd3bc4a3340e75bf857b3c51814384b5f1344f5`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 11.2 MB (11249844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4b7b85b9386e8a62061db8f6de3d3f14d9c766b5afc78bce6a2277e61cb0d35e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68850538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e15959eca1ab694d171b213aa90363b529e588c0d215964cf8a4c3e6e8c0acc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791a92fb38ebf78f5ed530cc39361869dd25ce941ea09d0580b866204f0e8e1`  
		Last Modified: Thu, 09 Feb 2023 07:59:50 GMT  
		Size: 4.9 MB (4921594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c347eddc487950d631dca4e7c20c1165566e8418703435fad325a721c0e8d`  
		Last Modified: Thu, 09 Feb 2023 07:59:52 GMT  
		Size: 10.7 MB (10662160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5cf07060832cb3528f68597bf86a23931d11ca79238393925aa56a42aefbf2f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75966476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8505f47b3532655ea317846fe63792fa9fb98b85bd3bc950eba5cda1532a0a29`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:01 GMT
ADD file:40523b7b16ccf1ff245b11e11f92d24e9e6e9dfbdbc755d4361cf55c7ec26244 in / 
# Wed, 01 Mar 2023 04:47:11 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:25:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3b7949e1acd104233f80137ab3a92a148b0d48e41b3075c70a2d636c3b4c60bf`  
		Last Modified: Wed, 01 Mar 2023 04:53:18 GMT  
		Size: 58.9 MB (58921304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b3574e90831068a9bd9f64e57da92a087d925f0a0e63c764ecf421b18d3a1`  
		Last Modified: Wed, 01 Mar 2023 05:39:22 GMT  
		Size: 5.4 MB (5415247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8bec1f2d073d24de5e7dd051bcada4f0a407fc713e38b49fc2d2a863bde38e`  
		Last Modified: Wed, 01 Mar 2023 05:39:23 GMT  
		Size: 11.6 MB (11629925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ef8f8a6921a906b5f70110da039d2ba658262090af1f1082123d7adc15ea63f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69192791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905dee6c4c69217ff79bc7d612aa22e1d4d29c3735ff980996291dfc3677f416`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:07 GMT
ADD file:e5f01d8f88c8134571e8998672a504ecad259a9a8322df73aed4a93ffac08ebd in / 
# Wed, 01 Mar 2023 02:50:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:51f6de0debe6daa552b12c9951f6529a870979d923187c1ba62ff66cee3450ac`  
		Last Modified: Wed, 01 Mar 2023 02:54:25 GMT  
		Size: 53.3 MB (53277694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6404e912b557d72a71a982115ad4b92e1c23918b7f0c950f6f22c2ec775ff936`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 5.1 MB (5149110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0561ee66ff6ae2ce12d922c3d0fed94e18a801571a2add9e526e914cb30a3bab`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 10.8 MB (10765987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:f5efcf35ed707b7aeb078d6ddfdefc91a9715390a7d8003e51338f7d3630c941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bullseye-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a6ef7420ef5f9b158be970b586c122041efe47c340f36511af02b66b15f50021
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125674680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5069942e3d6eec75afd35fb58f4b25abd6e63a90e224fdfc1ef8b3db05d82130`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:43:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cdcd4942ebc7445d8a70117a83ecbc77dcc5ffc72c4b6f8e24c0c76cfee15d`  
		Last Modified: Wed, 01 Mar 2023 04:50:33 GMT  
		Size: 54.6 MB (54585443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e6642afa6470d719d40e0aedb05dcd82386c83ea9e49990ecd703001eea0708c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120535205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10cf2c6f88593a41cfd3f16b24bfee123e13190615f8330cee60375c884c9e4b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:18:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d373aa541f88e7c81c88d63aca3fd07f01c6220ca295915af87f489a6cb251`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 5.1 MB (5072694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c176fe3230b5050ab13f5cd081fa601f679459e28449694496136a73bddd175c`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 10.6 MB (10573876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04072817b27c20dd9a7f9a0b93816bd195f8675845e235c0291c0f935824f610`  
		Last Modified: Wed, 01 Mar 2023 02:25:18 GMT  
		Size: 52.3 MB (52338815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c7076592183315790b451e7400610a2108a088eff9828031faacdc4ec0ef67b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115720274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adf4d1a818db1580563de9b22ed7fcc9738c034bdc78b5f4613ef9e96e02bd1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e676c4187d9dd900add9c8dd4b9c906be40a2b8db6cabfdaf280ac2e83cdfca`  
		Last Modified: Wed, 01 Mar 2023 03:09:35 GMT  
		Size: 50.4 MB (50355863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cf7219efab275bd3d3fbfd3ab95e7f321352cb3c012f6368843680ccb19abe5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124405850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf6eda9f040f4295ca3f9857f1ea0b5a1fdcc0cdb7491510b5223a2bf02530f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8747d4a988af1d119e668971a87213d5c7061fc04671ba6fcb7123a1c11507ac`  
		Last Modified: Wed, 01 Mar 2023 02:56:37 GMT  
		Size: 54.7 MB (54676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bf5cacb020595095738a86d659889e8825c9cee19c92064a670ddafcb6207a08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128494248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab6f0c472327c2c68c41ac703fb1caadce376b919f50c96745d2ae9165023bf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471482ade37b25d9ec22336d057dd4ed265a030b98595eac314b56d5709bbdff`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 5.3 MB (5293673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a995bf7fa061158e93790e264fd3bc4a3340e75bf857b3c51814384b5f1344f5`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 11.2 MB (11249844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9955e6ae7dba34d1170876e13f1c83b049619255f38babb22074d26848658318`  
		Last Modified: Wed, 01 Mar 2023 02:23:54 GMT  
		Size: 55.9 MB (55922655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:07d501b1a244ee7c0ed6d4e9c5c5704cedd96cfb51bc776b2c778aec5bd274a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122158227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f882bdd498e5f8cf1f6bfe78012ad9b00c0b3e1d476d3b20a12bef5e08231e5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:42:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791a92fb38ebf78f5ed530cc39361869dd25ce941ea09d0580b866204f0e8e1`  
		Last Modified: Thu, 09 Feb 2023 07:59:50 GMT  
		Size: 4.9 MB (4921594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c347eddc487950d631dca4e7c20c1165566e8418703435fad325a721c0e8d`  
		Last Modified: Thu, 09 Feb 2023 07:59:52 GMT  
		Size: 10.7 MB (10662160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9ee56dfe2667a1d6574684709026d72883d1af28301257038f732b76362e9a`  
		Last Modified: Thu, 09 Feb 2023 08:00:40 GMT  
		Size: 53.3 MB (53307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8bd4ae58c5a9dd9152f3d51bfd815b98f2dbfec6309beb31666524144e8db6a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134830408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0053e746dde1fab6a1b0954f7f14f6d3a0eb7689b80f2ccaa15954b3b156e44c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:01 GMT
ADD file:40523b7b16ccf1ff245b11e11f92d24e9e6e9dfbdbc755d4361cf55c7ec26244 in / 
# Wed, 01 Mar 2023 04:47:11 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:25:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:26:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b7949e1acd104233f80137ab3a92a148b0d48e41b3075c70a2d636c3b4c60bf`  
		Last Modified: Wed, 01 Mar 2023 04:53:18 GMT  
		Size: 58.9 MB (58921304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b3574e90831068a9bd9f64e57da92a087d925f0a0e63c764ecf421b18d3a1`  
		Last Modified: Wed, 01 Mar 2023 05:39:22 GMT  
		Size: 5.4 MB (5415247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8bec1f2d073d24de5e7dd051bcada4f0a407fc713e38b49fc2d2a863bde38e`  
		Last Modified: Wed, 01 Mar 2023 05:39:23 GMT  
		Size: 11.6 MB (11629925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3bc8a98c359709356de5d552e69a43170d7f81b4ad5ac17cfbb0eb8d3da2b1`  
		Last Modified: Wed, 01 Mar 2023 05:39:53 GMT  
		Size: 58.9 MB (58863932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f26531b6a394a77d086c8d03202eddded5c7e44b39da743ad759ba173721a941
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123252982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab21b2830a2681e63ef03f163b5c2437190e155339ff1e3db316ff358b283e3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:07 GMT
ADD file:e5f01d8f88c8134571e8998672a504ecad259a9a8322df73aed4a93ffac08ebd in / 
# Wed, 01 Mar 2023 02:50:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:14:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51f6de0debe6daa552b12c9951f6529a870979d923187c1ba62ff66cee3450ac`  
		Last Modified: Wed, 01 Mar 2023 02:54:25 GMT  
		Size: 53.3 MB (53277694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6404e912b557d72a71a982115ad4b92e1c23918b7f0c950f6f22c2ec775ff936`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 5.1 MB (5149110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0561ee66ff6ae2ce12d922c3d0fed94e18a801571a2add9e526e914cb30a3bab`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 10.8 MB (10765987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c7ccf7cb532de1600bce9245b8e167d6d644608677c26601c246c4e80cdbf`  
		Last Modified: Wed, 01 Mar 2023 03:22:28 GMT  
		Size: 54.1 MB (54060191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:63be0fe0bfb9d06b8747dcd87683787ef6d82c6f05b8a2ae213c38d56dc2bf53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d836de599cb6f6ae477b9fd28a1439b9ee0a26d805a2be9fec1aeb7df5256811
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.1 MB (312112050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd092f9559e9c632d4ce17e2cc3a5a87d8bfe07663f67c5416f5cadf4a9b23a6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:44:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:44:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:44:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:46:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fc05781c9a4a3dee77723abf708dd674020a00d7d57dd6cc1f9bc72da96143`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 7.9 MB (7862980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efc3ea86e67ce8cdce1cf3619f311735cbbb8744a1c69536f8a390d014c0a99`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 10.0 MB (10001392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47452733a7c0712961d7ef8b48e3d823328f056af1c90c715966748b137b3d1c`  
		Last Modified: Wed, 01 Mar 2023 04:51:39 GMT  
		Size: 51.9 MB (51873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f68a3641163543e513f65bb04fd6c440c0569b7f3e0cf3c3735a5718cb42169`  
		Last Modified: Wed, 01 Mar 2023 04:52:10 GMT  
		Size: 191.9 MB (191924876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8203a9192ea844c6cb0f1f395cd6baa1f8db1c36605c92ca4392a817bcfaf81d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.9 MB (277910034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a08160c6fdb784988b93c2bdf8eead75a0af2edffc9c3bc13ffe5e54839098`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:03 GMT
ADD file:28e7414281fcd12661d43cccdf7062bf4aa15641f986cae3aa3260fcb8e16bb5 in / 
# Wed, 01 Mar 2023 01:58:03 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:34:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:34:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:34:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:36:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ba30d485dd0583b3079a70184a97c458599a0629e661b1382394653cb802242`  
		Last Modified: Wed, 01 Mar 2023 02:03:25 GMT  
		Size: 45.9 MB (45916077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5b3ed640e906ad20c2a86568f52c60a48e1d82e4654d3378280f572737f7c1`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 7.2 MB (7152340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028b21e39d17f6632c7b82f0c900d32b50233b13940a7a60009782a6abc32cdd`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 9.3 MB (9349019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35297b6d570293c7581e727c51353a6eb15d3b2f7bdaf391595c28c2a8d4fc6`  
		Last Modified: Wed, 01 Mar 2023 03:10:43 GMT  
		Size: 47.4 MB (47396639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db985543ef8399c92c217abd234865cfb8fc38d73e04bede21a4921385745eae`  
		Last Modified: Wed, 01 Mar 2023 03:11:15 GMT  
		Size: 168.1 MB (168095959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:142ad5211953587c7ba8af3681096fee98c692d6b3c9edaf36daac5e1eb477e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302666222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf2cd8921f2ed4913a5a1f9d79c8b6ef3776901ad259d2e10a0e271e66bb1d25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:50:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:51:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:52:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a788623352140f16227efacfe9a8b497cf91ee63fa69554615640474975ca5`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 7.7 MB (7731356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12086fb08985806514ae1e77eef44a12e303bd44b113e62dac28b16b778fc797`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 10.0 MB (10003642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afc4bf76406adbdc8533ba0c416f2aac77ca7db02bb6d380eaeeb778f56c5d4`  
		Last Modified: Wed, 01 Mar 2023 02:57:32 GMT  
		Size: 52.2 MB (52192055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7fd78b041bf9263b5362da19c99f8256c7954621d32679777cd6fcd99d86a`  
		Last Modified: Wed, 01 Mar 2023 02:57:57 GMT  
		Size: 183.5 MB (183499167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d05278970db620073bd62426cdb4d4dc191128f0fd30eb30b0d260b452482119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.5 MB (321526216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95d43e15f63c3b2bafcd52b42a1a9f683924f8208cec5e19fb9dac302ee4a1b1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:23 GMT
ADD file:4a87d706ba1c6cdeab729abca0c932709611862dfdf5d46d9f07660a549fd043 in / 
# Wed, 01 Mar 2023 01:39:24 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:10:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:11:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:11:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:13:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:965c7d391035444250e8549e1aa77d80a0692089e844b5c3d6f4e4924f096a99`  
		Last Modified: Wed, 01 Mar 2023 01:45:08 GMT  
		Size: 51.2 MB (51207396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7561c3f10011960cdcee2d97ca318791aeb60e8e7b34375e50ce1691e1f373b6`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 8.0 MB (8033127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edba82cb80eba68e543537bb7bf09a496a1270646491b65f1804a2551eceae`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 10.3 MB (10345751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe6c0714838b2d72c79e2fb8a0fb23c8de6b3d246827b2fd913e3af6734aaa`  
		Last Modified: Wed, 01 Mar 2023 02:25:21 GMT  
		Size: 53.5 MB (53471402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858b45e654212bda5c76759252da6702f83ee966fcf91e7131a8e9ab4f2f5a17`  
		Last Modified: Wed, 01 Mar 2023 02:26:05 GMT  
		Size: 198.5 MB (198468540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:42598525905fd1e45966adbb9f2c69f78ca053feb530bf7b99e572b89fd3f77c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:edf320c3d1538c793e4aa6db8ae0030fb8d9bcd93c32d1173668018af289abd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68313473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e264a14e2fb2275166171b218ac3b34315ea1e90c78b540056de532c018c86b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:44:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:44:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fc05781c9a4a3dee77723abf708dd674020a00d7d57dd6cc1f9bc72da96143`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 7.9 MB (7862980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efc3ea86e67ce8cdce1cf3619f311735cbbb8744a1c69536f8a390d014c0a99`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 10.0 MB (10001392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:260fa862731a48f61d191023a25f1f9b657f45a421b53cb8857c87b68f3d1e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62417436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768e09ebea3080e9905c76f34b636f7ae2caced8f0c84dcdb609ad8c6b2d1c5a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:03 GMT
ADD file:28e7414281fcd12661d43cccdf7062bf4aa15641f986cae3aa3260fcb8e16bb5 in / 
# Wed, 01 Mar 2023 01:58:03 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:34:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:34:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4ba30d485dd0583b3079a70184a97c458599a0629e661b1382394653cb802242`  
		Last Modified: Wed, 01 Mar 2023 02:03:25 GMT  
		Size: 45.9 MB (45916077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5b3ed640e906ad20c2a86568f52c60a48e1d82e4654d3378280f572737f7c1`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 7.2 MB (7152340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028b21e39d17f6632c7b82f0c900d32b50233b13940a7a60009782a6abc32cdd`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 9.3 MB (9349019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:129a088e650fae94076fc92386141a86cd2f37e370edc651d6fcdebd47ca9887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66975000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4479ef63c587db1ceab4c7d6387457f7c8109f921dc37d1fb1618c608893d402`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:50:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a788623352140f16227efacfe9a8b497cf91ee63fa69554615640474975ca5`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 7.7 MB (7731356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12086fb08985806514ae1e77eef44a12e303bd44b113e62dac28b16b778fc797`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 10.0 MB (10003642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8f735fd4bda81af31cec932c12fee884df969e8a32b286fa0d652d1555d356a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69586274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed659aba5f7d179e5c1a17d9d85e4a30314268a86ca791736d27013b45cc57ef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:23 GMT
ADD file:4a87d706ba1c6cdeab729abca0c932709611862dfdf5d46d9f07660a549fd043 in / 
# Wed, 01 Mar 2023 01:39:24 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:10:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:11:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:965c7d391035444250e8549e1aa77d80a0692089e844b5c3d6f4e4924f096a99`  
		Last Modified: Wed, 01 Mar 2023 01:45:08 GMT  
		Size: 51.2 MB (51207396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7561c3f10011960cdcee2d97ca318791aeb60e8e7b34375e50ce1691e1f373b6`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 8.0 MB (8033127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edba82cb80eba68e543537bb7bf09a496a1270646491b65f1804a2551eceae`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 10.3 MB (10345751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:179f7c72ed12161b5e7a09e106882d6b82077554946eb99908d44ac79a1d8a91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f2c53ffd804089bac100dacb8c968c3c9d375d99a42a7ab5f596d77ba333046b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120187174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da6f85600da7d195cbab7b247097c398fdf3b93551418d77e05df7d7563d17d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:44:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:44:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:44:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fc05781c9a4a3dee77723abf708dd674020a00d7d57dd6cc1f9bc72da96143`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 7.9 MB (7862980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efc3ea86e67ce8cdce1cf3619f311735cbbb8744a1c69536f8a390d014c0a99`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 10.0 MB (10001392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47452733a7c0712961d7ef8b48e3d823328f056af1c90c715966748b137b3d1c`  
		Last Modified: Wed, 01 Mar 2023 04:51:39 GMT  
		Size: 51.9 MB (51873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:88b650bc14650aff80cfac6809cce960f3eb237f5d1aa230be53efcbb8e39e0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109814075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd66a0bcb6cf53591c330eecba51cca59ae4ab082c1d62528b68861ac89863cf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:03 GMT
ADD file:28e7414281fcd12661d43cccdf7062bf4aa15641f986cae3aa3260fcb8e16bb5 in / 
# Wed, 01 Mar 2023 01:58:03 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:34:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:34:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:34:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ba30d485dd0583b3079a70184a97c458599a0629e661b1382394653cb802242`  
		Last Modified: Wed, 01 Mar 2023 02:03:25 GMT  
		Size: 45.9 MB (45916077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5b3ed640e906ad20c2a86568f52c60a48e1d82e4654d3378280f572737f7c1`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 7.2 MB (7152340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028b21e39d17f6632c7b82f0c900d32b50233b13940a7a60009782a6abc32cdd`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 9.3 MB (9349019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35297b6d570293c7581e727c51353a6eb15d3b2f7bdaf391595c28c2a8d4fc6`  
		Last Modified: Wed, 01 Mar 2023 03:10:43 GMT  
		Size: 47.4 MB (47396639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:90aa1cac3a307d98880753d6cf9760451142763726f491a838ac25e086333607
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119167055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e9a68c76d5f6d839f7521c0ad7aea5ed89f2bc316ae2264d2194744d29c61b7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:50:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:51:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a788623352140f16227efacfe9a8b497cf91ee63fa69554615640474975ca5`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 7.7 MB (7731356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12086fb08985806514ae1e77eef44a12e303bd44b113e62dac28b16b778fc797`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 10.0 MB (10003642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afc4bf76406adbdc8533ba0c416f2aac77ca7db02bb6d380eaeeb778f56c5d4`  
		Last Modified: Wed, 01 Mar 2023 02:57:32 GMT  
		Size: 52.2 MB (52192055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0229c279db07ac7afae573e7d92394661b8c51cf18da96afb9fa3484414f8d88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123057676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5cfe505ca5988b3b2fe88cd03e4789c502265fc7d6bee4b1b277b5241d4c139`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:23 GMT
ADD file:4a87d706ba1c6cdeab729abca0c932709611862dfdf5d46d9f07660a549fd043 in / 
# Wed, 01 Mar 2023 01:39:24 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:10:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:11:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:11:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:965c7d391035444250e8549e1aa77d80a0692089e844b5c3d6f4e4924f096a99`  
		Last Modified: Wed, 01 Mar 2023 01:45:08 GMT  
		Size: 51.2 MB (51207396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7561c3f10011960cdcee2d97ca318791aeb60e8e7b34375e50ce1691e1f373b6`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 8.0 MB (8033127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edba82cb80eba68e543537bb7bf09a496a1270646491b65f1804a2551eceae`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 10.3 MB (10345751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe6c0714838b2d72c79e2fb8a0fb23c8de6b3d246827b2fd913e3af6734aaa`  
		Last Modified: Wed, 01 Mar 2023 02:25:21 GMT  
		Size: 53.5 MB (53471402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:ec811d02884e77b7756e199aa29b0865fbff832fdb1b5f9e510ab1ec7059fbe0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fcea8a2b5af99f3d6240c4f8eb6bd3c30893eef1187fdcee771094c9dff6ae15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71089237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b9d6ef1ff1378d683604cf4ba99f8836f7e2f16205f16d0feee677d899d5f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:be1997f59f6670c0a7fc280c3d6359c5d34415bc035eb076dfd4bd5f03501c85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68196390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e730b28fdc731ae3aaca7b8b139d87185e0c39a2bd20b42109b12e72aa0236c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d373aa541f88e7c81c88d63aca3fd07f01c6220ca295915af87f489a6cb251`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 5.1 MB (5072694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c176fe3230b5050ab13f5cd081fa601f679459e28449694496136a73bddd175c`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 10.6 MB (10573876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:18d2756e7bcd00b93725240b830db6fe1095fc56d99228add890da041da1f64d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65364411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f10eddb1560f07c7bcfb9aae4af0d2ea57813820d425be262f39715ac534f490`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b0704702833d7486169b32592de4d7068ee216859e8120201ea440fa4b09d0bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69729485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff94eb1fb8fbc51d7ca80c6fc3291cde8e30e0e72289b6f6eaf32f54a0c6bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d92dd1d966478b3c6c0071bda6a468cf1459f49477c797452577f15e8810419b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72571593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5754a4da25c3b4c118346601bc5c735071a21e432587b386aa113af8f5d0e31`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471482ade37b25d9ec22336d057dd4ed265a030b98595eac314b56d5709bbdff`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 5.3 MB (5293673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a995bf7fa061158e93790e264fd3bc4a3340e75bf857b3c51814384b5f1344f5`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 11.2 MB (11249844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4b7b85b9386e8a62061db8f6de3d3f14d9c766b5afc78bce6a2277e61cb0d35e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68850538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e15959eca1ab694d171b213aa90363b529e588c0d215964cf8a4c3e6e8c0acc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791a92fb38ebf78f5ed530cc39361869dd25ce941ea09d0580b866204f0e8e1`  
		Last Modified: Thu, 09 Feb 2023 07:59:50 GMT  
		Size: 4.9 MB (4921594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c347eddc487950d631dca4e7c20c1165566e8418703435fad325a721c0e8d`  
		Last Modified: Thu, 09 Feb 2023 07:59:52 GMT  
		Size: 10.7 MB (10662160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5cf07060832cb3528f68597bf86a23931d11ca79238393925aa56a42aefbf2f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75966476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8505f47b3532655ea317846fe63792fa9fb98b85bd3bc950eba5cda1532a0a29`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:01 GMT
ADD file:40523b7b16ccf1ff245b11e11f92d24e9e6e9dfbdbc755d4361cf55c7ec26244 in / 
# Wed, 01 Mar 2023 04:47:11 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:25:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3b7949e1acd104233f80137ab3a92a148b0d48e41b3075c70a2d636c3b4c60bf`  
		Last Modified: Wed, 01 Mar 2023 04:53:18 GMT  
		Size: 58.9 MB (58921304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b3574e90831068a9bd9f64e57da92a087d925f0a0e63c764ecf421b18d3a1`  
		Last Modified: Wed, 01 Mar 2023 05:39:22 GMT  
		Size: 5.4 MB (5415247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8bec1f2d073d24de5e7dd051bcada4f0a407fc713e38b49fc2d2a863bde38e`  
		Last Modified: Wed, 01 Mar 2023 05:39:23 GMT  
		Size: 11.6 MB (11629925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ef8f8a6921a906b5f70110da039d2ba658262090af1f1082123d7adc15ea63f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69192791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905dee6c4c69217ff79bc7d612aa22e1d4d29c3735ff980996291dfc3677f416`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:07 GMT
ADD file:e5f01d8f88c8134571e8998672a504ecad259a9a8322df73aed4a93ffac08ebd in / 
# Wed, 01 Mar 2023 02:50:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:51f6de0debe6daa552b12c9951f6529a870979d923187c1ba62ff66cee3450ac`  
		Last Modified: Wed, 01 Mar 2023 02:54:25 GMT  
		Size: 53.3 MB (53277694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6404e912b557d72a71a982115ad4b92e1c23918b7f0c950f6f22c2ec775ff936`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 5.1 MB (5149110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0561ee66ff6ae2ce12d922c3d0fed94e18a801571a2add9e526e914cb30a3bab`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 10.8 MB (10765987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:a11f66d3c0fa48068548afb9f0f6267d91c30c0978f7188baecddf4633ce1bc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b6044fe0ea91b2cd36ee16c377c20c075edb706ba5be48540aa2fccf4169ff31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245768017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0a701ccabc26fb680af02d6d5484e65e2f848b7c60b7dcfabd456bb4e567dc4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:04:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:10:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a237f683deeaa2a1c0890df8ef39ae4992942dd5f941568e877d152a4122aeff`  
		Last Modified: Wed, 01 Feb 2023 18:22:50 GMT  
		Size: 7.7 MB (7735535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84750871be6cfbe4bb1ca3e7384e8526de5f7b7b8f49b37bbc0d94287db639f5`  
		Last Modified: Wed, 01 Feb 2023 18:22:49 GMT  
		Size: 3.6 MB (3627183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3056067387e475581218929338f5478a109fa03d224f88cef9f5ba3a22fbc800`  
		Last Modified: Wed, 01 Feb 2023 18:23:08 GMT  
		Size: 60.7 MB (60742597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258c66296219a7b7f41beceb4f3979c1dd30fb4a55f596c75335276bb34d88d3`  
		Last Modified: Wed, 01 Feb 2023 18:23:36 GMT  
		Size: 145.1 MB (145084818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f4ee369710a84cb660402bee1c73209a428f764fda46b673feec3f37e2190801
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211782702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0351a6ec07f5b3af00d6ced3b1f89da1250782ef25e86ba929626bb6b0552836`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:44:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:45:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:46:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfec9140f00308d23390b191044e2a19bc136e489c813d5449af91bce5b0fe91`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 6.7 MB (6726028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322177715419d97a5871a54f1c8b6fe075220a62dbc72bf41c6dc026440d5e77`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 3.1 MB (3104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33af114797df1d06812900ae5107eeafe4a319eb59a0e0388b6727ec52388a`  
		Last Modified: Wed, 01 Mar 2023 03:13:52 GMT  
		Size: 55.4 MB (55434564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d2ed515ae4a65ad774d2b63208aab21556b5bbae0dbca4126eb26d47e5fbcc`  
		Last Modified: Wed, 01 Mar 2023 03:14:20 GMT  
		Size: 121.9 MB (121931243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b4cc7c24edb74db1d3026fde36d7f4446fd8f4c3b25754916267437eb4ae9253
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235991864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f505c560cb68d89c057dd93202d11b7d6c7e1c58b8cc78793c3e2024e0915d6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:06:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:08:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5cdb9cef850190bebb21cad6356c74e592895e595965cc2791e2ef2e3fe489`  
		Last Modified: Wed, 01 Feb 2023 18:15:45 GMT  
		Size: 7.6 MB (7598155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8388998b5fb9689298ae466de71dd61e6152fe5f0af22c8bef8f73143bacbe`  
		Last Modified: Wed, 01 Feb 2023 18:15:44 GMT  
		Size: 3.6 MB (3616397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758f847d5fa3aeb24a4166e14afe827f2c45890b91333846af93d79830b11e52`  
		Last Modified: Wed, 01 Feb 2023 18:16:01 GMT  
		Size: 60.8 MB (60817045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c190fb00c9b4804425a4c226157db47db90c06ebb209ce79bffd3f87905464`  
		Last Modified: Wed, 01 Feb 2023 18:16:24 GMT  
		Size: 136.8 MB (136766530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:debd6713520a08db50ed1f8da42e4bb8e64256ff314855e17f38e90446516066
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269615848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895823ff50fad310667fb8ab0c42d6f19c33db62519e3d9b21d71a03b38ef2db`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:30 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:31 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:34 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Wed, 01 Feb 2023 11:27:34 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:06:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:10:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c2f997991bfe2ed920105bb595c3662038cc90a08c6db9888fffdfa8c673b16`  
		Last Modified: Tue, 31 Jan 2023 18:14:55 GMT  
		Size: 33.3 MB (33300341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade8a91aca205fdfb604595f12435c45449780688c97c002034b3480b4d6e2f`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 8.7 MB (8689144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d265fb7cba3184708a8658bbe28f6d6d9211befbded0f8b5cfeb9ffa0ba5450`  
		Last Modified: Wed, 01 Feb 2023 18:20:40 GMT  
		Size: 4.5 MB (4486791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a9987c53440b65f7504e1d2c125e138e961fb52b5bddc2d0867140186bf880`  
		Last Modified: Wed, 01 Feb 2023 18:21:16 GMT  
		Size: 69.5 MB (69549088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62134bdf1c65d5122d7110f6b1b984c70adc7fd07c674647a66c826e82bb4db`  
		Last Modified: Wed, 01 Feb 2023 18:22:05 GMT  
		Size: 153.6 MB (153590484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c95b6aae122f7f76230ddda12ca65b704361cbe8e9494b2361443a8eb10fcf5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226361958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4911e269a7ec2a84ce69826ff10b45db58595afe5b4e7e8597412cc3d7b80c7b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 12:00:21 GMT
ARG RELEASE
# Wed, 01 Feb 2023 12:00:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 12:00:23 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Wed, 01 Feb 2023 12:00:24 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:12:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:14:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbc0e1117f61ba365a9a02263b82c04f704d5d162aa31b25a9326797dd1c7084`  
		Last Modified: Tue, 31 Jan 2023 17:54:46 GMT  
		Size: 27.0 MB (27016130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc2216ece6dadf4da9b635d2395de116381e0d77d88f239e2440d4b3bd4786c`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 7.4 MB (7375308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d74c38d5b135b15d3f891f4092219a28a69ce6738a9f6f36d1e2a5797d17ae6`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 3.5 MB (3542223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c45bf4caa5f11965d7b2ffce3e1020b2c76ddf1303186de98cb306ca4dedb2`  
		Last Modified: Wed, 01 Feb 2023 18:21:22 GMT  
		Size: 60.0 MB (60013452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1303d755910ead728efff8974e64e475b681de3250682a0aa8d0a19094c85b`  
		Last Modified: Wed, 01 Feb 2023 18:21:45 GMT  
		Size: 128.4 MB (128414845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:49e6eaf11041a83345b2d88f3989f933e331423be807bf41d12ac9ec19510376
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:139902f730347058d9c1a1601cedbd51c4a2656bda19472be86e9ce88d1b09b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39940602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65cdd40989a1f01db8064bf6f6ab912f1a303f06e61425eb6a86136c09a67435`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:04:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a237f683deeaa2a1c0890df8ef39ae4992942dd5f941568e877d152a4122aeff`  
		Last Modified: Wed, 01 Feb 2023 18:22:50 GMT  
		Size: 7.7 MB (7735535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84750871be6cfbe4bb1ca3e7384e8526de5f7b7b8f49b37bbc0d94287db639f5`  
		Last Modified: Wed, 01 Feb 2023 18:22:49 GMT  
		Size: 3.6 MB (3627183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5fdcbea172ca3a8d6a3c1f8e79956915271ef25a450e23c0f8d002d8a40cbf58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34416895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f121c3293b2153a65dc0914441f3c0ce8cdfd71bfe9ffd405a153dc811bce5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:44:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:45:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfec9140f00308d23390b191044e2a19bc136e489c813d5449af91bce5b0fe91`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 6.7 MB (6726028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322177715419d97a5871a54f1c8b6fe075220a62dbc72bf41c6dc026440d5e77`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 3.1 MB (3104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d25ee52ef857785d1cf3704c3ea1d271d3dd3131c3f4d8c46187ce62e02a24e3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38408289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026010a0d29289f441533dfb0918a2ec67e947cf80f38369b4be824ebd761abd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5cdb9cef850190bebb21cad6356c74e592895e595965cc2791e2ef2e3fe489`  
		Last Modified: Wed, 01 Feb 2023 18:15:45 GMT  
		Size: 7.6 MB (7598155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8388998b5fb9689298ae466de71dd61e6152fe5f0af22c8bef8f73143bacbe`  
		Last Modified: Wed, 01 Feb 2023 18:15:44 GMT  
		Size: 3.6 MB (3616397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f12fd21739b9805f915c8a8fcd95f77440c2ade1713eb864f3e9a9cd8f2e1aa0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46476276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e576a3c65f45877574e6fd14bf5613665e5df7b810945d8f29cfb3e32788d488`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:30 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:31 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:34 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Wed, 01 Feb 2023 11:27:34 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0c2f997991bfe2ed920105bb595c3662038cc90a08c6db9888fffdfa8c673b16`  
		Last Modified: Tue, 31 Jan 2023 18:14:55 GMT  
		Size: 33.3 MB (33300341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade8a91aca205fdfb604595f12435c45449780688c97c002034b3480b4d6e2f`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 8.7 MB (8689144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d265fb7cba3184708a8658bbe28f6d6d9211befbded0f8b5cfeb9ffa0ba5450`  
		Last Modified: Wed, 01 Feb 2023 18:20:40 GMT  
		Size: 4.5 MB (4486791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ead28fd5276dd6d06beead5edda1c5465fdaf1102c638d302804abdbf3ab8112
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37933661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf5e6c104c73bfc12b1098e513fdac7cd8818362937b3180a7671a449699f116`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 12:00:21 GMT
ARG RELEASE
# Wed, 01 Feb 2023 12:00:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 12:00:23 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Wed, 01 Feb 2023 12:00:24 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cbc0e1117f61ba365a9a02263b82c04f704d5d162aa31b25a9326797dd1c7084`  
		Last Modified: Tue, 31 Jan 2023 17:54:46 GMT  
		Size: 27.0 MB (27016130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc2216ece6dadf4da9b635d2395de116381e0d77d88f239e2440d4b3bd4786c`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 7.4 MB (7375308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d74c38d5b135b15d3f891f4092219a28a69ce6738a9f6f36d1e2a5797d17ae6`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 3.5 MB (3542223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:97a93de68bfcd86027cb9660aca032ff8201aad2d56677e8db2d49ab799bac95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b001233b50ee9b078a84543d8d08551ff93f4c47c841cd89924c557fda980084
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100683199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508dc825343263364ae968240e3719932e52f5f5de5216a5d2ba307191056546`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:04:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a237f683deeaa2a1c0890df8ef39ae4992942dd5f941568e877d152a4122aeff`  
		Last Modified: Wed, 01 Feb 2023 18:22:50 GMT  
		Size: 7.7 MB (7735535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84750871be6cfbe4bb1ca3e7384e8526de5f7b7b8f49b37bbc0d94287db639f5`  
		Last Modified: Wed, 01 Feb 2023 18:22:49 GMT  
		Size: 3.6 MB (3627183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3056067387e475581218929338f5478a109fa03d224f88cef9f5ba3a22fbc800`  
		Last Modified: Wed, 01 Feb 2023 18:23:08 GMT  
		Size: 60.7 MB (60742597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bc5573a38cb133e8647d1a65a0af37d38f7dea0fa4c9c8f35396e4d80c48cfb5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89851459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a7185ef92eae1a4d52e27855dab33ccee9eabf97d62256082b958d573f92bd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:44:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:45:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:46:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfec9140f00308d23390b191044e2a19bc136e489c813d5449af91bce5b0fe91`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 6.7 MB (6726028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322177715419d97a5871a54f1c8b6fe075220a62dbc72bf41c6dc026440d5e77`  
		Last Modified: Wed, 01 Mar 2023 03:13:31 GMT  
		Size: 3.1 MB (3104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33af114797df1d06812900ae5107eeafe4a319eb59a0e0388b6727ec52388a`  
		Last Modified: Wed, 01 Mar 2023 03:13:52 GMT  
		Size: 55.4 MB (55434564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:31b0c3a25fb4a67287257afd0dbc7ca11f85f0635bf2fa3e746e580c7d79e3ba
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99225334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d3534946432eb97d22d0b303eeaf07846380627bceb09c91f522e5b2b7715b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:06:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5cdb9cef850190bebb21cad6356c74e592895e595965cc2791e2ef2e3fe489`  
		Last Modified: Wed, 01 Feb 2023 18:15:45 GMT  
		Size: 7.6 MB (7598155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8388998b5fb9689298ae466de71dd61e6152fe5f0af22c8bef8f73143bacbe`  
		Last Modified: Wed, 01 Feb 2023 18:15:44 GMT  
		Size: 3.6 MB (3616397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758f847d5fa3aeb24a4166e14afe827f2c45890b91333846af93d79830b11e52`  
		Last Modified: Wed, 01 Feb 2023 18:16:01 GMT  
		Size: 60.8 MB (60817045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ddf4f10cc043ec41a872de8194f92e5c44dbcad6de965cb6be6449dc9bf70425
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116025364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438a5c02f5081ad8934e225034c0bcde18e4aadc08fc556957740a6ee39f4313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:30 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:31 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:34 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Wed, 01 Feb 2023 11:27:34 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:04:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:05:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:06:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c2f997991bfe2ed920105bb595c3662038cc90a08c6db9888fffdfa8c673b16`  
		Last Modified: Tue, 31 Jan 2023 18:14:55 GMT  
		Size: 33.3 MB (33300341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade8a91aca205fdfb604595f12435c45449780688c97c002034b3480b4d6e2f`  
		Last Modified: Wed, 01 Feb 2023 18:20:42 GMT  
		Size: 8.7 MB (8689144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d265fb7cba3184708a8658bbe28f6d6d9211befbded0f8b5cfeb9ffa0ba5450`  
		Last Modified: Wed, 01 Feb 2023 18:20:40 GMT  
		Size: 4.5 MB (4486791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a9987c53440b65f7504e1d2c125e138e961fb52b5bddc2d0867140186bf880`  
		Last Modified: Wed, 01 Feb 2023 18:21:16 GMT  
		Size: 69.5 MB (69549088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7206163a36b7760c9efdbd29a434acc8b1990718675a8ca5f045f76507a5cd08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97947113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f3b12ede6075af4413052ec568fae6e5c908e6e17e9df7d596293718a962c7b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 12:00:21 GMT
ARG RELEASE
# Wed, 01 Feb 2023 12:00:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 12:00:23 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Wed, 01 Feb 2023 12:00:24 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:12:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbc0e1117f61ba365a9a02263b82c04f704d5d162aa31b25a9326797dd1c7084`  
		Last Modified: Tue, 31 Jan 2023 17:54:46 GMT  
		Size: 27.0 MB (27016130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc2216ece6dadf4da9b635d2395de116381e0d77d88f239e2440d4b3bd4786c`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 7.4 MB (7375308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d74c38d5b135b15d3f891f4092219a28a69ce6738a9f6f36d1e2a5797d17ae6`  
		Last Modified: Wed, 01 Feb 2023 18:21:06 GMT  
		Size: 3.5 MB (3542223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c45bf4caa5f11965d7b2ffce3e1020b2c76ddf1303186de98cb306ca4dedb2`  
		Last Modified: Wed, 01 Feb 2023 18:21:22 GMT  
		Size: 60.0 MB (60013452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy`

```console
$ docker pull buildpack-deps@sha256:7934746af260757ca2bd84afbc1df916b3fadde6cb3a3a2e8dd09782ec81ae27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:jammy` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e902a5ede3335b40edf720db97f0f318f2f014bf34395671c61dd7c554c38967
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (250046286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6288482ed9f9138697941e4e8d8adbccf0abf3881591a8a78034ce0bcb07033a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:48:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:48:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:51:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec15466900398b5d701c68ab4f91684333cee7a531fee222d5fcb8a8a7b20d`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.8 MB (3788240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91ea6918177a2aa7ef5f879923eaccfb2e1ddaca74cc714d50e7132ffe71309`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.6 MB (3561486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a44fd0db0640850be18488f070ec215526d9623b7ae525fac72b3f7e3c8efe2`  
		Last Modified: Tue, 31 Jan 2023 18:02:55 GMT  
		Size: 39.4 MB (39353567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df80616fdd7c890e62484c7b02ed89709cb73ab849066978bdfed12211de1893`  
		Last Modified: Tue, 31 Jan 2023 18:03:27 GMT  
		Size: 172.9 MB (172913989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7f1d248f07fb9e2219f7db6f6f1eb23066ceaed4aaac404d9a2e522827dc4508
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218684697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae1e90e96a16ea3fb4fcef9e7eb2c23dfb79daab0d2a3f6479a3b11527335b5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:50:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:51:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:55:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d0210273e3495988f639f6164118a5bba55666799ba86ac3e60a001cf7be3b31`  
		Last Modified: Thu, 26 Jan 2023 18:27:33 GMT  
		Size: 27.0 MB (27022323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adb291ac80bc7a7317277f7bf249ff5cee81ed669a710b5737232792791a9f`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.5 MB (3539082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba7d9da50e7339baf72675e0901adcd0e2dfd5d11fe2d97e09d1847f81f5ec`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.7 MB (3713370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896e49ffa5a98b69e4cc86adad3458a6aeb57fd62d4c77c9346d8ae519a7b34e`  
		Last Modified: Wed, 01 Mar 2023 03:14:50 GMT  
		Size: 41.9 MB (41907099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34997242b6cd858fe662b73826646cda831aab2e426f7100e4bea8e85873b8a`  
		Last Modified: Wed, 01 Mar 2023 03:15:21 GMT  
		Size: 142.5 MB (142502823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:caf791e40ac6f0b770478b2a972bb61566b61055bec3c490602002e692e5a750
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241354172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62b8f09e6592d8a2cb59c6daf4d3893cb9f79a786eacb03714fc9684d6668bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:19:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:19:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:19:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:22:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157508d48eacd7b747f0b9c99ce627da62dd75af25ef8cae0d4a18512f51295`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.8 MB (3761409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53567c3f9bdfe731ccd25b9ed68fb667d0fcde2958e4503859e5d2ad3373d169`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.5 MB (3537451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0d60d77f4f4af1d086be5423a3022abc995163617875e8e23be1474f4e24e1`  
		Last Modified: Tue, 31 Jan 2023 18:35:00 GMT  
		Size: 39.2 MB (39245555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717de65a0562bcf94ca5d94a5fb666ddf872d7dd4266e8185585926c9456b276`  
		Last Modified: Tue, 31 Jan 2023 18:35:26 GMT  
		Size: 166.4 MB (166424783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b6ae80b9fadb3a70f3c443d6a93e07d84d9e9d175e9dd6783e47306ca302f375
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271852926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a05dbe2e0f04dd5f4e8161ff88cec0291770a4b2525078673aa8040c1038b68`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:53:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:54:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:58:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b919bd9d6c8a596b3ac4fb9ee1cc6727efdd1f1b05e5c130efec5deaae53ae60`  
		Last Modified: Tue, 31 Jan 2023 17:52:02 GMT  
		Size: 35.7 MB (35708930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59507b6d89bb36f24882056a420b04435132767ba96bd9396f58bc20ed960488`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.3 MB (4261748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc075be4c307553b270bec14a982c75e55b12a8be0e1232b459d394d27745b9`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.2 MB (4234708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e937188d1ea78ae620a3bc6d078cc63b62a04652da54f26e500081c9d671513`  
		Last Modified: Tue, 31 Jan 2023 18:16:58 GMT  
		Size: 43.8 MB (43763369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92d97251e9f8900abcc79cb6a6dd50f43fb01c99e9b1fd976faa362de19c103`  
		Last Modified: Tue, 31 Jan 2023 18:17:52 GMT  
		Size: 183.9 MB (183884171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bb62bc850242365646a2809a31ec247d0fcde4025c4455a9e1b2c9a8e012d4a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223700429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3bcc113c5afc55cc232bf30c91750911ed6bc45e2a5e111b279a87548ec789`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:42:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:43:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:45:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d244ff6bc0f1d8aab1af2badfb1f1ea2f619ca2316288c519afed909e08b35`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.8 MB (3792000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165dd3ed55b51c4b79b3be0051fe345d5b7e6bedbac65941ff7793e50e07420f`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.5 MB (3472764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bdc26d335cd59059e8429dd773b96bf895a6a3ba4f780d1f01410bfcc95406`  
		Last Modified: Tue, 31 Jan 2023 17:55:46 GMT  
		Size: 39.3 MB (39281842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc1cc2e9a60306dacea281a04f4ce4c694dd1f337848c27c007323cd75c2d3a`  
		Last Modified: Tue, 31 Jan 2023 17:56:09 GMT  
		Size: 148.5 MB (148511897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:77593d112e66c76bcb5a721c77ab1800fc5b926a98ad0f371ef477d1f59fafdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:jammy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f5e6509df320f7774bd73272759602386e5d645fe971116c7dbed0f38e5fdd9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37778730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2441c30f4b69d5096de28028237f2028653245ec5675b95f2d0ba43db75d04bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:48:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec15466900398b5d701c68ab4f91684333cee7a531fee222d5fcb8a8a7b20d`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.8 MB (3788240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91ea6918177a2aa7ef5f879923eaccfb2e1ddaca74cc714d50e7132ffe71309`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.6 MB (3561486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:81c8f547fdd0f4bf9a2ca2f8f03a7269c827b263ce8a97f9fa154ff0c238a49b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34274775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c2f1e2b1fdc4443fba9a9bf00e489d2d7af1f3e886c967e6d9ad67efcb8888e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:50:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d0210273e3495988f639f6164118a5bba55666799ba86ac3e60a001cf7be3b31`  
		Last Modified: Thu, 26 Jan 2023 18:27:33 GMT  
		Size: 27.0 MB (27022323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adb291ac80bc7a7317277f7bf249ff5cee81ed669a710b5737232792791a9f`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.5 MB (3539082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba7d9da50e7339baf72675e0901adcd0e2dfd5d11fe2d97e09d1847f81f5ec`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.7 MB (3713370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:32acc0bceb4b1c5c72adca26c93d797456c8c103acfbd50cd2eda82ee7dbb3f9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35683834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bdaf7c5d9feef034d451541b098820f1836d948fcfe9d0503d7eecc5f27526`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:19:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:19:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157508d48eacd7b747f0b9c99ce627da62dd75af25ef8cae0d4a18512f51295`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.8 MB (3761409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53567c3f9bdfe731ccd25b9ed68fb667d0fcde2958e4503859e5d2ad3373d169`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.5 MB (3537451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b739e985cfa01beb77701e6fda59cbee4cac87054300d98a262a007bc00307fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44205386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f056e39bef72c9a8e678fd7d9cf620857f579ef83f6b5249fddeb1b5edaec956`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:53:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b919bd9d6c8a596b3ac4fb9ee1cc6727efdd1f1b05e5c130efec5deaae53ae60`  
		Last Modified: Tue, 31 Jan 2023 17:52:02 GMT  
		Size: 35.7 MB (35708930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59507b6d89bb36f24882056a420b04435132767ba96bd9396f58bc20ed960488`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.3 MB (4261748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc075be4c307553b270bec14a982c75e55b12a8be0e1232b459d394d27745b9`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.2 MB (4234708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:64c9f347cc5b6931002286f26b60966f7c186b2cde74c1a07cf6a9fbf4d4377d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35906690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e80805a3881c6a17e1e4319a43ce51e28dd9e4c9c2d2fe2e6264526e9a854082`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:42:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d244ff6bc0f1d8aab1af2badfb1f1ea2f619ca2316288c519afed909e08b35`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.8 MB (3792000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165dd3ed55b51c4b79b3be0051fe345d5b7e6bedbac65941ff7793e50e07420f`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.5 MB (3472764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:3c5a7f839c140e03c5210ed96ff4431a338cedf298fe76f68826c4f7e8f6314d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:jammy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:454e170619b5a1fb45cef7bdc6018f456604aecc3a666421048f3b3634964fff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77132297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4fe1d95d55417c7a0fa773212bafbad5fd48a1289f797a988afa9f6ba146653`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:48:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:48:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec15466900398b5d701c68ab4f91684333cee7a531fee222d5fcb8a8a7b20d`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.8 MB (3788240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91ea6918177a2aa7ef5f879923eaccfb2e1ddaca74cc714d50e7132ffe71309`  
		Last Modified: Tue, 31 Jan 2023 18:02:37 GMT  
		Size: 3.6 MB (3561486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a44fd0db0640850be18488f070ec215526d9623b7ae525fac72b3f7e3c8efe2`  
		Last Modified: Tue, 31 Jan 2023 18:02:55 GMT  
		Size: 39.4 MB (39353567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:14b4d1303ec69612ce0d88d0010e45653d7be25d82d48b970925729d826d978d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76181874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a08f78865a253a9d8a65f0544013cf8ddd7c3013aa999a473a82dabc4c5e02`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:50:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:51:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d0210273e3495988f639f6164118a5bba55666799ba86ac3e60a001cf7be3b31`  
		Last Modified: Thu, 26 Jan 2023 18:27:33 GMT  
		Size: 27.0 MB (27022323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adb291ac80bc7a7317277f7bf249ff5cee81ed669a710b5737232792791a9f`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.5 MB (3539082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba7d9da50e7339baf72675e0901adcd0e2dfd5d11fe2d97e09d1847f81f5ec`  
		Last Modified: Wed, 01 Mar 2023 03:14:32 GMT  
		Size: 3.7 MB (3713370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896e49ffa5a98b69e4cc86adad3458a6aeb57fd62d4c77c9346d8ae519a7b34e`  
		Last Modified: Wed, 01 Mar 2023 03:14:50 GMT  
		Size: 41.9 MB (41907099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b6bd1a02efc77bf123fcae7c5524a04f64b272c6a10a3331bdcad862a4fd9d83
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74929389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd560f6d4173dc6a3a41c956564e75c8ad5aa0ff7772f15509939d87cb2c831`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:19:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:19:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:19:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157508d48eacd7b747f0b9c99ce627da62dd75af25ef8cae0d4a18512f51295`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.8 MB (3761409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53567c3f9bdfe731ccd25b9ed68fb667d0fcde2958e4503859e5d2ad3373d169`  
		Last Modified: Tue, 31 Jan 2023 18:34:47 GMT  
		Size: 3.5 MB (3537451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0d60d77f4f4af1d086be5423a3022abc995163617875e8e23be1474f4e24e1`  
		Last Modified: Tue, 31 Jan 2023 18:35:00 GMT  
		Size: 39.2 MB (39245555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:78a62961a5c701ae4bb9459ad0c52261017b9f3b55272c5e4bb4a0796cb3decf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87968755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78a2a507eba7bb61c03b0fd5655bd066d3b7169c709e287b5dc6e1976413cbe9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:53:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:54:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b919bd9d6c8a596b3ac4fb9ee1cc6727efdd1f1b05e5c130efec5deaae53ae60`  
		Last Modified: Tue, 31 Jan 2023 17:52:02 GMT  
		Size: 35.7 MB (35708930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59507b6d89bb36f24882056a420b04435132767ba96bd9396f58bc20ed960488`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.3 MB (4261748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc075be4c307553b270bec14a982c75e55b12a8be0e1232b459d394d27745b9`  
		Last Modified: Tue, 31 Jan 2023 18:16:28 GMT  
		Size: 4.2 MB (4234708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e937188d1ea78ae620a3bc6d078cc63b62a04652da54f26e500081c9d671513`  
		Last Modified: Tue, 31 Jan 2023 18:16:58 GMT  
		Size: 43.8 MB (43763369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:42d39982209dec20dda4c1a0eb82aa5f7965e10ddf4762b57d79d8a32dc0ad5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75188532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92676457c8f951741aa984be933cefc329a160a810bc49d61775949c32487a82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:42:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:43:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d244ff6bc0f1d8aab1af2badfb1f1ea2f619ca2316288c519afed909e08b35`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.8 MB (3792000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165dd3ed55b51c4b79b3be0051fe345d5b7e6bedbac65941ff7793e50e07420f`  
		Last Modified: Tue, 31 Jan 2023 17:55:31 GMT  
		Size: 3.5 MB (3472764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bdc26d335cd59059e8429dd773b96bf895a6a3ba4f780d1f01410bfcc95406`  
		Last Modified: Tue, 31 Jan 2023 17:55:46 GMT  
		Size: 39.3 MB (39281842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:7d4d71ac75f26b243c8409094b796b8f0a8cc231241262f5babe6d5e7b10309e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:kinetic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3a758ae57c8a7346ba305b53acd626f697ff9eb9f0a1bc2e35ed8aa0fd4090cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.7 MB (258713730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9ffcea5f1bfb263a26234b8ad41d79b047fde2acbf3c33f0f64f7d3e7a27f0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:51:12 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:51:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:51:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:51:13 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:51:14 GMT
ADD file:e886423892b371751386c0ce7147599acb72d8fb528eaaa78092b879d9ff58ce in / 
# Thu, 26 Jan 2023 11:51:15 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:52:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:52:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:55:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62a5d402f83137154c8e54f4f370e9f9f70b5a6892f6ec8cc2fae7be0fd8ae91`  
		Last Modified: Tue, 31 Jan 2023 18:03:39 GMT  
		Size: 27.5 MB (27479169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f8f31e97bc8f200f610260668952e0a909150c1e95f494e3165edd6a4e74d`  
		Last Modified: Tue, 31 Jan 2023 18:03:36 GMT  
		Size: 6.8 MB (6764654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddf4e3936d1208458d4e3e5395b8b86da6f3f7ef3b30242decd50ee0403f1e9`  
		Last Modified: Tue, 31 Jan 2023 18:03:35 GMT  
		Size: 3.6 MB (3635171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b0d398ef08d48d4f39203eb13897978a42e2aa1da1465591c472c03f5975ec`  
		Last Modified: Tue, 31 Jan 2023 18:03:53 GMT  
		Size: 39.7 MB (39740240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01848c64b150b130ec1ae2bc4551ec1f49701b2de7a636fb9197ed2381f48a9`  
		Last Modified: Tue, 31 Jan 2023 18:04:26 GMT  
		Size: 181.1 MB (181094496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:07ca08046c135432af3c0105454a2cb893bf741d6c9275bd43a1fa73d344ae15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.0 MB (221026709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04a755b1a8dff6a40b4cd35245c8f32599ccad2ef814341f3843a5c84ce63d57`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:52:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:52:03 GMT
ADD file:d35c57b0dc2840a8b1ef40f7f6cfd826da68611f1ba37a89a382618c8612b52c in / 
# Thu, 26 Jan 2023 11:52:03 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:56:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:57:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:00:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:697d38f8dfe625e3e751c0b01ddeaaeeff6e8d6f594dd7da227aea3974a49ce1`  
		Last Modified: Thu, 26 Jan 2023 12:14:16 GMT  
		Size: 25.1 MB (25066997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404f4cb6d67c78771ca841794019841127207d81397dddc44c0de7b2a042428`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 5.9 MB (5940499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fa0889fdc983e7d5186fd6c7c7d65241a345cd87db62b962cc1ac632edba88`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 3.8 MB (3800405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cfdc6c62b64f7606245b4e8a795a610e9495fee93fe702f9b6d05ad773b238`  
		Last Modified: Wed, 01 Mar 2023 03:15:50 GMT  
		Size: 42.6 MB (42606983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4061239f68932a6818d689fc46f2f9e4b67bda3c98c4f57d7665d86b78c8c4`  
		Last Modified: Wed, 01 Mar 2023 03:16:21 GMT  
		Size: 143.6 MB (143611825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:75712c8314b8699bf216ddf2252b05b7650004e43c3f63f261d00feb65a3b6a9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.7 MB (246697214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a2c33d0062a7f8588a0cb9df7c0fdd2f82dde2c2faa4468870ad8b74412aa2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:18 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:20 GMT
ADD file:f61617371f6963c6be2852e2b94d04e8507feb8f77e3484c94aa8b9d0ac67f76 in / 
# Thu, 26 Jan 2023 12:08:20 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:23:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:24:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:27:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44d97c2a5ae0fb5d56de8a6242583e80e9265c58a742eb1e52d40264d9f034e9`  
		Last Modified: Tue, 31 Jan 2023 18:35:38 GMT  
		Size: 26.7 MB (26699721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3b285ead03b32399f7eb21eb63769c45b64c8b1731dfc244904cc2e9a8262a`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 6.6 MB (6595500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855afc623fecc9cad347ac6e791b5bb08dd8331201f22400b2764672b1e9a48c`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 3.6 MB (3602406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8fe5b73117b2d29e76fe2d924c4310d621681b761a3e4efcce5bd6842cb3e`  
		Last Modified: Tue, 31 Jan 2023 18:35:51 GMT  
		Size: 39.5 MB (39523097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a13a0356c3c1fefb6afeae0373f345a4200ce0ef8d8c9e383948efc6d1c22d`  
		Last Modified: Tue, 31 Jan 2023 18:36:20 GMT  
		Size: 170.3 MB (170276490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:39314d421779e71395dbf25c5a7c7a6ef6515a692304a576870c50b83b208938
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281283945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1378e98d0d7fb14e25257a0ba00eb60fc2e01ca1b97ceaa7a95eef16b9248db6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:57:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:57:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:57:03 GMT
ADD file:3c2bc98d283cce5149d7992233f5fe644b7239417045faf3f93750b92de5f68e in / 
# Thu, 26 Jan 2023 11:57:04 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:59:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:04:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a06c15ccb04b9b73efad888bdc885d26bd74537d9322b6629f3b3ef906c0756`  
		Last Modified: Tue, 31 Jan 2023 18:18:11 GMT  
		Size: 32.1 MB (32109752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ee7c83faf85e0ce7383151d494b3fbc177d548f264c95b2dcbf49dca2d06d2`  
		Last Modified: Tue, 31 Jan 2023 18:18:05 GMT  
		Size: 7.7 MB (7741886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e688b449cdca40b587631310483952ae87bf319f0b7d13251a6a085f60c05db4`  
		Last Modified: Tue, 31 Jan 2023 18:18:04 GMT  
		Size: 4.4 MB (4362437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecff49481c045e5964caf1cd33337e518465376e603f708da227d433ae19a74c`  
		Last Modified: Tue, 31 Jan 2023 18:18:35 GMT  
		Size: 44.1 MB (44142262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbb04761be0c3739265acca2d4d506ca2d2a045b958a8b9c295a0c33484a051`  
		Last Modified: Tue, 31 Jan 2023 18:19:33 GMT  
		Size: 192.9 MB (192927608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4d1b7f50c9f545d3504d52d8a1cd6dd4a15ce64ab075d2f1955dcef467fc3a47
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228596958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81d546f7822fba9006d358b9d186652f2af4a869ec2464c6c390bd1dd2ef6c9c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:47 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:50 GMT
ADD file:a83afd93816f868be76d243df85b87a66b39d5ef0497c3cb8d0bba2bd4a27c40 in / 
# Thu, 26 Jan 2023 12:08:50 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:45:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:46:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:48:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5bec5e5b1f8afd82addaa8ef129ee5026d804c474c34ca3e565dfa18fa5f877`  
		Last Modified: Tue, 31 Jan 2023 17:56:19 GMT  
		Size: 26.0 MB (26029773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888884268a5ab3f78486597366fa902253286ebe039958a9950d8ab78853d5c5`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 6.5 MB (6457669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7aa7ab93554822a6ee5149dc403f0ba1aa47ed227911574510630a9383bf8f`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 3.6 MB (3625074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173761a853e728963d055e12ba7bf5951b85d93c0ac60955fa793be53aa69f57`  
		Last Modified: Tue, 31 Jan 2023 17:56:31 GMT  
		Size: 39.6 MB (39552159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2930464a0032aa36dbe69f2c0b3faceaa7a67f8de234438b28d703357998a09c`  
		Last Modified: Tue, 31 Jan 2023 17:56:55 GMT  
		Size: 152.9 MB (152932283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:d446c39e8b9aa2eb7699b23def524d291bdc0d5c0fc50556d2123633348b658e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:kinetic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:aee83996c48b86aeb5b790a31fe66a215e9925a3476a210d23b74f1ed7217bc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37878994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154ba55bc0e297c9fb12b70cceafd72e5fb510e6be0838aeac5e673ba3eb83b0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:51:12 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:51:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:51:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:51:13 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:51:14 GMT
ADD file:e886423892b371751386c0ce7147599acb72d8fb528eaaa78092b879d9ff58ce in / 
# Thu, 26 Jan 2023 11:51:15 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:52:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:52:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:62a5d402f83137154c8e54f4f370e9f9f70b5a6892f6ec8cc2fae7be0fd8ae91`  
		Last Modified: Tue, 31 Jan 2023 18:03:39 GMT  
		Size: 27.5 MB (27479169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f8f31e97bc8f200f610260668952e0a909150c1e95f494e3165edd6a4e74d`  
		Last Modified: Tue, 31 Jan 2023 18:03:36 GMT  
		Size: 6.8 MB (6764654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddf4e3936d1208458d4e3e5395b8b86da6f3f7ef3b30242decd50ee0403f1e9`  
		Last Modified: Tue, 31 Jan 2023 18:03:35 GMT  
		Size: 3.6 MB (3635171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:138bf1078343221e08092695ceb35b3b4786103d589ba18af108a037e5f2fb02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34807901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3a38c11fedc1ac56d6be15d7180635f23c3420b28e4c6174b521908a0083a1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:52:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:52:03 GMT
ADD file:d35c57b0dc2840a8b1ef40f7f6cfd826da68611f1ba37a89a382618c8612b52c in / 
# Thu, 26 Jan 2023 11:52:03 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:56:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:697d38f8dfe625e3e751c0b01ddeaaeeff6e8d6f594dd7da227aea3974a49ce1`  
		Last Modified: Thu, 26 Jan 2023 12:14:16 GMT  
		Size: 25.1 MB (25066997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404f4cb6d67c78771ca841794019841127207d81397dddc44c0de7b2a042428`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 5.9 MB (5940499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fa0889fdc983e7d5186fd6c7c7d65241a345cd87db62b962cc1ac632edba88`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 3.8 MB (3800405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:459333d1097d8ab2a535f9c41fd9eff41b7f5820d2c47c0d962e093657486976
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36897627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9f0ccf2c259d8726bab173cdcb0552efa2ef70239be80ab1d4ec8c83bd6a86e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:18 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:20 GMT
ADD file:f61617371f6963c6be2852e2b94d04e8507feb8f77e3484c94aa8b9d0ac67f76 in / 
# Thu, 26 Jan 2023 12:08:20 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:23:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:44d97c2a5ae0fb5d56de8a6242583e80e9265c58a742eb1e52d40264d9f034e9`  
		Last Modified: Tue, 31 Jan 2023 18:35:38 GMT  
		Size: 26.7 MB (26699721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3b285ead03b32399f7eb21eb63769c45b64c8b1731dfc244904cc2e9a8262a`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 6.6 MB (6595500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855afc623fecc9cad347ac6e791b5bb08dd8331201f22400b2764672b1e9a48c`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 3.6 MB (3602406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:055376708ea1867e94b93cf561f8cef6c53ee9ef58b8b61cd47ead6df152da8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44214075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6297083ca03c278a01cf0c0652d9765e62bcb400e73228e55692cf5c25319c77`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:57:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:57:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:57:03 GMT
ADD file:3c2bc98d283cce5149d7992233f5fe644b7239417045faf3f93750b92de5f68e in / 
# Thu, 26 Jan 2023 11:57:04 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:59:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6a06c15ccb04b9b73efad888bdc885d26bd74537d9322b6629f3b3ef906c0756`  
		Last Modified: Tue, 31 Jan 2023 18:18:11 GMT  
		Size: 32.1 MB (32109752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ee7c83faf85e0ce7383151d494b3fbc177d548f264c95b2dcbf49dca2d06d2`  
		Last Modified: Tue, 31 Jan 2023 18:18:05 GMT  
		Size: 7.7 MB (7741886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e688b449cdca40b587631310483952ae87bf319f0b7d13251a6a085f60c05db4`  
		Last Modified: Tue, 31 Jan 2023 18:18:04 GMT  
		Size: 4.4 MB (4362437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:832891dce637dd6a45a4d5349c2792f04ad3f518c1596702561171552b5eb5fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36112516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4326242fb08207106428f6944530b3e0d79c30fcfb112b958bcf78cf90ad2b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:47 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:50 GMT
ADD file:a83afd93816f868be76d243df85b87a66b39d5ef0497c3cb8d0bba2bd4a27c40 in / 
# Thu, 26 Jan 2023 12:08:50 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:45:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a5bec5e5b1f8afd82addaa8ef129ee5026d804c474c34ca3e565dfa18fa5f877`  
		Last Modified: Tue, 31 Jan 2023 17:56:19 GMT  
		Size: 26.0 MB (26029773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888884268a5ab3f78486597366fa902253286ebe039958a9950d8ab78853d5c5`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 6.5 MB (6457669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7aa7ab93554822a6ee5149dc403f0ba1aa47ed227911574510630a9383bf8f`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 3.6 MB (3625074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:9054ceda293660bef628525b88aa77598174bc7a55d364ca2be3c855d7cb69cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:kinetic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5d4e37dd49baaa117ef3d71a175e2b65793fb2ccb4df8a9e401c9b8ee1905393
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77619234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a378bfcf3067410dc87bed8f89e0c492ceb4927beca11af10ffc6f972865637`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:51:12 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:51:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:51:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:51:13 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:51:14 GMT
ADD file:e886423892b371751386c0ce7147599acb72d8fb528eaaa78092b879d9ff58ce in / 
# Thu, 26 Jan 2023 11:51:15 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:52:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:52:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62a5d402f83137154c8e54f4f370e9f9f70b5a6892f6ec8cc2fae7be0fd8ae91`  
		Last Modified: Tue, 31 Jan 2023 18:03:39 GMT  
		Size: 27.5 MB (27479169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f8f31e97bc8f200f610260668952e0a909150c1e95f494e3165edd6a4e74d`  
		Last Modified: Tue, 31 Jan 2023 18:03:36 GMT  
		Size: 6.8 MB (6764654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddf4e3936d1208458d4e3e5395b8b86da6f3f7ef3b30242decd50ee0403f1e9`  
		Last Modified: Tue, 31 Jan 2023 18:03:35 GMT  
		Size: 3.6 MB (3635171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b0d398ef08d48d4f39203eb13897978a42e2aa1da1465591c472c03f5975ec`  
		Last Modified: Tue, 31 Jan 2023 18:03:53 GMT  
		Size: 39.7 MB (39740240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:df9482f8aafc2f7b4abf8e2fff63de1427eae9c4e93ef78925b89c7207497450
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.4 MB (77414884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27db2823f44839863528aacd8914aa05e7f260dbb2373b0ffab72dcc1f60457f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:52:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:52:03 GMT
ADD file:d35c57b0dc2840a8b1ef40f7f6cfd826da68611f1ba37a89a382618c8612b52c in / 
# Thu, 26 Jan 2023 11:52:03 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 02:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:56:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:57:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:697d38f8dfe625e3e751c0b01ddeaaeeff6e8d6f594dd7da227aea3974a49ce1`  
		Last Modified: Thu, 26 Jan 2023 12:14:16 GMT  
		Size: 25.1 MB (25066997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404f4cb6d67c78771ca841794019841127207d81397dddc44c0de7b2a042428`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 5.9 MB (5940499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fa0889fdc983e7d5186fd6c7c7d65241a345cd87db62b962cc1ac632edba88`  
		Last Modified: Wed, 01 Mar 2023 03:15:33 GMT  
		Size: 3.8 MB (3800405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cfdc6c62b64f7606245b4e8a795a610e9495fee93fe702f9b6d05ad773b238`  
		Last Modified: Wed, 01 Mar 2023 03:15:50 GMT  
		Size: 42.6 MB (42606983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7122957b9251055a81faead01a15fbd23d457f0f694320c75c72e167bae939c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76420724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1a7465b31ec6c65ee04ea8cd0b6fcb28a729ef78f9c54f094a85d16eb4d7e84`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:18 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:20 GMT
ADD file:f61617371f6963c6be2852e2b94d04e8507feb8f77e3484c94aa8b9d0ac67f76 in / 
# Thu, 26 Jan 2023 12:08:20 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:23:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:24:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:24:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44d97c2a5ae0fb5d56de8a6242583e80e9265c58a742eb1e52d40264d9f034e9`  
		Last Modified: Tue, 31 Jan 2023 18:35:38 GMT  
		Size: 26.7 MB (26699721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3b285ead03b32399f7eb21eb63769c45b64c8b1731dfc244904cc2e9a8262a`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 6.6 MB (6595500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855afc623fecc9cad347ac6e791b5bb08dd8331201f22400b2764672b1e9a48c`  
		Last Modified: Tue, 31 Jan 2023 18:35:35 GMT  
		Size: 3.6 MB (3602406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8fe5b73117b2d29e76fe2d924c4310d621681b761a3e4efcce5bd6842cb3e`  
		Last Modified: Tue, 31 Jan 2023 18:35:51 GMT  
		Size: 39.5 MB (39523097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a92b717633421c919c8437841cec0c8fe13b56c6c1448937c07a7f37c01a7ebb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88356337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c053aa26c6dbf33d593218945dffc872660a52734291c7d1b459c175ecdcfb05`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:57:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:57:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:57:03 GMT
ADD file:3c2bc98d283cce5149d7992233f5fe644b7239417045faf3f93750b92de5f68e in / 
# Thu, 26 Jan 2023 11:57:04 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:59:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 18:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a06c15ccb04b9b73efad888bdc885d26bd74537d9322b6629f3b3ef906c0756`  
		Last Modified: Tue, 31 Jan 2023 18:18:11 GMT  
		Size: 32.1 MB (32109752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ee7c83faf85e0ce7383151d494b3fbc177d548f264c95b2dcbf49dca2d06d2`  
		Last Modified: Tue, 31 Jan 2023 18:18:05 GMT  
		Size: 7.7 MB (7741886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e688b449cdca40b587631310483952ae87bf319f0b7d13251a6a085f60c05db4`  
		Last Modified: Tue, 31 Jan 2023 18:18:04 GMT  
		Size: 4.4 MB (4362437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecff49481c045e5964caf1cd33337e518465376e603f708da227d433ae19a74c`  
		Last Modified: Tue, 31 Jan 2023 18:18:35 GMT  
		Size: 44.1 MB (44142262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8aa73932942674acc171a5ab84eec601e912cf168a5949af6fbbd9b42e1b0114
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75664675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f39289322452926c88ff808fa932fca05a4903be6317283d1fe28e26c0fc154`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:47 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:50 GMT
ADD file:a83afd93816f868be76d243df85b87a66b39d5ef0497c3cb8d0bba2bd4a27c40 in / 
# Thu, 26 Jan 2023 12:08:50 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:45:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Jan 2023 17:46:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5bec5e5b1f8afd82addaa8ef129ee5026d804c474c34ca3e565dfa18fa5f877`  
		Last Modified: Tue, 31 Jan 2023 17:56:19 GMT  
		Size: 26.0 MB (26029773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888884268a5ab3f78486597366fa902253286ebe039958a9950d8ab78853d5c5`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 6.5 MB (6457669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7aa7ab93554822a6ee5149dc403f0ba1aa47ed227911574510630a9383bf8f`  
		Last Modified: Tue, 31 Jan 2023 17:56:16 GMT  
		Size: 3.6 MB (3625074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173761a853e728963d055e12ba7bf5951b85d93c0ac60955fa793be53aa69f57`  
		Last Modified: Tue, 31 Jan 2023 17:56:31 GMT  
		Size: 39.6 MB (39552159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:6fc33b1f1bc5e9d66a7cbbaab3f0de66bcdfee49fc51cdd7a1abe8f9e93a1640
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:latest` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1ab51e666d5331b2ca90421dc657968b50de8c4ea86e747b51f24b0ceac6ee20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322486156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f6175124be93225950f0f44661e6d04c099685b1c6cfdce98c94b6908a005ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:43:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:44:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cdcd4942ebc7445d8a70117a83ecbc77dcc5ffc72c4b6f8e24c0c76cfee15d`  
		Last Modified: Wed, 01 Mar 2023 04:50:33 GMT  
		Size: 54.6 MB (54585443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3bce705f6c47c25b6e7896b4da514bf271c5827b1d19f51611c4a149dd713c`  
		Last Modified: Wed, 01 Mar 2023 04:51:08 GMT  
		Size: 196.8 MB (196811476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d5ebd7b5044f44ae29cf2301dc9d211d4a91de578f8643d9447e2705c89e1fa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295543491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25085575e82e41137aadeab7abf493a22196af92d25adbdd636b34ea590b35b8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:18:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:20:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d373aa541f88e7c81c88d63aca3fd07f01c6220ca295915af87f489a6cb251`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 5.1 MB (5072694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c176fe3230b5050ab13f5cd081fa601f679459e28449694496136a73bddd175c`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 10.6 MB (10573876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04072817b27c20dd9a7f9a0b93816bd195f8675845e235c0291c0f935824f610`  
		Last Modified: Wed, 01 Mar 2023 02:25:18 GMT  
		Size: 52.3 MB (52338815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6353168632306a6374c103fef267a9c6d96bb6102c9ad2cf73bbcd81093088a0`  
		Last Modified: Wed, 01 Mar 2023 02:25:56 GMT  
		Size: 175.0 MB (175008286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:68a9f7cc0785c70372cb8a12f4c245fc83255dabf264e6be54ff359ed27e2a40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (283008511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0390df189979c07f1a2462cc444b49d2112865ac9a6a1631e580a27b55539b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:33:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e676c4187d9dd900add9c8dd4b9c906be40a2b8db6cabfdaf280ac2e83cdfca`  
		Last Modified: Wed, 01 Mar 2023 03:09:35 GMT  
		Size: 50.4 MB (50355863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df966bf734b2531648679fbd424ead324e0892e75539a7b995ac958175ebd568`  
		Last Modified: Wed, 01 Mar 2023 03:10:10 GMT  
		Size: 167.3 MB (167288237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8917040dd4bb6aedfddba59aa82d51536b6ec25930b6f06c9733532a61912af2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.1 MB (314133809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2780396f13c4cbb69cfd74d843bc7bf52d0e90e5d9d9802e537a1a9769446f3a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8747d4a988af1d119e668971a87213d5c7061fc04671ba6fcb7123a1c11507ac`  
		Last Modified: Wed, 01 Mar 2023 02:56:37 GMT  
		Size: 54.7 MB (54676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb701404a7a0229719104b05970d81ecf0a7dea50b3defe137088db6cc3c0d0c`  
		Last Modified: Wed, 01 Mar 2023 02:57:06 GMT  
		Size: 189.7 MB (189727959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:151857e29bb1821d712ec7cfd8e4d8a5d883f37adea2a83c01a48cc2ac69239f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.2 MB (328218457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:038aa1836a9a96ce7b81933a91fa4831e0ba0d768de322b4835e86368581db36`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:10:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471482ade37b25d9ec22336d057dd4ed265a030b98595eac314b56d5709bbdff`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 5.3 MB (5293673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a995bf7fa061158e93790e264fd3bc4a3340e75bf857b3c51814384b5f1344f5`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 11.2 MB (11249844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9955e6ae7dba34d1170876e13f1c83b049619255f38babb22074d26848658318`  
		Last Modified: Wed, 01 Mar 2023 02:23:54 GMT  
		Size: 55.9 MB (55922655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc50efa640196b1840993873638e42246a1137dc3e2ac3534d6cba803fef33f`  
		Last Modified: Wed, 01 Mar 2023 02:24:42 GMT  
		Size: 199.7 MB (199724209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5ea0d35f075afa10f4b0b4cc10b69f2acc8c18ce4089182ad36a944bc68e2d38
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.2 MB (301151652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0222370846c985596fd3058856c6c93024191a6b9fc9adfbf00825509403dfbd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:42:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:47:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791a92fb38ebf78f5ed530cc39361869dd25ce941ea09d0580b866204f0e8e1`  
		Last Modified: Thu, 09 Feb 2023 07:59:50 GMT  
		Size: 4.9 MB (4921594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c347eddc487950d631dca4e7c20c1165566e8418703435fad325a721c0e8d`  
		Last Modified: Thu, 09 Feb 2023 07:59:52 GMT  
		Size: 10.7 MB (10662160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9ee56dfe2667a1d6574684709026d72883d1af28301257038f732b76362e9a`  
		Last Modified: Thu, 09 Feb 2023 08:00:40 GMT  
		Size: 53.3 MB (53307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec8851fe07613cc20ef37a5c4e83efee0eba7c47c653df09be97f187753970`  
		Last Modified: Thu, 09 Feb 2023 08:02:44 GMT  
		Size: 179.0 MB (178993425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bc66949fb3e5bb8519171d6c99462250e7c90213077a00562f8da2ad7567fdd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330990552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e22aacee9f5e429288440511032e88b59ac9b6015c67ad2859a1549cfdc03f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:01 GMT
ADD file:40523b7b16ccf1ff245b11e11f92d24e9e6e9dfbdbc755d4361cf55c7ec26244 in / 
# Wed, 01 Mar 2023 04:47:11 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:25:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:26:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:30:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b7949e1acd104233f80137ab3a92a148b0d48e41b3075c70a2d636c3b4c60bf`  
		Last Modified: Wed, 01 Mar 2023 04:53:18 GMT  
		Size: 58.9 MB (58921304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b3574e90831068a9bd9f64e57da92a087d925f0a0e63c764ecf421b18d3a1`  
		Last Modified: Wed, 01 Mar 2023 05:39:22 GMT  
		Size: 5.4 MB (5415247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8bec1f2d073d24de5e7dd051bcada4f0a407fc713e38b49fc2d2a863bde38e`  
		Last Modified: Wed, 01 Mar 2023 05:39:23 GMT  
		Size: 11.6 MB (11629925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3bc8a98c359709356de5d552e69a43170d7f81b4ad5ac17cfbb0eb8d3da2b1`  
		Last Modified: Wed, 01 Mar 2023 05:39:53 GMT  
		Size: 58.9 MB (58863932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266ad73c7e2640ed2a8bd13bc5ae4a7289e4d94678b520531d6e6a4c628b4936`  
		Last Modified: Wed, 01 Mar 2023 05:40:52 GMT  
		Size: 196.2 MB (196160144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8ced439af7f8f74e519890670464e8a54d02445b50906c0a580cb23381403b74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296068375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be656e6f4f9d501e5be96387e4ee7f13eed0dda7e92ac3582f1ba01b78338d6b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:07 GMT
ADD file:e5f01d8f88c8134571e8998672a504ecad259a9a8322df73aed4a93ffac08ebd in / 
# Wed, 01 Mar 2023 02:50:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:14:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:16:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51f6de0debe6daa552b12c9951f6529a870979d923187c1ba62ff66cee3450ac`  
		Last Modified: Wed, 01 Mar 2023 02:54:25 GMT  
		Size: 53.3 MB (53277694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6404e912b557d72a71a982115ad4b92e1c23918b7f0c950f6f22c2ec775ff936`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 5.1 MB (5149110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0561ee66ff6ae2ce12d922c3d0fed94e18a801571a2add9e526e914cb30a3bab`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 10.8 MB (10765987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c7ccf7cb532de1600bce9245b8e167d6d644608677c26601c246c4e80cdbf`  
		Last Modified: Wed, 01 Mar 2023 03:22:28 GMT  
		Size: 54.1 MB (54060191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2854c5c8fd871ba1d0f27ad51f05fba4d434683959e10cbe9fc7fb3281ec3415`  
		Last Modified: Wed, 01 Mar 2023 03:22:56 GMT  
		Size: 172.8 MB (172815393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar`

```console
$ docker pull buildpack-deps@sha256:b6c8f6bfaf6ebc9ffa3ac4a7f91829fd0b1040f3fb14d470c045c693ddec41e7
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
$ docker pull buildpack-deps@sha256:6afd26c62d559b4fa71aa25b11d68f20128236eba753b8c8b78c82048a01ee7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.3 MB (258330292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44a9ffc7d1ca5998e864650d5669556b2dd055296fb3a8a33b7a2c8f13aff074`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:15:52 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:15:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:15:54 GMT
ADD file:915f1a27db0a8b9a9dd58d40086cb7d45b2722e8ceb29ed8bcb306d4dcd3688e in / 
# Sat, 28 Jan 2023 05:15:54 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:12:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:21:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7610e15a5bf822d71b65f5f7c7d873b70f585cebc9b4bfd76dedd61997f9e1c2`  
		Last Modified: Wed, 01 Feb 2023 18:23:55 GMT  
		Size: 27.4 MB (27419700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc4589b98247ebd93b0b4ca6c08ebf74c1fcb7fe81d1ee3a00ddd0381b99aaa`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 6.6 MB (6635143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c87abeb95cddddf017930e8ffec58593bd520216c779b25e710376682a56c6`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 3.7 MB (3690296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b97131389bee769ba93a32a51aee8b1f6fa2936b506cd9be1296fe2e9ef3d`  
		Last Modified: Wed, 01 Feb 2023 18:24:10 GMT  
		Size: 40.9 MB (40948895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dba4cd6fa73d5141eb96b8088c1a0ab5efb6125eb26b9aab86cca0e7f172ec`  
		Last Modified: Wed, 01 Feb 2023 18:24:44 GMT  
		Size: 179.6 MB (179636258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4c79aad28f82a6612c1d9a32df92cce9c2e7498061c8c485b2fe2554f851e965
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.7 MB (244651591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f73b6dab560b07c846121f5172e0c5f76c67989f848e3ec9d236d0d695dd93`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:25 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:31 GMT
ADD file:c0ac354f01ba9deb72bda06f4368650e0cc3ad5c3425ce0eb452561b56a1734a in / 
# Sat, 28 Jan 2023 05:11:32 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 03:01:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:01:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:02:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:05:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2cf733a376b355703d852c37fb66314a9d27adeb140641f229bd7d5b089c8ef7`  
		Last Modified: Sat, 28 Jan 2023 05:21:37 GMT  
		Size: 25.1 MB (25086001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8391c317b70a65f7c7d5bf15686f27d06e2c79b286c3a86cb70987de2acdc4`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 5.8 MB (5808831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd77c8b93dd4f4c7b1af018a1de3fc89606fac50a049b8ee85bd1ccd0335294`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 3.9 MB (3851906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9367c233564b3534a29ad60c3843f0bbd6a4105cc65519f48f91cf119358142`  
		Last Modified: Wed, 01 Mar 2023 03:16:51 GMT  
		Size: 48.6 MB (48602279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c639059702b5fc046342922b5b562597eb8ec1d3fa1484357d33845656e117`  
		Last Modified: Wed, 01 Mar 2023 03:17:23 GMT  
		Size: 161.3 MB (161302574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:914aa413772a5b51585daf8e054b1c90924bb20dcbdb32ef75d72152a9944578
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.4 MB (248385791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16afca163301c787bfd70226721890aa01ca555f65875af6e8202e1d5747985`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:24 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:29 GMT
ADD file:c6e9b4142d0eef696dbc592460bdbd505f41a98d02ba1c7a84caedbb5f84ea1b in / 
# Sat, 28 Jan 2023 05:11:29 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:09:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:10:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:10:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:14:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86b4004853063d73760cb92de14cb3a62665a38c8761227cbb1afdd83e3c2463`  
		Last Modified: Wed, 01 Feb 2023 18:16:40 GMT  
		Size: 26.8 MB (26755970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabf667a5a78f05803b7cfc5334c39586cc72c5e9f5c4b3d057eeaeae60adab9`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 6.5 MB (6468704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f5bbd1102042fd3e0960b145074562a58c2191adc81cbc46fe1f667ee5e5c`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 3.6 MB (3649392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c999a4e8e593fbc5591306b84b879ccd3dede542421a341ded4ce652345c0`  
		Last Modified: Wed, 01 Feb 2023 18:16:53 GMT  
		Size: 40.8 MB (40753202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c74342ec10c904450e8a7bee3d119d1a5124a8e306607a703ca2006f59e5d7`  
		Last Modified: Wed, 01 Feb 2023 18:17:20 GMT  
		Size: 170.8 MB (170758523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:863b48e351486104089d5665e2d2889a5c29940e2995df5037567c62cac0ee36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (282968437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3738e6e9ee8b954e2cb450930080810a2d809f552328fbfddf8a9ad3ee09e2c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:09:15 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:09:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:09:19 GMT
ADD file:1c6ae50eb1e182a9aa8f750f61a615d5b3578b7c2f94e58678359bf1f43d3780 in / 
# Sat, 28 Jan 2023 05:09:19 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:17:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5151cf1d3445f8b719163cb88c8ee7f7f2368e309dd1d14016546804fc05126`  
		Last Modified: Wed, 01 Feb 2023 18:22:34 GMT  
		Size: 32.0 MB (31980199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337c3408ba6fc96792e39145bb0a122a3f04a96a5571d97c3f265402359009c`  
		Last Modified: Wed, 01 Feb 2023 18:22:28 GMT  
		Size: 7.6 MB (7605406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1579dbb09dc76707e4839919fcec93b48be4479e103cb1aeed1a50194d1724e8`  
		Last Modified: Wed, 01 Feb 2023 18:22:27 GMT  
		Size: 4.4 MB (4408979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f651ad714aac8d2542de9fc23ff6b10701efb943ac6c9538ea45be37d726bf0e`  
		Last Modified: Wed, 01 Feb 2023 18:22:57 GMT  
		Size: 45.7 MB (45720315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd9b71849d33f1ac6239db3ee29c7575dcc37fb97cfb76c27f3f0ef8754c45f`  
		Last Modified: Wed, 01 Feb 2023 18:23:55 GMT  
		Size: 193.3 MB (193253538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5a1dac520bcbb95170725e4974c5d3e58177a10b865930b4b7e3fd2f0289b52f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (229954138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:461ca2b8a46d2de7d07b24d64eb0ab47dea82cf2629e45bf12fb050bc95c69f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:10:10 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:10:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:10:12 GMT
ADD file:b85f8b675931991dc4361ad29563c508e8cdd381491f1da64b998d7742f72c42 in / 
# Sat, 28 Jan 2023 05:10:12 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:15:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:16:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:18:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ec11bba63863786b2862fe78b2d89ce7f2cf2ab178c9abc17064e250fc6a07b`  
		Last Modified: Wed, 01 Feb 2023 18:22:06 GMT  
		Size: 26.0 MB (26014630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50701e4538cb519cc258f9f917c69bd16c143f281ac369a90c6aba3f40dcff3`  
		Last Modified: Wed, 01 Feb 2023 18:22:04 GMT  
		Size: 6.3 MB (6318048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c474c2328ae2c175dbac9c35c888383f82da2ae100c9197db0e3a1912be9dd3e`  
		Last Modified: Wed, 01 Feb 2023 18:22:03 GMT  
		Size: 3.7 MB (3674786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eabce57ad05a030ae2bc38b37ffdb539eef43109d4503a2b66e82f71391c9bb`  
		Last Modified: Wed, 01 Feb 2023 18:22:20 GMT  
		Size: 40.7 MB (40730894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b71b0b4891fc62494cfff677b3e282387e98f36b19733cec13dccdae9ab15`  
		Last Modified: Wed, 01 Feb 2023 18:22:49 GMT  
		Size: 153.2 MB (153215780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-curl`

```console
$ docker pull buildpack-deps@sha256:f1e3051d65bd5ac55c65d52254eba29ff0f754b0e6bced73d7224f3e8ea2e3bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:537eea6319443a5bc614bfb7b4e5cdbcfc9e13586c211abcc852eea86d07d663
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37745139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed4daa4196e32ecf36c1e23528d2d324d3d143e881960c908c9b58ddf0fc25f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:15:52 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:15:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:15:54 GMT
ADD file:915f1a27db0a8b9a9dd58d40086cb7d45b2722e8ceb29ed8bcb306d4dcd3688e in / 
# Sat, 28 Jan 2023 05:15:54 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:12:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7610e15a5bf822d71b65f5f7c7d873b70f585cebc9b4bfd76dedd61997f9e1c2`  
		Last Modified: Wed, 01 Feb 2023 18:23:55 GMT  
		Size: 27.4 MB (27419700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc4589b98247ebd93b0b4ca6c08ebf74c1fcb7fe81d1ee3a00ddd0381b99aaa`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 6.6 MB (6635143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c87abeb95cddddf017930e8ffec58593bd520216c779b25e710376682a56c6`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 3.7 MB (3690296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:83263b17a9332b259200af03feb6a20687800485d75e356abdd7e5b2fbb00e5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34746738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f4d40d7a0e65028a158d83cba12d690f50604a982fdde14ea99f2ce6fdf4f3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:25 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:31 GMT
ADD file:c0ac354f01ba9deb72bda06f4368650e0cc3ad5c3425ce0eb452561b56a1734a in / 
# Sat, 28 Jan 2023 05:11:32 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 03:01:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:01:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2cf733a376b355703d852c37fb66314a9d27adeb140641f229bd7d5b089c8ef7`  
		Last Modified: Sat, 28 Jan 2023 05:21:37 GMT  
		Size: 25.1 MB (25086001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8391c317b70a65f7c7d5bf15686f27d06e2c79b286c3a86cb70987de2acdc4`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 5.8 MB (5808831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd77c8b93dd4f4c7b1af018a1de3fc89606fac50a049b8ee85bd1ccd0335294`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 3.9 MB (3851906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c3edb731722f1b63d480271e6f2aaebf090d64c312181d330c9cd0a0e59ca25a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36874066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba32c939dfad52832eb293c54966c05a6b6d0096a74522b05bb10a2b9e0794fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:24 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:29 GMT
ADD file:c6e9b4142d0eef696dbc592460bdbd505f41a98d02ba1c7a84caedbb5f84ea1b in / 
# Sat, 28 Jan 2023 05:11:29 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:09:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:10:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:86b4004853063d73760cb92de14cb3a62665a38c8761227cbb1afdd83e3c2463`  
		Last Modified: Wed, 01 Feb 2023 18:16:40 GMT  
		Size: 26.8 MB (26755970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabf667a5a78f05803b7cfc5334c39586cc72c5e9f5c4b3d057eeaeae60adab9`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 6.5 MB (6468704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f5bbd1102042fd3e0960b145074562a58c2191adc81cbc46fe1f667ee5e5c`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 3.6 MB (3649392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2689fc68d1712090df249e5b92394fd8e147aa8e4b4f419a4849f377c21814cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43994584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:706de3f8b9b6b3b56436cd6c5541d09d59ab09b125fc6596f1b13d0ca35e3c3a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:09:15 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:09:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:09:19 GMT
ADD file:1c6ae50eb1e182a9aa8f750f61a615d5b3578b7c2f94e58678359bf1f43d3780 in / 
# Sat, 28 Jan 2023 05:09:19 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a5151cf1d3445f8b719163cb88c8ee7f7f2368e309dd1d14016546804fc05126`  
		Last Modified: Wed, 01 Feb 2023 18:22:34 GMT  
		Size: 32.0 MB (31980199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337c3408ba6fc96792e39145bb0a122a3f04a96a5571d97c3f265402359009c`  
		Last Modified: Wed, 01 Feb 2023 18:22:28 GMT  
		Size: 7.6 MB (7605406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1579dbb09dc76707e4839919fcec93b48be4479e103cb1aeed1a50194d1724e8`  
		Last Modified: Wed, 01 Feb 2023 18:22:27 GMT  
		Size: 4.4 MB (4408979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ade0a2429605778da48e86e85150f3bde89379b8572cc40bc9e5b466ddfe2d4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36007464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f4f980c08a961d5e32890459371417c50d867990d96e3ba9fbf9de7ce406ea8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:10:10 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:10:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:10:12 GMT
ADD file:b85f8b675931991dc4361ad29563c508e8cdd381491f1da64b998d7742f72c42 in / 
# Sat, 28 Jan 2023 05:10:12 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:15:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2ec11bba63863786b2862fe78b2d89ce7f2cf2ab178c9abc17064e250fc6a07b`  
		Last Modified: Wed, 01 Feb 2023 18:22:06 GMT  
		Size: 26.0 MB (26014630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50701e4538cb519cc258f9f917c69bd16c143f281ac369a90c6aba3f40dcff3`  
		Last Modified: Wed, 01 Feb 2023 18:22:04 GMT  
		Size: 6.3 MB (6318048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c474c2328ae2c175dbac9c35c888383f82da2ae100c9197db0e3a1912be9dd3e`  
		Last Modified: Wed, 01 Feb 2023 18:22:03 GMT  
		Size: 3.7 MB (3674786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:606403063d0774c59bdfdf8cec41792762059428f2335758b767a8a6419d131e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f4779bb631cc96f8c601cb3cb2d4d19fc819689d534b0ec2049fb2aeb96b7e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.7 MB (78694034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90cccf588560d124231ebdcf5f275b4e27dbb214d9bf110989c70b375d2885f9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:15:52 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:15:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:15:52 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:15:54 GMT
ADD file:915f1a27db0a8b9a9dd58d40086cb7d45b2722e8ceb29ed8bcb306d4dcd3688e in / 
# Sat, 28 Jan 2023 05:15:54 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:12:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7610e15a5bf822d71b65f5f7c7d873b70f585cebc9b4bfd76dedd61997f9e1c2`  
		Last Modified: Wed, 01 Feb 2023 18:23:55 GMT  
		Size: 27.4 MB (27419700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc4589b98247ebd93b0b4ca6c08ebf74c1fcb7fe81d1ee3a00ddd0381b99aaa`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 6.6 MB (6635143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c87abeb95cddddf017930e8ffec58593bd520216c779b25e710376682a56c6`  
		Last Modified: Wed, 01 Feb 2023 18:23:52 GMT  
		Size: 3.7 MB (3690296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b97131389bee769ba93a32a51aee8b1f6fa2936b506cd9be1296fe2e9ef3d`  
		Last Modified: Wed, 01 Feb 2023 18:24:10 GMT  
		Size: 40.9 MB (40948895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:049d82e7a50c297020943bab44d6ae17ffc80d524d72a34544bdffde74443213
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83349017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbaabfc7bbbedab1780b20eaee19155a1c5b9ebf58df1fc9f4f1df55b732b84e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:25 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:31 GMT
ADD file:c0ac354f01ba9deb72bda06f4368650e0cc3ad5c3425ce0eb452561b56a1734a in / 
# Sat, 28 Jan 2023 05:11:32 GMT
CMD ["/bin/bash"]
# Wed, 01 Mar 2023 03:01:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:01:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:02:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2cf733a376b355703d852c37fb66314a9d27adeb140641f229bd7d5b089c8ef7`  
		Last Modified: Sat, 28 Jan 2023 05:21:37 GMT  
		Size: 25.1 MB (25086001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8391c317b70a65f7c7d5bf15686f27d06e2c79b286c3a86cb70987de2acdc4`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 5.8 MB (5808831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd77c8b93dd4f4c7b1af018a1de3fc89606fac50a049b8ee85bd1ccd0335294`  
		Last Modified: Wed, 01 Mar 2023 03:16:32 GMT  
		Size: 3.9 MB (3851906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9367c233564b3534a29ad60c3843f0bbd6a4105cc65519f48f91cf119358142`  
		Last Modified: Wed, 01 Mar 2023 03:16:51 GMT  
		Size: 48.6 MB (48602279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:42463b1fa0a388d9801a062d9dd40ea8d72b288e886e5dd7ace63d7c8e99274a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77627268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9d5f1d5f2a4e64bbe95c49ca9314c9030fdcc07106445d0f6c7fa7d59d897a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:11:24 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:11:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:11:25 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:11:29 GMT
ADD file:c6e9b4142d0eef696dbc592460bdbd505f41a98d02ba1c7a84caedbb5f84ea1b in / 
# Sat, 28 Jan 2023 05:11:29 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:09:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:10:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:10:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86b4004853063d73760cb92de14cb3a62665a38c8761227cbb1afdd83e3c2463`  
		Last Modified: Wed, 01 Feb 2023 18:16:40 GMT  
		Size: 26.8 MB (26755970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabf667a5a78f05803b7cfc5334c39586cc72c5e9f5c4b3d057eeaeae60adab9`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 6.5 MB (6468704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f5bbd1102042fd3e0960b145074562a58c2191adc81cbc46fe1f667ee5e5c`  
		Last Modified: Wed, 01 Feb 2023 18:16:38 GMT  
		Size: 3.6 MB (3649392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c999a4e8e593fbc5591306b84b879ccd3dede542421a341ded4ce652345c0`  
		Last Modified: Wed, 01 Feb 2023 18:16:53 GMT  
		Size: 40.8 MB (40753202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a805a109b7caa13d3e7983ef1c11492c18454c10000ddc6c90fc09528e3427ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89714899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76476df3dde3cb0032f781c70db091e82cc22df5fee40845b4036edc34bda10d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:09:15 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:09:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:09:16 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:09:19 GMT
ADD file:1c6ae50eb1e182a9aa8f750f61a615d5b3578b7c2f94e58678359bf1f43d3780 in / 
# Sat, 28 Jan 2023 05:09:19 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:11:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:11:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5151cf1d3445f8b719163cb88c8ee7f7f2368e309dd1d14016546804fc05126`  
		Last Modified: Wed, 01 Feb 2023 18:22:34 GMT  
		Size: 32.0 MB (31980199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337c3408ba6fc96792e39145bb0a122a3f04a96a5571d97c3f265402359009c`  
		Last Modified: Wed, 01 Feb 2023 18:22:28 GMT  
		Size: 7.6 MB (7605406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1579dbb09dc76707e4839919fcec93b48be4479e103cb1aeed1a50194d1724e8`  
		Last Modified: Wed, 01 Feb 2023 18:22:27 GMT  
		Size: 4.4 MB (4408979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f651ad714aac8d2542de9fc23ff6b10701efb943ac6c9538ea45be37d726bf0e`  
		Last Modified: Wed, 01 Feb 2023 18:22:57 GMT  
		Size: 45.7 MB (45720315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:288d9bb7ed13a2a668f51e523fa6f73bb6cd8611fb7903414940a9b02618f78d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.7 MB (76738358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5814b74a158bb3239700bd17ecef82d37a7e245364d85b0f074b6e447ba0d37a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 28 Jan 2023 05:10:10 GMT
ARG RELEASE
# Sat, 28 Jan 2023 05:10:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 28 Jan 2023 05:10:10 GMT
LABEL org.opencontainers.image.version=23.04
# Sat, 28 Jan 2023 05:10:12 GMT
ADD file:b85f8b675931991dc4361ad29563c508e8cdd381491f1da64b998d7742f72c42 in / 
# Sat, 28 Jan 2023 05:10:12 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:15:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Feb 2023 18:16:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ec11bba63863786b2862fe78b2d89ce7f2cf2ab178c9abc17064e250fc6a07b`  
		Last Modified: Wed, 01 Feb 2023 18:22:06 GMT  
		Size: 26.0 MB (26014630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50701e4538cb519cc258f9f917c69bd16c143f281ac369a90c6aba3f40dcff3`  
		Last Modified: Wed, 01 Feb 2023 18:22:04 GMT  
		Size: 6.3 MB (6318048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c474c2328ae2c175dbac9c35c888383f82da2ae100c9197db0e3a1912be9dd3e`  
		Last Modified: Wed, 01 Feb 2023 18:22:03 GMT  
		Size: 3.7 MB (3674786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eabce57ad05a030ae2bc38b37ffdb539eef43109d4503a2b66e82f71391c9bb`  
		Last Modified: Wed, 01 Feb 2023 18:22:20 GMT  
		Size: 40.7 MB (40730894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:63be0fe0bfb9d06b8747dcd87683787ef6d82c6f05b8a2ae213c38d56dc2bf53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d836de599cb6f6ae477b9fd28a1439b9ee0a26d805a2be9fec1aeb7df5256811
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.1 MB (312112050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd092f9559e9c632d4ce17e2cc3a5a87d8bfe07663f67c5416f5cadf4a9b23a6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:44:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:44:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:44:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:46:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fc05781c9a4a3dee77723abf708dd674020a00d7d57dd6cc1f9bc72da96143`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 7.9 MB (7862980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efc3ea86e67ce8cdce1cf3619f311735cbbb8744a1c69536f8a390d014c0a99`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 10.0 MB (10001392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47452733a7c0712961d7ef8b48e3d823328f056af1c90c715966748b137b3d1c`  
		Last Modified: Wed, 01 Mar 2023 04:51:39 GMT  
		Size: 51.9 MB (51873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f68a3641163543e513f65bb04fd6c440c0569b7f3e0cf3c3735a5718cb42169`  
		Last Modified: Wed, 01 Mar 2023 04:52:10 GMT  
		Size: 191.9 MB (191924876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8203a9192ea844c6cb0f1f395cd6baa1f8db1c36605c92ca4392a817bcfaf81d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.9 MB (277910034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a08160c6fdb784988b93c2bdf8eead75a0af2edffc9c3bc13ffe5e54839098`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:03 GMT
ADD file:28e7414281fcd12661d43cccdf7062bf4aa15641f986cae3aa3260fcb8e16bb5 in / 
# Wed, 01 Mar 2023 01:58:03 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:34:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:34:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:34:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:36:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ba30d485dd0583b3079a70184a97c458599a0629e661b1382394653cb802242`  
		Last Modified: Wed, 01 Mar 2023 02:03:25 GMT  
		Size: 45.9 MB (45916077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5b3ed640e906ad20c2a86568f52c60a48e1d82e4654d3378280f572737f7c1`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 7.2 MB (7152340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028b21e39d17f6632c7b82f0c900d32b50233b13940a7a60009782a6abc32cdd`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 9.3 MB (9349019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35297b6d570293c7581e727c51353a6eb15d3b2f7bdaf391595c28c2a8d4fc6`  
		Last Modified: Wed, 01 Mar 2023 03:10:43 GMT  
		Size: 47.4 MB (47396639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db985543ef8399c92c217abd234865cfb8fc38d73e04bede21a4921385745eae`  
		Last Modified: Wed, 01 Mar 2023 03:11:15 GMT  
		Size: 168.1 MB (168095959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:142ad5211953587c7ba8af3681096fee98c692d6b3c9edaf36daac5e1eb477e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302666222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf2cd8921f2ed4913a5a1f9d79c8b6ef3776901ad259d2e10a0e271e66bb1d25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:50:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:51:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:52:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a788623352140f16227efacfe9a8b497cf91ee63fa69554615640474975ca5`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 7.7 MB (7731356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12086fb08985806514ae1e77eef44a12e303bd44b113e62dac28b16b778fc797`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 10.0 MB (10003642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afc4bf76406adbdc8533ba0c416f2aac77ca7db02bb6d380eaeeb778f56c5d4`  
		Last Modified: Wed, 01 Mar 2023 02:57:32 GMT  
		Size: 52.2 MB (52192055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7fd78b041bf9263b5362da19c99f8256c7954621d32679777cd6fcd99d86a`  
		Last Modified: Wed, 01 Mar 2023 02:57:57 GMT  
		Size: 183.5 MB (183499167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d05278970db620073bd62426cdb4d4dc191128f0fd30eb30b0d260b452482119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.5 MB (321526216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95d43e15f63c3b2bafcd52b42a1a9f683924f8208cec5e19fb9dac302ee4a1b1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:23 GMT
ADD file:4a87d706ba1c6cdeab729abca0c932709611862dfdf5d46d9f07660a549fd043 in / 
# Wed, 01 Mar 2023 01:39:24 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:10:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:11:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:11:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:13:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:965c7d391035444250e8549e1aa77d80a0692089e844b5c3d6f4e4924f096a99`  
		Last Modified: Wed, 01 Mar 2023 01:45:08 GMT  
		Size: 51.2 MB (51207396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7561c3f10011960cdcee2d97ca318791aeb60e8e7b34375e50ce1691e1f373b6`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 8.0 MB (8033127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edba82cb80eba68e543537bb7bf09a496a1270646491b65f1804a2551eceae`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 10.3 MB (10345751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe6c0714838b2d72c79e2fb8a0fb23c8de6b3d246827b2fd913e3af6734aaa`  
		Last Modified: Wed, 01 Mar 2023 02:25:21 GMT  
		Size: 53.5 MB (53471402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858b45e654212bda5c76759252da6702f83ee966fcf91e7131a8e9ab4f2f5a17`  
		Last Modified: Wed, 01 Mar 2023 02:26:05 GMT  
		Size: 198.5 MB (198468540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:42598525905fd1e45966adbb9f2c69f78ca053feb530bf7b99e572b89fd3f77c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:edf320c3d1538c793e4aa6db8ae0030fb8d9bcd93c32d1173668018af289abd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68313473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e264a14e2fb2275166171b218ac3b34315ea1e90c78b540056de532c018c86b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:44:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:44:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fc05781c9a4a3dee77723abf708dd674020a00d7d57dd6cc1f9bc72da96143`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 7.9 MB (7862980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efc3ea86e67ce8cdce1cf3619f311735cbbb8744a1c69536f8a390d014c0a99`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 10.0 MB (10001392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:260fa862731a48f61d191023a25f1f9b657f45a421b53cb8857c87b68f3d1e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62417436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768e09ebea3080e9905c76f34b636f7ae2caced8f0c84dcdb609ad8c6b2d1c5a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:03 GMT
ADD file:28e7414281fcd12661d43cccdf7062bf4aa15641f986cae3aa3260fcb8e16bb5 in / 
# Wed, 01 Mar 2023 01:58:03 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:34:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:34:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4ba30d485dd0583b3079a70184a97c458599a0629e661b1382394653cb802242`  
		Last Modified: Wed, 01 Mar 2023 02:03:25 GMT  
		Size: 45.9 MB (45916077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5b3ed640e906ad20c2a86568f52c60a48e1d82e4654d3378280f572737f7c1`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 7.2 MB (7152340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028b21e39d17f6632c7b82f0c900d32b50233b13940a7a60009782a6abc32cdd`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 9.3 MB (9349019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:129a088e650fae94076fc92386141a86cd2f37e370edc651d6fcdebd47ca9887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66975000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4479ef63c587db1ceab4c7d6387457f7c8109f921dc37d1fb1618c608893d402`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:50:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a788623352140f16227efacfe9a8b497cf91ee63fa69554615640474975ca5`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 7.7 MB (7731356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12086fb08985806514ae1e77eef44a12e303bd44b113e62dac28b16b778fc797`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 10.0 MB (10003642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8f735fd4bda81af31cec932c12fee884df969e8a32b286fa0d652d1555d356a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69586274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed659aba5f7d179e5c1a17d9d85e4a30314268a86ca791736d27013b45cc57ef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:23 GMT
ADD file:4a87d706ba1c6cdeab729abca0c932709611862dfdf5d46d9f07660a549fd043 in / 
# Wed, 01 Mar 2023 01:39:24 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:10:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:11:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:965c7d391035444250e8549e1aa77d80a0692089e844b5c3d6f4e4924f096a99`  
		Last Modified: Wed, 01 Mar 2023 01:45:08 GMT  
		Size: 51.2 MB (51207396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7561c3f10011960cdcee2d97ca318791aeb60e8e7b34375e50ce1691e1f373b6`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 8.0 MB (8033127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edba82cb80eba68e543537bb7bf09a496a1270646491b65f1804a2551eceae`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 10.3 MB (10345751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:179f7c72ed12161b5e7a09e106882d6b82077554946eb99908d44ac79a1d8a91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f2c53ffd804089bac100dacb8c968c3c9d375d99a42a7ab5f596d77ba333046b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120187174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da6f85600da7d195cbab7b247097c398fdf3b93551418d77e05df7d7563d17d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:44:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:44:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:44:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fc05781c9a4a3dee77723abf708dd674020a00d7d57dd6cc1f9bc72da96143`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 7.9 MB (7862980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efc3ea86e67ce8cdce1cf3619f311735cbbb8744a1c69536f8a390d014c0a99`  
		Last Modified: Wed, 01 Mar 2023 04:51:20 GMT  
		Size: 10.0 MB (10001392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47452733a7c0712961d7ef8b48e3d823328f056af1c90c715966748b137b3d1c`  
		Last Modified: Wed, 01 Mar 2023 04:51:39 GMT  
		Size: 51.9 MB (51873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:88b650bc14650aff80cfac6809cce960f3eb237f5d1aa230be53efcbb8e39e0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109814075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd66a0bcb6cf53591c330eecba51cca59ae4ab082c1d62528b68861ac89863cf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:03 GMT
ADD file:28e7414281fcd12661d43cccdf7062bf4aa15641f986cae3aa3260fcb8e16bb5 in / 
# Wed, 01 Mar 2023 01:58:03 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:34:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:34:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:34:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ba30d485dd0583b3079a70184a97c458599a0629e661b1382394653cb802242`  
		Last Modified: Wed, 01 Mar 2023 02:03:25 GMT  
		Size: 45.9 MB (45916077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5b3ed640e906ad20c2a86568f52c60a48e1d82e4654d3378280f572737f7c1`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 7.2 MB (7152340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028b21e39d17f6632c7b82f0c900d32b50233b13940a7a60009782a6abc32cdd`  
		Last Modified: Wed, 01 Mar 2023 03:10:25 GMT  
		Size: 9.3 MB (9349019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35297b6d570293c7581e727c51353a6eb15d3b2f7bdaf391595c28c2a8d4fc6`  
		Last Modified: Wed, 01 Mar 2023 03:10:43 GMT  
		Size: 47.4 MB (47396639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:90aa1cac3a307d98880753d6cf9760451142763726f491a838ac25e086333607
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119167055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e9a68c76d5f6d839f7521c0ad7aea5ed89f2bc316ae2264d2194744d29c61b7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:50:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:51:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a788623352140f16227efacfe9a8b497cf91ee63fa69554615640474975ca5`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 7.7 MB (7731356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12086fb08985806514ae1e77eef44a12e303bd44b113e62dac28b16b778fc797`  
		Last Modified: Wed, 01 Mar 2023 02:57:17 GMT  
		Size: 10.0 MB (10003642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afc4bf76406adbdc8533ba0c416f2aac77ca7db02bb6d380eaeeb778f56c5d4`  
		Last Modified: Wed, 01 Mar 2023 02:57:32 GMT  
		Size: 52.2 MB (52192055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0229c279db07ac7afae573e7d92394661b8c51cf18da96afb9fa3484414f8d88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123057676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5cfe505ca5988b3b2fe88cd03e4789c502265fc7d6bee4b1b277b5241d4c139`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:23 GMT
ADD file:4a87d706ba1c6cdeab729abca0c932709611862dfdf5d46d9f07660a549fd043 in / 
# Wed, 01 Mar 2023 01:39:24 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:10:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:11:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:11:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:965c7d391035444250e8549e1aa77d80a0692089e844b5c3d6f4e4924f096a99`  
		Last Modified: Wed, 01 Mar 2023 01:45:08 GMT  
		Size: 51.2 MB (51207396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7561c3f10011960cdcee2d97ca318791aeb60e8e7b34375e50ce1691e1f373b6`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 8.0 MB (8033127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edba82cb80eba68e543537bb7bf09a496a1270646491b65f1804a2551eceae`  
		Last Modified: Wed, 01 Mar 2023 02:24:59 GMT  
		Size: 10.3 MB (10345751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe6c0714838b2d72c79e2fb8a0fb23c8de6b3d246827b2fd913e3af6734aaa`  
		Last Modified: Wed, 01 Mar 2023 02:25:21 GMT  
		Size: 53.5 MB (53471402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:f5efcf35ed707b7aeb078d6ddfdefc91a9715390a7d8003e51338f7d3630c941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a6ef7420ef5f9b158be970b586c122041efe47c340f36511af02b66b15f50021
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125674680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5069942e3d6eec75afd35fb58f4b25abd6e63a90e224fdfc1ef8b3db05d82130`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:43:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cdcd4942ebc7445d8a70117a83ecbc77dcc5ffc72c4b6f8e24c0c76cfee15d`  
		Last Modified: Wed, 01 Mar 2023 04:50:33 GMT  
		Size: 54.6 MB (54585443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e6642afa6470d719d40e0aedb05dcd82386c83ea9e49990ecd703001eea0708c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120535205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10cf2c6f88593a41cfd3f16b24bfee123e13190615f8330cee60375c884c9e4b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:18:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d373aa541f88e7c81c88d63aca3fd07f01c6220ca295915af87f489a6cb251`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 5.1 MB (5072694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c176fe3230b5050ab13f5cd081fa601f679459e28449694496136a73bddd175c`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 10.6 MB (10573876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04072817b27c20dd9a7f9a0b93816bd195f8675845e235c0291c0f935824f610`  
		Last Modified: Wed, 01 Mar 2023 02:25:18 GMT  
		Size: 52.3 MB (52338815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c7076592183315790b451e7400610a2108a088eff9828031faacdc4ec0ef67b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115720274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adf4d1a818db1580563de9b22ed7fcc9738c034bdc78b5f4613ef9e96e02bd1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e676c4187d9dd900add9c8dd4b9c906be40a2b8db6cabfdaf280ac2e83cdfca`  
		Last Modified: Wed, 01 Mar 2023 03:09:35 GMT  
		Size: 50.4 MB (50355863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cf7219efab275bd3d3fbfd3ab95e7f321352cb3c012f6368843680ccb19abe5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124405850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf6eda9f040f4295ca3f9857f1ea0b5a1fdcc0cdb7491510b5223a2bf02530f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8747d4a988af1d119e668971a87213d5c7061fc04671ba6fcb7123a1c11507ac`  
		Last Modified: Wed, 01 Mar 2023 02:56:37 GMT  
		Size: 54.7 MB (54676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bf5cacb020595095738a86d659889e8825c9cee19c92064a670ddafcb6207a08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128494248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab6f0c472327c2c68c41ac703fb1caadce376b919f50c96745d2ae9165023bf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471482ade37b25d9ec22336d057dd4ed265a030b98595eac314b56d5709bbdff`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 5.3 MB (5293673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a995bf7fa061158e93790e264fd3bc4a3340e75bf857b3c51814384b5f1344f5`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 11.2 MB (11249844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9955e6ae7dba34d1170876e13f1c83b049619255f38babb22074d26848658318`  
		Last Modified: Wed, 01 Mar 2023 02:23:54 GMT  
		Size: 55.9 MB (55922655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:07d501b1a244ee7c0ed6d4e9c5c5704cedd96cfb51bc776b2c778aec5bd274a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122158227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f882bdd498e5f8cf1f6bfe78012ad9b00c0b3e1d476d3b20a12bef5e08231e5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:42:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791a92fb38ebf78f5ed530cc39361869dd25ce941ea09d0580b866204f0e8e1`  
		Last Modified: Thu, 09 Feb 2023 07:59:50 GMT  
		Size: 4.9 MB (4921594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c347eddc487950d631dca4e7c20c1165566e8418703435fad325a721c0e8d`  
		Last Modified: Thu, 09 Feb 2023 07:59:52 GMT  
		Size: 10.7 MB (10662160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9ee56dfe2667a1d6574684709026d72883d1af28301257038f732b76362e9a`  
		Last Modified: Thu, 09 Feb 2023 08:00:40 GMT  
		Size: 53.3 MB (53307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8bd4ae58c5a9dd9152f3d51bfd815b98f2dbfec6309beb31666524144e8db6a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134830408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0053e746dde1fab6a1b0954f7f14f6d3a0eb7689b80f2ccaa15954b3b156e44c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:01 GMT
ADD file:40523b7b16ccf1ff245b11e11f92d24e9e6e9dfbdbc755d4361cf55c7ec26244 in / 
# Wed, 01 Mar 2023 04:47:11 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:25:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:26:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b7949e1acd104233f80137ab3a92a148b0d48e41b3075c70a2d636c3b4c60bf`  
		Last Modified: Wed, 01 Mar 2023 04:53:18 GMT  
		Size: 58.9 MB (58921304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b3574e90831068a9bd9f64e57da92a087d925f0a0e63c764ecf421b18d3a1`  
		Last Modified: Wed, 01 Mar 2023 05:39:22 GMT  
		Size: 5.4 MB (5415247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8bec1f2d073d24de5e7dd051bcada4f0a407fc713e38b49fc2d2a863bde38e`  
		Last Modified: Wed, 01 Mar 2023 05:39:23 GMT  
		Size: 11.6 MB (11629925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3bc8a98c359709356de5d552e69a43170d7f81b4ad5ac17cfbb0eb8d3da2b1`  
		Last Modified: Wed, 01 Mar 2023 05:39:53 GMT  
		Size: 58.9 MB (58863932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f26531b6a394a77d086c8d03202eddded5c7e44b39da743ad759ba173721a941
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123252982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab21b2830a2681e63ef03f163b5c2437190e155339ff1e3db316ff358b283e3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:07 GMT
ADD file:e5f01d8f88c8134571e8998672a504ecad259a9a8322df73aed4a93ffac08ebd in / 
# Wed, 01 Mar 2023 02:50:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:14:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51f6de0debe6daa552b12c9951f6529a870979d923187c1ba62ff66cee3450ac`  
		Last Modified: Wed, 01 Mar 2023 02:54:25 GMT  
		Size: 53.3 MB (53277694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6404e912b557d72a71a982115ad4b92e1c23918b7f0c950f6f22c2ec775ff936`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 5.1 MB (5149110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0561ee66ff6ae2ce12d922c3d0fed94e18a801571a2add9e526e914cb30a3bab`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 10.8 MB (10765987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c7ccf7cb532de1600bce9245b8e167d6d644608677c26601c246c4e80cdbf`  
		Last Modified: Wed, 01 Mar 2023 03:22:28 GMT  
		Size: 54.1 MB (54060191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:a8e1957e6cdefeacc8d7a0099162f76da0746af71529e78f7d56e4e60ab1b44e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:sid` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4cf68c882cee9b417142c8f85e20e26fcdb0fa83cc0f991801de65462df2f4cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.8 MB (344815719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f756652badfd81aa904ebea98fc74ac8af051853f59e0e07e17c01a6fe5fd60`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:57 GMT
ADD file:742621d60641957542e01d843bc130e616ba577a7135783b21e53d3a5d77ad5b in / 
# Wed, 01 Mar 2023 04:10:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:46:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:46:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:47:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d80cbe2ffd4f13cce276662ea5b4fa412791129d545137a4bea79fc41c446e0b`  
		Last Modified: Wed, 01 Mar 2023 04:15:57 GMT  
		Size: 49.3 MB (49261286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414a406365e2c651e77ea1d2dedd2c2fe7317552757dfc2701d2cdf6a578a51e`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 9.1 MB (9063535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515af3674ccc4fa7b84288322c2d1250d4de5952aafb54a33baeaf74fb694632`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 11.4 MB (11405848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4328fcba3826a509a956e5614c022c05ed89b4e718a69b607176d4a8f97f0e86`  
		Last Modified: Wed, 01 Mar 2023 04:52:36 GMT  
		Size: 64.2 MB (64156733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5761bef1786d1a3043cfdd4502ded7b68eb76cddebebdfd5e61420f1ab445`  
		Last Modified: Wed, 01 Mar 2023 04:53:10 GMT  
		Size: 210.9 MB (210928317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cfab3ca8a8f26671e80ccdb59dd4ba9f96d324240fab5eca7fda5b7282e680d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.5 MB (313512864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98658392247eaba632e8d135986bbf3cb581ed4c064c7c09cc42508038e13052`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:01 GMT
ADD file:4fadb88d3ead8d91349c79d7e903bbb8f6130b292bda6cb8099131210a815bc1 in / 
# Wed, 01 Mar 2023 01:49:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:21:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:21:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:22:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03e1abdb2ebe924d64faf35eb6563891039999ec54a62f65419caf539ba6a88`  
		Last Modified: Wed, 01 Mar 2023 01:53:21 GMT  
		Size: 48.1 MB (48107781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d446d9cfc1201a906803d21a6e36423e22e9bebf24cf64bd16a4a3a73af61a2`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 8.5 MB (8514426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dc22595c5f06cd6d232ff8a3594b9aadef31095cb355dffad2b48a861717bf`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 11.1 MB (11051502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0760e34b5fee30fa55ba71775caf6a3b2e755775ea03be4db0c03e5d83ff0a3`  
		Last Modified: Wed, 01 Mar 2023 02:26:32 GMT  
		Size: 61.6 MB (61563988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0bee41572d3fd2c79c2cec17ba9f302c4197090c7cd926637454ea269c1fcf`  
		Last Modified: Wed, 01 Mar 2023 02:27:08 GMT  
		Size: 184.3 MB (184275167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4fd065ebb7280f186e201ef931745f11b0ed5709bb74ebfce845fa07383b77de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.9 MB (298924502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb866bf86688fd657c0d0bbb77f601dc7b5b740627aacc2b35cdb24985d07cd5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:39 GMT
ADD file:2cc322ac43103c8e367e39beaccf285da593ce4935ec4b1c90ae321a43b7123b in / 
# Wed, 01 Mar 2023 01:58:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:37:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:37:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:38:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e5967747d4d88696bd5d5f37c0b5b8bcf8b29f3b448f6d1dd9623bdcc655965`  
		Last Modified: Wed, 01 Mar 2023 02:04:52 GMT  
		Size: 45.9 MB (45878967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00c059161524278c4c36c19bc9e15f881a76d35dfa7907d64e5368fa08cfabe`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 8.2 MB (8158629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e2cef807b62672343d701b6833953bd521a7ce41702624f45d2d796b0748e2`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 10.7 MB (10687679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aec6c2a63ff15795fd7235464c074e62a01aab27b66c75e51aca4b22d1ec07`  
		Last Modified: Wed, 01 Mar 2023 03:11:48 GMT  
		Size: 59.3 MB (59272951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47368484dc827d2541150d970d099cbc827331cba4014efcecf477781757c153`  
		Last Modified: Wed, 01 Mar 2023 03:12:21 GMT  
		Size: 174.9 MB (174926276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:844c8028a9815c68e30fdb0e3c1284cdd82ca2e3b6d6c93da5ddd5c6fc929502
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335903373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932509bb66171d164ed37159485c8587937293e2a8149266b757ba8858fe5483`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:21:20 GMT
ADD file:83e31d97e59fa435e4367903bc4de14c4bc67178b21cea27910cd23f23eb3a80 in / 
# Wed, 01 Mar 2023 02:21:20 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:52:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:53:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4362be0bd44228649833bb1416738fd1e9e110c9b44995dc7b36d6f6c712645f`  
		Last Modified: Wed, 01 Mar 2023 02:25:46 GMT  
		Size: 49.3 MB (49295339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2110847b2a04ab78caa763031ad2defabdaf9d626dbfcec71b215d35f0b70f09`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 8.9 MB (8900926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd381966a1347f9482594ca89251700a2fc3c4cfc23300a89d68207091e90084`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 11.4 MB (11371514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade03fa0cf349d2c4310e97b9776862ea961b32865410ca43789d56b255550f`  
		Last Modified: Wed, 01 Mar 2023 02:58:24 GMT  
		Size: 64.0 MB (64013118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dd468c1139187176cb306ea33f3fa3f4b68fed6a00e7d0835793454ce00e1b`  
		Last Modified: Wed, 01 Mar 2023 02:58:52 GMT  
		Size: 202.3 MB (202322476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:631c6b61580c0129c1a56f05b9a93618a0a1afdabbcf59f3a128367f86d855d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.2 MB (347248309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:046c7b891ef4ccee961ced21d3fe4461e8ea27d47b2529539f9c33b23fdbb62b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:40:05 GMT
ADD file:6282b025bbfdc732e0b90ff88ecdc7d48b84ec602874ef46e276d0250551f12e in / 
# Wed, 01 Mar 2023 01:40:06 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:14:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:15:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:417b7bc42b68fb696c2efa25377639c22c351f4705d5168da4f5695d53e4ba47`  
		Last Modified: Wed, 01 Mar 2023 01:46:43 GMT  
		Size: 50.3 MB (50314271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b68a1e6101c58260f889183e2e061e123bbc07a479a4ee59fff5649daa51d`  
		Last Modified: Wed, 01 Mar 2023 02:26:18 GMT  
		Size: 9.3 MB (9251109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63437f1cf3bc2a6cddc930ecd9a659ccfbcce779ac90a9c50efc7e8c1f56b42`  
		Last Modified: Wed, 01 Mar 2023 02:26:17 GMT  
		Size: 11.8 MB (11808756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd353cc8e971b20a47938912dda14d6fec9624aa9880053413a451cb3bc0f60`  
		Last Modified: Wed, 01 Mar 2023 02:26:41 GMT  
		Size: 66.0 MB (66012422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b99a677370160cefe862644ca09270260b636f9de7ee445839ef305d8857f6`  
		Last Modified: Wed, 01 Mar 2023 02:27:28 GMT  
		Size: 209.9 MB (209861751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a82507a1277c2124e09e887dfd7b4a31b0b1a1fc8bdec1f883b117f297e76d2c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.0 MB (324036580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d50a394cea62448159f423b39c3070b86d3314f1423d507654ecb0497d9c0d7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:46:00 GMT
ADD file:e14c7d6714484cc404ef7af2c7e0fcb17120cc8c1b631e9ac731a3be75da22b8 in / 
# Thu, 09 Feb 2023 02:46:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:48:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:55:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84e1d5547cbc284ab87d41eaa50711a7148e6080522c4ba245d27048c9d0fe70`  
		Last Modified: Thu, 09 Feb 2023 02:54:32 GMT  
		Size: 49.1 MB (49094289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16034fc732dcaff117d4120f724155ad39c461a2791c8bc488000dd93d88467c`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 8.4 MB (8414070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cc8b6e8bd467b0d1e27bfaf0bf0138f2e690aa8dd7eeddcc636d65c4b0ac34`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 11.2 MB (11153733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23789f2ae164d9a3f26a9a0663d938660993a4ba223713b5bde1aa34f68d35dc`  
		Last Modified: Thu, 09 Feb 2023 08:03:53 GMT  
		Size: 63.3 MB (63305330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd03ad3d3e89587274ed0844975c8ff2700fd1f95b056d7346b990bf970c894`  
		Last Modified: Thu, 09 Feb 2023 08:06:05 GMT  
		Size: 192.1 MB (192069158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:270e720c1a0ba1d7fadc6591991b8d7f9984f5aea254d2191222f1caae76c910
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.7 MB (358677337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a4b45352ad5e080d3923b7fec61af29c23f2d69f6a6616fd50b10fd0c9e8385`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:54 GMT
ADD file:2c1195fd765d1da7082bf383b9c5ef0b244e5398006d53897d5ea40e919399f1 in / 
# Wed, 01 Mar 2023 04:47:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:31:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:31:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:34:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6800c47237e7f7a1e5340856e56ba98e2b69a475b2458bb2416fdb0582d8c28`  
		Last Modified: Wed, 01 Mar 2023 04:54:24 GMT  
		Size: 53.3 MB (53273011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff0fff502cf707b8386c45c579606a759f85d3b49c007814826ad27212fdf5`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 9.7 MB (9652015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ef4d32b9b5d605909945396d9e13b86c238ff2ea6c800b63cef6d06dc2d6a3`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 12.2 MB (12168382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecf54311632074a960030227c6fca18a718af9b2631164c5c93529e814a5f50`  
		Last Modified: Wed, 01 Mar 2023 05:41:38 GMT  
		Size: 69.6 MB (69617831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48046f9759059f8abfcf3bf8b3ff28b67f3df1bd9cc3a2d31dcbee40947822d6`  
		Last Modified: Wed, 01 Mar 2023 05:42:40 GMT  
		Size: 214.0 MB (213966098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f36f7686751e847a8c69af8eba89a80c31e16ec89434ba40ebccec03984464e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.8 MB (313760190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a70710ffc9aeb0b1ef9ecfdbb6a892cec5ccdd05e291bf44c01c504fb8cfe`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:42 GMT
ADD file:a35d410eeff51ff3b7d9c823bc5ba421ef11373fb29ee93e8256efcbcdcee908 in / 
# Wed, 01 Mar 2023 02:50:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:16:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:16:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:17:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57e87143a56f85b3245b752ff94d616ef62e6372c0bcd9338b791267ea20f326`  
		Last Modified: Wed, 01 Mar 2023 02:55:04 GMT  
		Size: 47.6 MB (47629137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07cda735865838550e6455f8a76e842211afddfe8503e32aa744121e3435ae0`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 8.7 MB (8700269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c406447e84cbeb09410da5fd14cb6601c6f124b564b303a89c89e53406f68863`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 11.3 MB (11268803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b0879a47bff8d8b52a41d4dd0ceb2fa4313863026dfe04be33a743663128f8`  
		Last Modified: Wed, 01 Mar 2023 03:23:22 GMT  
		Size: 63.2 MB (63158949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a52b22ad7915c526a6a5a76890d098c9218f26db48004203de3a4630e03a54`  
		Last Modified: Wed, 01 Mar 2023 03:23:50 GMT  
		Size: 183.0 MB (183003032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:f6ef54d09fc53d24d449af6a6a8400f9d4056aab7a21396f3e85e3e9a973720e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:93738b56202c447b2ea0eef8020a8d4664e3712974058a408730f1218abb1830
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69730669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712e351b2bc9d7d841a9fcc1bb27278f12cb09bb4240cdc6338503b846bf87e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:57 GMT
ADD file:742621d60641957542e01d843bc130e616ba577a7135783b21e53d3a5d77ad5b in / 
# Wed, 01 Mar 2023 04:10:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:46:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:46:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d80cbe2ffd4f13cce276662ea5b4fa412791129d545137a4bea79fc41c446e0b`  
		Last Modified: Wed, 01 Mar 2023 04:15:57 GMT  
		Size: 49.3 MB (49261286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414a406365e2c651e77ea1d2dedd2c2fe7317552757dfc2701d2cdf6a578a51e`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 9.1 MB (9063535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515af3674ccc4fa7b84288322c2d1250d4de5952aafb54a33baeaf74fb694632`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 11.4 MB (11405848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b130af12e26d3c5dbafb04dcbcf75f0e751bb8327318a85a088aa317ab591e69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67673709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa3339472cc907f434562326764e3c0a37312ea0c737ab2fe67f577e10abf020`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:01 GMT
ADD file:4fadb88d3ead8d91349c79d7e903bbb8f6130b292bda6cb8099131210a815bc1 in / 
# Wed, 01 Mar 2023 01:49:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:21:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a03e1abdb2ebe924d64faf35eb6563891039999ec54a62f65419caf539ba6a88`  
		Last Modified: Wed, 01 Mar 2023 01:53:21 GMT  
		Size: 48.1 MB (48107781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d446d9cfc1201a906803d21a6e36423e22e9bebf24cf64bd16a4a3a73af61a2`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 8.5 MB (8514426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dc22595c5f06cd6d232ff8a3594b9aadef31095cb355dffad2b48a861717bf`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 11.1 MB (11051502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c9f72e9a500675032dd14939ac68f619ef7378e2ba5fa0bbe71d9f4e138b1413
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64725275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5849c538e7b742ecab1b90a01e25aac9dcef8e7de5b52969e2db8b217418209`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:39 GMT
ADD file:2cc322ac43103c8e367e39beaccf285da593ce4935ec4b1c90ae321a43b7123b in / 
# Wed, 01 Mar 2023 01:58:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:37:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4e5967747d4d88696bd5d5f37c0b5b8bcf8b29f3b448f6d1dd9623bdcc655965`  
		Last Modified: Wed, 01 Mar 2023 02:04:52 GMT  
		Size: 45.9 MB (45878967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00c059161524278c4c36c19bc9e15f881a76d35dfa7907d64e5368fa08cfabe`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 8.2 MB (8158629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e2cef807b62672343d701b6833953bd521a7ce41702624f45d2d796b0748e2`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 10.7 MB (10687679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4e04b288f31813639ec17e2ea31d111af553db8e47d7f70b166a0772f57544bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69567779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f267da9f91af76c93bff56ed319ac711d450951f634b99b0aff5950a94ccc3c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:21:20 GMT
ADD file:83e31d97e59fa435e4367903bc4de14c4bc67178b21cea27910cd23f23eb3a80 in / 
# Wed, 01 Mar 2023 02:21:20 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:52:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4362be0bd44228649833bb1416738fd1e9e110c9b44995dc7b36d6f6c712645f`  
		Last Modified: Wed, 01 Mar 2023 02:25:46 GMT  
		Size: 49.3 MB (49295339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2110847b2a04ab78caa763031ad2defabdaf9d626dbfcec71b215d35f0b70f09`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 8.9 MB (8900926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd381966a1347f9482594ca89251700a2fc3c4cfc23300a89d68207091e90084`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 11.4 MB (11371514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:75ed184206d2a35482c7d7f4648ce76a7ff1ca43e067a606c00b50aa756c8a2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71374136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b3d805c3fa51b65df72429839a1b714ea37b5e2d1916b81f60bd136aa385b9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:40:05 GMT
ADD file:6282b025bbfdc732e0b90ff88ecdc7d48b84ec602874ef46e276d0250551f12e in / 
# Wed, 01 Mar 2023 01:40:06 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:417b7bc42b68fb696c2efa25377639c22c351f4705d5168da4f5695d53e4ba47`  
		Last Modified: Wed, 01 Mar 2023 01:46:43 GMT  
		Size: 50.3 MB (50314271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b68a1e6101c58260f889183e2e061e123bbc07a479a4ee59fff5649daa51d`  
		Last Modified: Wed, 01 Mar 2023 02:26:18 GMT  
		Size: 9.3 MB (9251109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63437f1cf3bc2a6cddc930ecd9a659ccfbcce779ac90a9c50efc7e8c1f56b42`  
		Last Modified: Wed, 01 Mar 2023 02:26:17 GMT  
		Size: 11.8 MB (11808756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:31fbd48d97655e5743ae24d79f322184b28fe3e464b6ed9b4413ed1ffbea4648
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68662092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c4ec537af7ac1217076c5de461da3049f4b71d1e970249041e8a4abcdf3f1e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:46:00 GMT
ADD file:e14c7d6714484cc404ef7af2c7e0fcb17120cc8c1b631e9ac731a3be75da22b8 in / 
# Thu, 09 Feb 2023 02:46:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:48:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:84e1d5547cbc284ab87d41eaa50711a7148e6080522c4ba245d27048c9d0fe70`  
		Last Modified: Thu, 09 Feb 2023 02:54:32 GMT  
		Size: 49.1 MB (49094289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16034fc732dcaff117d4120f724155ad39c461a2791c8bc488000dd93d88467c`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 8.4 MB (8414070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cc8b6e8bd467b0d1e27bfaf0bf0138f2e690aa8dd7eeddcc636d65c4b0ac34`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 11.2 MB (11153733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f9a20d8078e12b97c3af8d9cdf1430e92499f23331fb4b029781ed5c46a2d4f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75093408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63aab7de5aecbad2363c5a0586046d3331cbdb0b8c3f89bf38833c6666ef81f4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:54 GMT
ADD file:2c1195fd765d1da7082bf383b9c5ef0b244e5398006d53897d5ea40e919399f1 in / 
# Wed, 01 Mar 2023 04:47:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:31:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b6800c47237e7f7a1e5340856e56ba98e2b69a475b2458bb2416fdb0582d8c28`  
		Last Modified: Wed, 01 Mar 2023 04:54:24 GMT  
		Size: 53.3 MB (53273011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff0fff502cf707b8386c45c579606a759f85d3b49c007814826ad27212fdf5`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 9.7 MB (9652015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ef4d32b9b5d605909945396d9e13b86c238ff2ea6c800b63cef6d06dc2d6a3`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 12.2 MB (12168382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7d8971371d1f0e05a21c043ffe902ef04946af99350b31cd8f69abcdf9c17aa1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67598209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c301055db6d45991d5c906e7e43bace2c2bbd2050ca71189ea3d370259f5b54`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:42 GMT
ADD file:a35d410eeff51ff3b7d9c823bc5ba421ef11373fb29ee93e8256efcbcdcee908 in / 
# Wed, 01 Mar 2023 02:50:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:16:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:57e87143a56f85b3245b752ff94d616ef62e6372c0bcd9338b791267ea20f326`  
		Last Modified: Wed, 01 Mar 2023 02:55:04 GMT  
		Size: 47.6 MB (47629137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07cda735865838550e6455f8a76e842211afddfe8503e32aa744121e3435ae0`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 8.7 MB (8700269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c406447e84cbeb09410da5fd14cb6601c6f124b564b303a89c89e53406f68863`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 11.3 MB (11268803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:a656a4057c545394d275f9a2401b1212207ae6b365880a71f1bdac8ce7acb84e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:61e869911246ffffe7006b0cf40b8e69c786397789246c1d7f0c362b4f77f0a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133887402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea16ba12d186d3aa3a15eccbe528665df5a6182d3e781f14d550e664cad9220`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:57 GMT
ADD file:742621d60641957542e01d843bc130e616ba577a7135783b21e53d3a5d77ad5b in / 
# Wed, 01 Mar 2023 04:10:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:46:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:46:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d80cbe2ffd4f13cce276662ea5b4fa412791129d545137a4bea79fc41c446e0b`  
		Last Modified: Wed, 01 Mar 2023 04:15:57 GMT  
		Size: 49.3 MB (49261286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414a406365e2c651e77ea1d2dedd2c2fe7317552757dfc2701d2cdf6a578a51e`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 9.1 MB (9063535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515af3674ccc4fa7b84288322c2d1250d4de5952aafb54a33baeaf74fb694632`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 11.4 MB (11405848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4328fcba3826a509a956e5614c022c05ed89b4e718a69b607176d4a8f97f0e86`  
		Last Modified: Wed, 01 Mar 2023 04:52:36 GMT  
		Size: 64.2 MB (64156733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:769b660d04142b0b50dc374c44a0b6f21f9c173ee6da78112733f53722b345b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129237697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edd56cc8039bae242894637cb565ef5a4685943100e6e52d22630c1fe20fb1f8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:01 GMT
ADD file:4fadb88d3ead8d91349c79d7e903bbb8f6130b292bda6cb8099131210a815bc1 in / 
# Wed, 01 Mar 2023 01:49:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:21:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:21:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03e1abdb2ebe924d64faf35eb6563891039999ec54a62f65419caf539ba6a88`  
		Last Modified: Wed, 01 Mar 2023 01:53:21 GMT  
		Size: 48.1 MB (48107781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d446d9cfc1201a906803d21a6e36423e22e9bebf24cf64bd16a4a3a73af61a2`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 8.5 MB (8514426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dc22595c5f06cd6d232ff8a3594b9aadef31095cb355dffad2b48a861717bf`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 11.1 MB (11051502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0760e34b5fee30fa55ba71775caf6a3b2e755775ea03be4db0c03e5d83ff0a3`  
		Last Modified: Wed, 01 Mar 2023 02:26:32 GMT  
		Size: 61.6 MB (61563988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eec8b1e8acf1938703616b1dd5e636aafaf9a348da0a8b4f760abadf820d5f02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123998226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4711888af9d924bb6d81ff35c959c48dc8dd3764331e7e8f75c4be9208721f1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:39 GMT
ADD file:2cc322ac43103c8e367e39beaccf285da593ce4935ec4b1c90ae321a43b7123b in / 
# Wed, 01 Mar 2023 01:58:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:37:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:37:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e5967747d4d88696bd5d5f37c0b5b8bcf8b29f3b448f6d1dd9623bdcc655965`  
		Last Modified: Wed, 01 Mar 2023 02:04:52 GMT  
		Size: 45.9 MB (45878967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00c059161524278c4c36c19bc9e15f881a76d35dfa7907d64e5368fa08cfabe`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 8.2 MB (8158629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e2cef807b62672343d701b6833953bd521a7ce41702624f45d2d796b0748e2`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 10.7 MB (10687679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aec6c2a63ff15795fd7235464c074e62a01aab27b66c75e51aca4b22d1ec07`  
		Last Modified: Wed, 01 Mar 2023 03:11:48 GMT  
		Size: 59.3 MB (59272951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:79a54877762e7ec47749ccafef71d6e63006d42146126ffde09fa7cd30f3571b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133580897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:280a9022e0a86f89746caefe50eaaece1019298b65d05471d89f1afde4acd87e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:21:20 GMT
ADD file:83e31d97e59fa435e4367903bc4de14c4bc67178b21cea27910cd23f23eb3a80 in / 
# Wed, 01 Mar 2023 02:21:20 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:52:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4362be0bd44228649833bb1416738fd1e9e110c9b44995dc7b36d6f6c712645f`  
		Last Modified: Wed, 01 Mar 2023 02:25:46 GMT  
		Size: 49.3 MB (49295339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2110847b2a04ab78caa763031ad2defabdaf9d626dbfcec71b215d35f0b70f09`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 8.9 MB (8900926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd381966a1347f9482594ca89251700a2fc3c4cfc23300a89d68207091e90084`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 11.4 MB (11371514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade03fa0cf349d2c4310e97b9776862ea961b32865410ca43789d56b255550f`  
		Last Modified: Wed, 01 Mar 2023 02:58:24 GMT  
		Size: 64.0 MB (64013118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6cde2155211d3f4d8d5db27af2fcc9954e9dbbe93b2e7a4208d6d145acb510de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137386558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed49974f31df5dbc1da3062aa51816dadfe02a8052b7def49df2b41c34fd9ff7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:40:05 GMT
ADD file:6282b025bbfdc732e0b90ff88ecdc7d48b84ec602874ef46e276d0250551f12e in / 
# Wed, 01 Mar 2023 01:40:06 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:14:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:417b7bc42b68fb696c2efa25377639c22c351f4705d5168da4f5695d53e4ba47`  
		Last Modified: Wed, 01 Mar 2023 01:46:43 GMT  
		Size: 50.3 MB (50314271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b68a1e6101c58260f889183e2e061e123bbc07a479a4ee59fff5649daa51d`  
		Last Modified: Wed, 01 Mar 2023 02:26:18 GMT  
		Size: 9.3 MB (9251109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63437f1cf3bc2a6cddc930ecd9a659ccfbcce779ac90a9c50efc7e8c1f56b42`  
		Last Modified: Wed, 01 Mar 2023 02:26:17 GMT  
		Size: 11.8 MB (11808756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd353cc8e971b20a47938912dda14d6fec9624aa9880053413a451cb3bc0f60`  
		Last Modified: Wed, 01 Mar 2023 02:26:41 GMT  
		Size: 66.0 MB (66012422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0abaabff52c976ed8f5fad72ca4d2637d4a6156591f7273dd926406bf5ab1b78
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131967422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9530e0dcd15bd60dd08d51b5a5cce11f7dd40d377205a10ef937708bfd716fce`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:46:00 GMT
ADD file:e14c7d6714484cc404ef7af2c7e0fcb17120cc8c1b631e9ac731a3be75da22b8 in / 
# Thu, 09 Feb 2023 02:46:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:48:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84e1d5547cbc284ab87d41eaa50711a7148e6080522c4ba245d27048c9d0fe70`  
		Last Modified: Thu, 09 Feb 2023 02:54:32 GMT  
		Size: 49.1 MB (49094289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16034fc732dcaff117d4120f724155ad39c461a2791c8bc488000dd93d88467c`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 8.4 MB (8414070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cc8b6e8bd467b0d1e27bfaf0bf0138f2e690aa8dd7eeddcc636d65c4b0ac34`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 11.2 MB (11153733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23789f2ae164d9a3f26a9a0663d938660993a4ba223713b5bde1aa34f68d35dc`  
		Last Modified: Thu, 09 Feb 2023 08:03:53 GMT  
		Size: 63.3 MB (63305330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0f7a8b3c9b4996e2ee9e65041bb5c8ea311482213b54d004d43cfa0da3bcf469
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144711239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a4114106d760615f32f4b575122bc6f8862f40d4c00e8535a1aa756c7b5014`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:54 GMT
ADD file:2c1195fd765d1da7082bf383b9c5ef0b244e5398006d53897d5ea40e919399f1 in / 
# Wed, 01 Mar 2023 04:47:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:31:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:31:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6800c47237e7f7a1e5340856e56ba98e2b69a475b2458bb2416fdb0582d8c28`  
		Last Modified: Wed, 01 Mar 2023 04:54:24 GMT  
		Size: 53.3 MB (53273011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff0fff502cf707b8386c45c579606a759f85d3b49c007814826ad27212fdf5`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 9.7 MB (9652015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ef4d32b9b5d605909945396d9e13b86c238ff2ea6c800b63cef6d06dc2d6a3`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 12.2 MB (12168382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecf54311632074a960030227c6fca18a718af9b2631164c5c93529e814a5f50`  
		Last Modified: Wed, 01 Mar 2023 05:41:38 GMT  
		Size: 69.6 MB (69617831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:384e64893747febf163fb0367883ec34308fc83212306707553bdb6011615410
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130757158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e16e9c63e3d82f943d4f4c6e591119c775a9709ea0848fa6fa822c3cf9f942`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:42 GMT
ADD file:a35d410eeff51ff3b7d9c823bc5ba421ef11373fb29ee93e8256efcbcdcee908 in / 
# Wed, 01 Mar 2023 02:50:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:16:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:16:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57e87143a56f85b3245b752ff94d616ef62e6372c0bcd9338b791267ea20f326`  
		Last Modified: Wed, 01 Mar 2023 02:55:04 GMT  
		Size: 47.6 MB (47629137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07cda735865838550e6455f8a76e842211afddfe8503e32aa744121e3435ae0`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 8.7 MB (8700269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c406447e84cbeb09410da5fd14cb6601c6f124b564b303a89c89e53406f68863`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 11.3 MB (11268803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b0879a47bff8d8b52a41d4dd0ceb2fa4313863026dfe04be33a743663128f8`  
		Last Modified: Wed, 01 Mar 2023 03:23:22 GMT  
		Size: 63.2 MB (63158949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:6fc33b1f1bc5e9d66a7cbbaab3f0de66bcdfee49fc51cdd7a1abe8f9e93a1640
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:stable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1ab51e666d5331b2ca90421dc657968b50de8c4ea86e747b51f24b0ceac6ee20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322486156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f6175124be93225950f0f44661e6d04c099685b1c6cfdce98c94b6908a005ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:43:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:44:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cdcd4942ebc7445d8a70117a83ecbc77dcc5ffc72c4b6f8e24c0c76cfee15d`  
		Last Modified: Wed, 01 Mar 2023 04:50:33 GMT  
		Size: 54.6 MB (54585443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3bce705f6c47c25b6e7896b4da514bf271c5827b1d19f51611c4a149dd713c`  
		Last Modified: Wed, 01 Mar 2023 04:51:08 GMT  
		Size: 196.8 MB (196811476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d5ebd7b5044f44ae29cf2301dc9d211d4a91de578f8643d9447e2705c89e1fa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295543491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25085575e82e41137aadeab7abf493a22196af92d25adbdd636b34ea590b35b8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:18:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:20:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d373aa541f88e7c81c88d63aca3fd07f01c6220ca295915af87f489a6cb251`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 5.1 MB (5072694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c176fe3230b5050ab13f5cd081fa601f679459e28449694496136a73bddd175c`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 10.6 MB (10573876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04072817b27c20dd9a7f9a0b93816bd195f8675845e235c0291c0f935824f610`  
		Last Modified: Wed, 01 Mar 2023 02:25:18 GMT  
		Size: 52.3 MB (52338815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6353168632306a6374c103fef267a9c6d96bb6102c9ad2cf73bbcd81093088a0`  
		Last Modified: Wed, 01 Mar 2023 02:25:56 GMT  
		Size: 175.0 MB (175008286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:68a9f7cc0785c70372cb8a12f4c245fc83255dabf264e6be54ff359ed27e2a40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (283008511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0390df189979c07f1a2462cc444b49d2112865ac9a6a1631e580a27b55539b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:33:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e676c4187d9dd900add9c8dd4b9c906be40a2b8db6cabfdaf280ac2e83cdfca`  
		Last Modified: Wed, 01 Mar 2023 03:09:35 GMT  
		Size: 50.4 MB (50355863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df966bf734b2531648679fbd424ead324e0892e75539a7b995ac958175ebd568`  
		Last Modified: Wed, 01 Mar 2023 03:10:10 GMT  
		Size: 167.3 MB (167288237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8917040dd4bb6aedfddba59aa82d51536b6ec25930b6f06c9733532a61912af2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.1 MB (314133809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2780396f13c4cbb69cfd74d843bc7bf52d0e90e5d9d9802e537a1a9769446f3a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:50:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8747d4a988af1d119e668971a87213d5c7061fc04671ba6fcb7123a1c11507ac`  
		Last Modified: Wed, 01 Mar 2023 02:56:37 GMT  
		Size: 54.7 MB (54676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb701404a7a0229719104b05970d81ecf0a7dea50b3defe137088db6cc3c0d0c`  
		Last Modified: Wed, 01 Mar 2023 02:57:06 GMT  
		Size: 189.7 MB (189727959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:151857e29bb1821d712ec7cfd8e4d8a5d883f37adea2a83c01a48cc2ac69239f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.2 MB (328218457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:038aa1836a9a96ce7b81933a91fa4831e0ba0d768de322b4835e86368581db36`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:10:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471482ade37b25d9ec22336d057dd4ed265a030b98595eac314b56d5709bbdff`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 5.3 MB (5293673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a995bf7fa061158e93790e264fd3bc4a3340e75bf857b3c51814384b5f1344f5`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 11.2 MB (11249844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9955e6ae7dba34d1170876e13f1c83b049619255f38babb22074d26848658318`  
		Last Modified: Wed, 01 Mar 2023 02:23:54 GMT  
		Size: 55.9 MB (55922655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc50efa640196b1840993873638e42246a1137dc3e2ac3534d6cba803fef33f`  
		Last Modified: Wed, 01 Mar 2023 02:24:42 GMT  
		Size: 199.7 MB (199724209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5ea0d35f075afa10f4b0b4cc10b69f2acc8c18ce4089182ad36a944bc68e2d38
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.2 MB (301151652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0222370846c985596fd3058856c6c93024191a6b9fc9adfbf00825509403dfbd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:42:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:47:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791a92fb38ebf78f5ed530cc39361869dd25ce941ea09d0580b866204f0e8e1`  
		Last Modified: Thu, 09 Feb 2023 07:59:50 GMT  
		Size: 4.9 MB (4921594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c347eddc487950d631dca4e7c20c1165566e8418703435fad325a721c0e8d`  
		Last Modified: Thu, 09 Feb 2023 07:59:52 GMT  
		Size: 10.7 MB (10662160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9ee56dfe2667a1d6574684709026d72883d1af28301257038f732b76362e9a`  
		Last Modified: Thu, 09 Feb 2023 08:00:40 GMT  
		Size: 53.3 MB (53307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec8851fe07613cc20ef37a5c4e83efee0eba7c47c653df09be97f187753970`  
		Last Modified: Thu, 09 Feb 2023 08:02:44 GMT  
		Size: 179.0 MB (178993425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bc66949fb3e5bb8519171d6c99462250e7c90213077a00562f8da2ad7567fdd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330990552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e22aacee9f5e429288440511032e88b59ac9b6015c67ad2859a1549cfdc03f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:01 GMT
ADD file:40523b7b16ccf1ff245b11e11f92d24e9e6e9dfbdbc755d4361cf55c7ec26244 in / 
# Wed, 01 Mar 2023 04:47:11 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:25:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:26:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:30:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b7949e1acd104233f80137ab3a92a148b0d48e41b3075c70a2d636c3b4c60bf`  
		Last Modified: Wed, 01 Mar 2023 04:53:18 GMT  
		Size: 58.9 MB (58921304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b3574e90831068a9bd9f64e57da92a087d925f0a0e63c764ecf421b18d3a1`  
		Last Modified: Wed, 01 Mar 2023 05:39:22 GMT  
		Size: 5.4 MB (5415247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8bec1f2d073d24de5e7dd051bcada4f0a407fc713e38b49fc2d2a863bde38e`  
		Last Modified: Wed, 01 Mar 2023 05:39:23 GMT  
		Size: 11.6 MB (11629925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3bc8a98c359709356de5d552e69a43170d7f81b4ad5ac17cfbb0eb8d3da2b1`  
		Last Modified: Wed, 01 Mar 2023 05:39:53 GMT  
		Size: 58.9 MB (58863932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266ad73c7e2640ed2a8bd13bc5ae4a7289e4d94678b520531d6e6a4c628b4936`  
		Last Modified: Wed, 01 Mar 2023 05:40:52 GMT  
		Size: 196.2 MB (196160144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8ced439af7f8f74e519890670464e8a54d02445b50906c0a580cb23381403b74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296068375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be656e6f4f9d501e5be96387e4ee7f13eed0dda7e92ac3582f1ba01b78338d6b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:07 GMT
ADD file:e5f01d8f88c8134571e8998672a504ecad259a9a8322df73aed4a93ffac08ebd in / 
# Wed, 01 Mar 2023 02:50:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:14:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:16:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51f6de0debe6daa552b12c9951f6529a870979d923187c1ba62ff66cee3450ac`  
		Last Modified: Wed, 01 Mar 2023 02:54:25 GMT  
		Size: 53.3 MB (53277694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6404e912b557d72a71a982115ad4b92e1c23918b7f0c950f6f22c2ec775ff936`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 5.1 MB (5149110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0561ee66ff6ae2ce12d922c3d0fed94e18a801571a2add9e526e914cb30a3bab`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 10.8 MB (10765987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c7ccf7cb532de1600bce9245b8e167d6d644608677c26601c246c4e80cdbf`  
		Last Modified: Wed, 01 Mar 2023 03:22:28 GMT  
		Size: 54.1 MB (54060191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2854c5c8fd871ba1d0f27ad51f05fba4d434683959e10cbe9fc7fb3281ec3415`  
		Last Modified: Wed, 01 Mar 2023 03:22:56 GMT  
		Size: 172.8 MB (172815393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:ec811d02884e77b7756e199aa29b0865fbff832fdb1b5f9e510ab1ec7059fbe0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:stable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fcea8a2b5af99f3d6240c4f8eb6bd3c30893eef1187fdcee771094c9dff6ae15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71089237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b9d6ef1ff1378d683604cf4ba99f8836f7e2f16205f16d0feee677d899d5f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:be1997f59f6670c0a7fc280c3d6359c5d34415bc035eb076dfd4bd5f03501c85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68196390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e730b28fdc731ae3aaca7b8b139d87185e0c39a2bd20b42109b12e72aa0236c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d373aa541f88e7c81c88d63aca3fd07f01c6220ca295915af87f489a6cb251`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 5.1 MB (5072694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c176fe3230b5050ab13f5cd081fa601f679459e28449694496136a73bddd175c`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 10.6 MB (10573876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:18d2756e7bcd00b93725240b830db6fe1095fc56d99228add890da041da1f64d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65364411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f10eddb1560f07c7bcfb9aae4af0d2ea57813820d425be262f39715ac534f490`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b0704702833d7486169b32592de4d7068ee216859e8120201ea440fa4b09d0bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69729485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff94eb1fb8fbc51d7ca80c6fc3291cde8e30e0e72289b6f6eaf32f54a0c6bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d92dd1d966478b3c6c0071bda6a468cf1459f49477c797452577f15e8810419b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72571593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5754a4da25c3b4c118346601bc5c735071a21e432587b386aa113af8f5d0e31`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471482ade37b25d9ec22336d057dd4ed265a030b98595eac314b56d5709bbdff`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 5.3 MB (5293673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a995bf7fa061158e93790e264fd3bc4a3340e75bf857b3c51814384b5f1344f5`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 11.2 MB (11249844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4b7b85b9386e8a62061db8f6de3d3f14d9c766b5afc78bce6a2277e61cb0d35e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68850538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e15959eca1ab694d171b213aa90363b529e588c0d215964cf8a4c3e6e8c0acc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791a92fb38ebf78f5ed530cc39361869dd25ce941ea09d0580b866204f0e8e1`  
		Last Modified: Thu, 09 Feb 2023 07:59:50 GMT  
		Size: 4.9 MB (4921594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c347eddc487950d631dca4e7c20c1165566e8418703435fad325a721c0e8d`  
		Last Modified: Thu, 09 Feb 2023 07:59:52 GMT  
		Size: 10.7 MB (10662160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5cf07060832cb3528f68597bf86a23931d11ca79238393925aa56a42aefbf2f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75966476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8505f47b3532655ea317846fe63792fa9fb98b85bd3bc950eba5cda1532a0a29`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:01 GMT
ADD file:40523b7b16ccf1ff245b11e11f92d24e9e6e9dfbdbc755d4361cf55c7ec26244 in / 
# Wed, 01 Mar 2023 04:47:11 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:25:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3b7949e1acd104233f80137ab3a92a148b0d48e41b3075c70a2d636c3b4c60bf`  
		Last Modified: Wed, 01 Mar 2023 04:53:18 GMT  
		Size: 58.9 MB (58921304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b3574e90831068a9bd9f64e57da92a087d925f0a0e63c764ecf421b18d3a1`  
		Last Modified: Wed, 01 Mar 2023 05:39:22 GMT  
		Size: 5.4 MB (5415247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8bec1f2d073d24de5e7dd051bcada4f0a407fc713e38b49fc2d2a863bde38e`  
		Last Modified: Wed, 01 Mar 2023 05:39:23 GMT  
		Size: 11.6 MB (11629925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ef8f8a6921a906b5f70110da039d2ba658262090af1f1082123d7adc15ea63f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69192791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905dee6c4c69217ff79bc7d612aa22e1d4d29c3735ff980996291dfc3677f416`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:07 GMT
ADD file:e5f01d8f88c8134571e8998672a504ecad259a9a8322df73aed4a93ffac08ebd in / 
# Wed, 01 Mar 2023 02:50:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:51f6de0debe6daa552b12c9951f6529a870979d923187c1ba62ff66cee3450ac`  
		Last Modified: Wed, 01 Mar 2023 02:54:25 GMT  
		Size: 53.3 MB (53277694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6404e912b557d72a71a982115ad4b92e1c23918b7f0c950f6f22c2ec775ff936`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 5.1 MB (5149110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0561ee66ff6ae2ce12d922c3d0fed94e18a801571a2add9e526e914cb30a3bab`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 10.8 MB (10765987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:f5efcf35ed707b7aeb078d6ddfdefc91a9715390a7d8003e51338f7d3630c941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:stable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a6ef7420ef5f9b158be970b586c122041efe47c340f36511af02b66b15f50021
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125674680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5069942e3d6eec75afd35fb58f4b25abd6e63a90e224fdfc1ef8b3db05d82130`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:43:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cdcd4942ebc7445d8a70117a83ecbc77dcc5ffc72c4b6f8e24c0c76cfee15d`  
		Last Modified: Wed, 01 Mar 2023 04:50:33 GMT  
		Size: 54.6 MB (54585443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e6642afa6470d719d40e0aedb05dcd82386c83ea9e49990ecd703001eea0708c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120535205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10cf2c6f88593a41cfd3f16b24bfee123e13190615f8330cee60375c884c9e4b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:18:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d373aa541f88e7c81c88d63aca3fd07f01c6220ca295915af87f489a6cb251`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 5.1 MB (5072694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c176fe3230b5050ab13f5cd081fa601f679459e28449694496136a73bddd175c`  
		Last Modified: Wed, 01 Mar 2023 02:24:55 GMT  
		Size: 10.6 MB (10573876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04072817b27c20dd9a7f9a0b93816bd195f8675845e235c0291c0f935824f610`  
		Last Modified: Wed, 01 Mar 2023 02:25:18 GMT  
		Size: 52.3 MB (52338815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c7076592183315790b451e7400610a2108a088eff9828031faacdc4ec0ef67b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115720274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adf4d1a818db1580563de9b22ed7fcc9738c034bdc78b5f4613ef9e96e02bd1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e676c4187d9dd900add9c8dd4b9c906be40a2b8db6cabfdaf280ac2e83cdfca`  
		Last Modified: Wed, 01 Mar 2023 03:09:35 GMT  
		Size: 50.4 MB (50355863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cf7219efab275bd3d3fbfd3ab95e7f321352cb3c012f6368843680ccb19abe5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124405850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf6eda9f040f4295ca3f9857f1ea0b5a1fdcc0cdb7491510b5223a2bf02530f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8747d4a988af1d119e668971a87213d5c7061fc04671ba6fcb7123a1c11507ac`  
		Last Modified: Wed, 01 Mar 2023 02:56:37 GMT  
		Size: 54.7 MB (54676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bf5cacb020595095738a86d659889e8825c9cee19c92064a670ddafcb6207a08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128494248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab6f0c472327c2c68c41ac703fb1caadce376b919f50c96745d2ae9165023bf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471482ade37b25d9ec22336d057dd4ed265a030b98595eac314b56d5709bbdff`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 5.3 MB (5293673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a995bf7fa061158e93790e264fd3bc4a3340e75bf857b3c51814384b5f1344f5`  
		Last Modified: Wed, 01 Mar 2023 02:23:29 GMT  
		Size: 11.2 MB (11249844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9955e6ae7dba34d1170876e13f1c83b049619255f38babb22074d26848658318`  
		Last Modified: Wed, 01 Mar 2023 02:23:54 GMT  
		Size: 55.9 MB (55922655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:07d501b1a244ee7c0ed6d4e9c5c5704cedd96cfb51bc776b2c778aec5bd274a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122158227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f882bdd498e5f8cf1f6bfe78012ad9b00c0b3e1d476d3b20a12bef5e08231e5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:42:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791a92fb38ebf78f5ed530cc39361869dd25ce941ea09d0580b866204f0e8e1`  
		Last Modified: Thu, 09 Feb 2023 07:59:50 GMT  
		Size: 4.9 MB (4921594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c347eddc487950d631dca4e7c20c1165566e8418703435fad325a721c0e8d`  
		Last Modified: Thu, 09 Feb 2023 07:59:52 GMT  
		Size: 10.7 MB (10662160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9ee56dfe2667a1d6574684709026d72883d1af28301257038f732b76362e9a`  
		Last Modified: Thu, 09 Feb 2023 08:00:40 GMT  
		Size: 53.3 MB (53307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8bd4ae58c5a9dd9152f3d51bfd815b98f2dbfec6309beb31666524144e8db6a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134830408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0053e746dde1fab6a1b0954f7f14f6d3a0eb7689b80f2ccaa15954b3b156e44c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:01 GMT
ADD file:40523b7b16ccf1ff245b11e11f92d24e9e6e9dfbdbc755d4361cf55c7ec26244 in / 
# Wed, 01 Mar 2023 04:47:11 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:25:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:26:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b7949e1acd104233f80137ab3a92a148b0d48e41b3075c70a2d636c3b4c60bf`  
		Last Modified: Wed, 01 Mar 2023 04:53:18 GMT  
		Size: 58.9 MB (58921304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b3574e90831068a9bd9f64e57da92a087d925f0a0e63c764ecf421b18d3a1`  
		Last Modified: Wed, 01 Mar 2023 05:39:22 GMT  
		Size: 5.4 MB (5415247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8bec1f2d073d24de5e7dd051bcada4f0a407fc713e38b49fc2d2a863bde38e`  
		Last Modified: Wed, 01 Mar 2023 05:39:23 GMT  
		Size: 11.6 MB (11629925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3bc8a98c359709356de5d552e69a43170d7f81b4ad5ac17cfbb0eb8d3da2b1`  
		Last Modified: Wed, 01 Mar 2023 05:39:53 GMT  
		Size: 58.9 MB (58863932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f26531b6a394a77d086c8d03202eddded5c7e44b39da743ad759ba173721a941
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123252982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab21b2830a2681e63ef03f163b5c2437190e155339ff1e3db316ff358b283e3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:07 GMT
ADD file:e5f01d8f88c8134571e8998672a504ecad259a9a8322df73aed4a93ffac08ebd in / 
# Wed, 01 Mar 2023 02:50:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:14:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:51f6de0debe6daa552b12c9951f6529a870979d923187c1ba62ff66cee3450ac`  
		Last Modified: Wed, 01 Mar 2023 02:54:25 GMT  
		Size: 53.3 MB (53277694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6404e912b557d72a71a982115ad4b92e1c23918b7f0c950f6f22c2ec775ff936`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 5.1 MB (5149110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0561ee66ff6ae2ce12d922c3d0fed94e18a801571a2add9e526e914cb30a3bab`  
		Last Modified: Wed, 01 Mar 2023 03:22:11 GMT  
		Size: 10.8 MB (10765987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c7ccf7cb532de1600bce9245b8e167d6d644608677c26601c246c4e80cdbf`  
		Last Modified: Wed, 01 Mar 2023 03:22:28 GMT  
		Size: 54.1 MB (54060191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:6028d65928c1f2cc6fd1d75a1b33eed8a49da8b88d92a0d871a72b89128ca400
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:195681bdeac6045bdaae7f1c8a3d555ef169b6200ef761cde689fd8e5ebc1544
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.7 MB (344673834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4434dc6ee1bad5f222d7d8e7ce697a1f5dc4fbc07f8f595bec3f1f7d3697ec47`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:21 GMT
ADD file:74b4e0fbcb9cb38344c32a0512a72d8179f885de4b7bb127215f8d96a6262664 in / 
# Wed, 01 Mar 2023 04:09:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:40:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d915a4248d2913bb8451eba978ac348a983990eca9186543367f5f44900e0fb`  
		Last Modified: Wed, 01 Mar 2023 04:13:25 GMT  
		Size: 49.2 MB (49237273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012774ea2ca6d41295cf7bc05a82ac4aa9183dd2ce4f4c0584b549d922ef6b2e`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 9.0 MB (9049510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871c0f2b6b6518e6675004eb4ccd8a8d77105f4f1d83d8f0d0168b16f544ffbe`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 11.4 MB (11405791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df7f0c3bf5351a2fa63ae6776d5565929b9afb539c689cadd1e415b1751f478`  
		Last Modified: Wed, 01 Mar 2023 04:49:31 GMT  
		Size: 64.1 MB (64094287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7b30ee362037144052a76832c9fb5838292f13214d0adcce12770da6ebef28`  
		Last Modified: Wed, 01 Mar 2023 04:50:05 GMT  
		Size: 210.9 MB (210886973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6020af7ec13e1b5c9b5a69273fee42ba9794d8fbebc5b1cd02cf1ee36c7fc9fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.4 MB (313404899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a30408ef722d243b15667eb01103cf5a198e0540e6c3dabf09a3068a7bf151`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:24 GMT
ADD file:1685939a153ab7a7aa03035565c60e99663abd3a416ef0d00bddaf24e0ae6f08 in / 
# Wed, 01 Mar 2023 01:48:25 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:15:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:17:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f7516928cdf57280d137bb31220dd9f0b6ca54e290189b42a68ab64d0d2065b7`  
		Last Modified: Wed, 01 Mar 2023 01:51:43 GMT  
		Size: 48.1 MB (48072838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402a03a1c745fc42a93ed0082abf13d52e0c961da496b7b2d7d9a60a1d8031f`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 8.5 MB (8496389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea6f1f01cbcb26c4e22bf2c443b3515e57d9267d84661daeb7ae809ff62ff82`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 11.1 MB (11051495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db38c030ddb0562da5b6a4ed2e4333299c295c785959c19faae6aecfee04f841`  
		Last Modified: Wed, 01 Mar 2023 02:24:07 GMT  
		Size: 61.5 MB (61520999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca85168741ee98a96b0dd356f399b344b82fee50e8e9efd731252ebe921ef5b`  
		Last Modified: Wed, 01 Mar 2023 02:24:43 GMT  
		Size: 184.3 MB (184263178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7bf5be439e3fda124e262e33b08707f2ca5141674cde6b7714cd35627da86d16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.8 MB (298825417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6e75b174f39ba61336f8b77fb439838425edd2ef79572e33b69628b8cff7060`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:26 GMT
ADD file:9f8ce83cf3e75c63cb351ec688378ffe29d7105ff8e8892b3cef95aeacbf6779 in / 
# Wed, 01 Mar 2023 01:57:27 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:28:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:29:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:31:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c5d14f15cd67359c9f8d5dbc636ce6ffee972aa4acbeb663e40e865b0dd7dee`  
		Last Modified: Wed, 01 Mar 2023 02:01:54 GMT  
		Size: 45.8 MB (45843301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925df4d36e5e8049cacb403582ac8832aed842417020be560ab0398e08c8fb67`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 8.1 MB (8140837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5921afe59294ea6e26c9a0c8c143bce276da4ba83ef2f7194b96d034a2b463d`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 10.7 MB (10687660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daffa30bd41618c0f8d8bc932ac6b2e541af6a12c3462963570690c046fb0eb`  
		Last Modified: Wed, 01 Mar 2023 03:08:25 GMT  
		Size: 59.2 MB (59228783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50887d27d71d122cc7300c13322d74bde98f553f7cf135b1505f230f518673f`  
		Last Modified: Wed, 01 Mar 2023 03:09:01 GMT  
		Size: 174.9 MB (174924836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d7ffe8d49a7b80dcc5663e150f752387a766b3b53160652991c0ab26d07643fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335767410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18c2cda0cb0dac04945795df83d91094f7b8f7a976279c2b80ccdd1a54abcd98`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:13 GMT
ADD file:5b81699b80066f9e3bc967bdf130a67f54ebe15cd80df6c952262d6132b1cabf in / 
# Wed, 01 Mar 2023 02:20:14 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:46:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:47:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:48:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf639a903cc04a00c81ac77b3b9f9a79644c51b7f515895fd60403c20ff34a80`  
		Last Modified: Wed, 01 Mar 2023 02:23:22 GMT  
		Size: 49.3 MB (49273990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42632d5ac93ac504d393018f5e0f56f02bedd9cd2df6e1d91da9fc0ef4806d9b`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 8.9 MB (8882130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c0a0685e10806d6ca5aac08337a76d9fd6a47f16f665f5d3a2e692eabfeb3f`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 11.4 MB (11371530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1ccc2a9c1e986768a01b08e1009a75262c8bac308f9c9d414685034ce162c1`  
		Last Modified: Wed, 01 Mar 2023 02:55:40 GMT  
		Size: 63.9 MB (63942296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6498018d1c1322fabda196170f7912e9dcca825fed9a4aec837be082b1b225fb`  
		Last Modified: Wed, 01 Mar 2023 02:56:09 GMT  
		Size: 202.3 MB (202297464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bfe43663f0657294ca025418f275e8e909e49dc6114c520c8c1b8c0f2bf064d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.1 MB (347082902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f9b45267606b6b6a34d9882904bfc4bd4fbaa171ab797bf69b5fd7109e2efbb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:38:40 GMT
ADD file:0ccdbb7b1f104c23abcf77c506eed771d5759d210c2284a95f85e558405a5390 in / 
# Wed, 01 Mar 2023 01:38:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:05:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:05:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b5ba6d7d02dd42cc6291ae5b4e129956756f664662a78db71f320107a1b6d189`  
		Last Modified: Wed, 01 Mar 2023 01:43:30 GMT  
		Size: 50.3 MB (50273396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f35c12f0528f81569a1c99e040f4d3527ee4391aa4079d740a4c6638bcece0`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 9.2 MB (9230996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319f35836381f914f3bbf4d55b955e9cf90a83165b64e829c72b52051b5e5c5`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 11.8 MB (11808790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a8ff813204e629160f019ffdb45960b87b39f586133418d3fd5f36323e5f03`  
		Last Modified: Wed, 01 Mar 2023 02:22:30 GMT  
		Size: 65.9 MB (65937993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8466c42e65a0d855e2465ff126267c143a76b83ccd4d4770213c0472a28557ae`  
		Last Modified: Wed, 01 Mar 2023 02:23:17 GMT  
		Size: 209.8 MB (209831727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c57a7f1ec7adfe8459654df4f071d8f4d79ec1a0316240f76409fc967eb537ba
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321227952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5849000d7db598292b11707a555bbb2b5de9bbd7035008cf9f52e0e35e9d58f0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:43:09 GMT
ADD file:bff5ae942e6561f2afffbbd0267d57706f7fdd71ebe43c64b369b20940d55f00 in / 
# Thu, 09 Feb 2023 02:43:14 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:31:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:32:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:33:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:39:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aa6addfe979ac43879ea9517851622f7a6c1516568fbd6a0c101c3b86cc1163`  
		Last Modified: Thu, 09 Feb 2023 02:51:51 GMT  
		Size: 49.1 MB (49063446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6db93799880bf6f9525fc696324e0d450fd37ebbb37d356955a9057236da38`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 8.4 MB (8399010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b19fed47eb69b023968097b12ef67cad0d7e15a03675cc16e3efc9b67a44e4`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 11.1 MB (11105521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7152f2a237e2d177c5dc02d27a4b1e0433902b36280eb92369c2a9e5620678e`  
		Last Modified: Thu, 09 Feb 2023 07:57:24 GMT  
		Size: 63.3 MB (63307246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7ff536332669177f30e959f391f586eaf9b5c716f81f9a50b31c0c1ce869d6`  
		Last Modified: Thu, 09 Feb 2023 07:59:38 GMT  
		Size: 189.4 MB (189352729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d5e1db6aed979d645af6fee7361c5a23b34c1d43584bf4db444cc8bfde6221a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.5 MB (358527778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe7a5c69cddd5f8e4e1b828ca19c143392e37b1cd9c29f6b9ae04774856707e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:46:00 GMT
ADD file:311d9174b941eeaaa2babe3a94b035ab7c3880d5908d630bdec420f42eff6a06 in / 
# Wed, 01 Mar 2023 04:46:05 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:18:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:18:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:20:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:24:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6b61b4a96c9a944bd44d67cc885cdb2ef5f9aa35a0a94dba6ea2b6372ad27e48`  
		Last Modified: Wed, 01 Mar 2023 04:52:26 GMT  
		Size: 53.3 MB (53250230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a057e1f93c20f3bf648ce49e3455619f0854aef331a7d297c7425e435adfcb8`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 9.6 MB (9631581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb4683b31216d30e252186c2c0cb6f06f69d737321cb3d95c8f1036adca0bea`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 12.2 MB (12168325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18e9322efa86ed752abe3ce6c6627d95fb158f9e6fc57b15a1dd5c4eeac07ae`  
		Last Modified: Wed, 01 Mar 2023 05:38:09 GMT  
		Size: 69.5 MB (69538650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0dfbe78692a54c80a5b039ccab3594a7e5bd520477c34ff0871e776ced27bb`  
		Last Modified: Wed, 01 Mar 2023 05:39:11 GMT  
		Size: 213.9 MB (213938992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2746edcd036ffa0e80571e197771eb53a1e7d407da3edb91126e6256b418c611
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313638662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d1cd40898cf919229eebdad2f4a408e5b37c0c37062ab7763759c8d26d4ae52`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:49:37 GMT
ADD file:55baf50ca3524103dfcb38a8784744d482a5cdb19f66a7baa92d44dc18483a58 in / 
# Wed, 01 Mar 2023 02:49:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:12:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:14:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e95e47ef2a5cde1145fe4af2db22dbfe40c09cf83dbb9ff00d400d23e6dd5331`  
		Last Modified: Wed, 01 Mar 2023 02:53:58 GMT  
		Size: 47.6 MB (47608102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf204e7b8be3c288518bf65a248e94d7d77b56c235d30b3eb93058f663337226`  
		Last Modified: Wed, 01 Mar 2023 03:21:19 GMT  
		Size: 8.7 MB (8684339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca66d3959e328f7d96d65cb0b1a3f79c9c7f949a2fefecdadb692344f6e8a5b`  
		Last Modified: Wed, 01 Mar 2023 03:21:18 GMT  
		Size: 11.3 MB (11268858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb5857b88499838945e97d7c6a6c6ebe9e8cedf2f9e53fd3969022b50bafb3c`  
		Last Modified: Wed, 01 Mar 2023 03:21:34 GMT  
		Size: 63.1 MB (63088618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7a497c30bac5956b1d898cc4c280377487b7b0abb58817eed64f480bb4fb69`  
		Last Modified: Wed, 01 Mar 2023 03:22:03 GMT  
		Size: 183.0 MB (182988745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:c8f091cd0bdf8be224eb2fe67d5861723a681b2a0aead26099000373f5bd2b9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d4b35a63544657e87fe7761075ad7fc9666a5d864314a5d931be9bd6c7f9ef54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69692574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3d26fafdceaae720d412163f42c2d209fac53ec665bc89ce3d048ebcbbe1f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:21 GMT
ADD file:74b4e0fbcb9cb38344c32a0512a72d8179f885de4b7bb127215f8d96a6262664 in / 
# Wed, 01 Mar 2023 04:09:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:40:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9d915a4248d2913bb8451eba978ac348a983990eca9186543367f5f44900e0fb`  
		Last Modified: Wed, 01 Mar 2023 04:13:25 GMT  
		Size: 49.2 MB (49237273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012774ea2ca6d41295cf7bc05a82ac4aa9183dd2ce4f4c0584b549d922ef6b2e`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 9.0 MB (9049510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871c0f2b6b6518e6675004eb4ccd8a8d77105f4f1d83d8f0d0168b16f544ffbe`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 11.4 MB (11405791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:62c8e4b2d3cb76df9cd0da0c61644cfd48542f5dcab0f8876ac5006f197b466b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67620722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302c483085eabc43b0bc26a0ec3388ba8bd6e850b6aaf90bee3067eb1b06e29d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:24 GMT
ADD file:1685939a153ab7a7aa03035565c60e99663abd3a416ef0d00bddaf24e0ae6f08 in / 
# Wed, 01 Mar 2023 01:48:25 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f7516928cdf57280d137bb31220dd9f0b6ca54e290189b42a68ab64d0d2065b7`  
		Last Modified: Wed, 01 Mar 2023 01:51:43 GMT  
		Size: 48.1 MB (48072838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402a03a1c745fc42a93ed0082abf13d52e0c961da496b7b2d7d9a60a1d8031f`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 8.5 MB (8496389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea6f1f01cbcb26c4e22bf2c443b3515e57d9267d84661daeb7ae809ff62ff82`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 11.1 MB (11051495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:89d5b8cad9b7628091dc315c80ac73032be23c33ffc20a54daa4494c2b869d0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64671798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4424c860db17396c58ff3e4f5cc348d934583867019f1491602086ce7f289e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:26 GMT
ADD file:9f8ce83cf3e75c63cb351ec688378ffe29d7105ff8e8892b3cef95aeacbf6779 in / 
# Wed, 01 Mar 2023 01:57:27 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:28:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4c5d14f15cd67359c9f8d5dbc636ce6ffee972aa4acbeb663e40e865b0dd7dee`  
		Last Modified: Wed, 01 Mar 2023 02:01:54 GMT  
		Size: 45.8 MB (45843301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925df4d36e5e8049cacb403582ac8832aed842417020be560ab0398e08c8fb67`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 8.1 MB (8140837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5921afe59294ea6e26c9a0c8c143bce276da4ba83ef2f7194b96d034a2b463d`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 10.7 MB (10687660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:de24f24c37e458d6b286a7c11bfa15cdcbc2c98af24cb1b5d4ca4d41fe220b93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69527650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1935824d13726e2507f35f1e2b012cdc815e6923d82f8ef0dad82ae11e50138`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:13 GMT
ADD file:5b81699b80066f9e3bc967bdf130a67f54ebe15cd80df6c952262d6132b1cabf in / 
# Wed, 01 Mar 2023 02:20:14 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:46:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cf639a903cc04a00c81ac77b3b9f9a79644c51b7f515895fd60403c20ff34a80`  
		Last Modified: Wed, 01 Mar 2023 02:23:22 GMT  
		Size: 49.3 MB (49273990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42632d5ac93ac504d393018f5e0f56f02bedd9cd2df6e1d91da9fc0ef4806d9b`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 8.9 MB (8882130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c0a0685e10806d6ca5aac08337a76d9fd6a47f16f665f5d3a2e692eabfeb3f`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 11.4 MB (11371530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0cd5d6206f9f4c2d947dad0bfb51b68944ebe17cf3baf558cc906cb8a3467117
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71313182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78a3dfaf671eb3aee58f8b6339b0f8dc5fcc24c896f58aded93920c474c13e83`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:38:40 GMT
ADD file:0ccdbb7b1f104c23abcf77c506eed771d5759d210c2284a95f85e558405a5390 in / 
# Wed, 01 Mar 2023 01:38:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:05:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b5ba6d7d02dd42cc6291ae5b4e129956756f664662a78db71f320107a1b6d189`  
		Last Modified: Wed, 01 Mar 2023 01:43:30 GMT  
		Size: 50.3 MB (50273396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f35c12f0528f81569a1c99e040f4d3527ee4391aa4079d740a4c6638bcece0`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 9.2 MB (9230996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319f35836381f914f3bbf4d55b955e9cf90a83165b64e829c72b52051b5e5c5`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 11.8 MB (11808790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2fbb3255f217e7530d462b4aacaaa94d13346677c94e5283617b6f03c701cf36
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68567977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:debaa28c7b7c6c9f25d29679aa12d4fcce59bc201a8da4940981fd15ac5ec342`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:43:09 GMT
ADD file:bff5ae942e6561f2afffbbd0267d57706f7fdd71ebe43c64b369b20940d55f00 in / 
# Thu, 09 Feb 2023 02:43:14 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:31:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:32:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9aa6addfe979ac43879ea9517851622f7a6c1516568fbd6a0c101c3b86cc1163`  
		Last Modified: Thu, 09 Feb 2023 02:51:51 GMT  
		Size: 49.1 MB (49063446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6db93799880bf6f9525fc696324e0d450fd37ebbb37d356955a9057236da38`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 8.4 MB (8399010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b19fed47eb69b023968097b12ef67cad0d7e15a03675cc16e3efc9b67a44e4`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 11.1 MB (11105521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:36f29f426e14bbe0de3f0f8ec7ca53855abbdbc9166223f63f386475adb95a3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75050136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca0a733a8ebc11612b7086f5d280d94b7bb2a33ff7f588e472fb573dca062ba0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:46:00 GMT
ADD file:311d9174b941eeaaa2babe3a94b035ab7c3880d5908d630bdec420f42eff6a06 in / 
# Wed, 01 Mar 2023 04:46:05 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:18:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:18:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6b61b4a96c9a944bd44d67cc885cdb2ef5f9aa35a0a94dba6ea2b6372ad27e48`  
		Last Modified: Wed, 01 Mar 2023 04:52:26 GMT  
		Size: 53.3 MB (53250230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a057e1f93c20f3bf648ce49e3455619f0854aef331a7d297c7425e435adfcb8`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 9.6 MB (9631581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb4683b31216d30e252186c2c0cb6f06f69d737321cb3d95c8f1036adca0bea`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 12.2 MB (12168325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f2a5b2e26281c3af1970a2678213fa7f844b2177a0acf92329b9ba345095af29
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67561299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be9d847d83a7f68910f5e39bea22c25f248156368cdfc6bb475d02073299fdc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:49:37 GMT
ADD file:55baf50ca3524103dfcb38a8784744d482a5cdb19f66a7baa92d44dc18483a58 in / 
# Wed, 01 Mar 2023 02:49:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:12:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e95e47ef2a5cde1145fe4af2db22dbfe40c09cf83dbb9ff00d400d23e6dd5331`  
		Last Modified: Wed, 01 Mar 2023 02:53:58 GMT  
		Size: 47.6 MB (47608102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf204e7b8be3c288518bf65a248e94d7d77b56c235d30b3eb93058f663337226`  
		Last Modified: Wed, 01 Mar 2023 03:21:19 GMT  
		Size: 8.7 MB (8684339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca66d3959e328f7d96d65cb0b1a3f79c9c7f949a2fefecdadb692344f6e8a5b`  
		Last Modified: Wed, 01 Mar 2023 03:21:18 GMT  
		Size: 11.3 MB (11268858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:6010adfdd68330d5cc75103f4204b81cbd0975c60b82d835e0bf7660febf6864
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7672703ae082615e986385b91c9fa35429dde626233955b38d57cd672e8220e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133786861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da1325778cc479069b68fd4bbf41083893a5ce9810f4735b36ddb24809bbcdcd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:21 GMT
ADD file:74b4e0fbcb9cb38344c32a0512a72d8179f885de4b7bb127215f8d96a6262664 in / 
# Wed, 01 Mar 2023 04:09:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:40:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d915a4248d2913bb8451eba978ac348a983990eca9186543367f5f44900e0fb`  
		Last Modified: Wed, 01 Mar 2023 04:13:25 GMT  
		Size: 49.2 MB (49237273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012774ea2ca6d41295cf7bc05a82ac4aa9183dd2ce4f4c0584b549d922ef6b2e`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 9.0 MB (9049510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871c0f2b6b6518e6675004eb4ccd8a8d77105f4f1d83d8f0d0168b16f544ffbe`  
		Last Modified: Wed, 01 Mar 2023 04:49:14 GMT  
		Size: 11.4 MB (11405791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df7f0c3bf5351a2fa63ae6776d5565929b9afb539c689cadd1e415b1751f478`  
		Last Modified: Wed, 01 Mar 2023 04:49:31 GMT  
		Size: 64.1 MB (64094287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e368a980ce07d0d05c407f5f83fd7eaa214a94ab89a68fd65bcc72113d126c75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129141721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f1ccaedc02174ef64b93a8f0f326ec4ffec1458f1c54768a5da3d2e53c616d2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:24 GMT
ADD file:1685939a153ab7a7aa03035565c60e99663abd3a416ef0d00bddaf24e0ae6f08 in / 
# Wed, 01 Mar 2023 01:48:25 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:15:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f7516928cdf57280d137bb31220dd9f0b6ca54e290189b42a68ab64d0d2065b7`  
		Last Modified: Wed, 01 Mar 2023 01:51:43 GMT  
		Size: 48.1 MB (48072838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b402a03a1c745fc42a93ed0082abf13d52e0c961da496b7b2d7d9a60a1d8031f`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 8.5 MB (8496389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea6f1f01cbcb26c4e22bf2c443b3515e57d9267d84661daeb7ae809ff62ff82`  
		Last Modified: Wed, 01 Mar 2023 02:23:46 GMT  
		Size: 11.1 MB (11051495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db38c030ddb0562da5b6a4ed2e4333299c295c785959c19faae6aecfee04f841`  
		Last Modified: Wed, 01 Mar 2023 02:24:07 GMT  
		Size: 61.5 MB (61520999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9363999a5ced7319bb4e8233919bcf696a5ff06ce055f6ff25cddc125630fe82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123900581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14baa6809f04057f886b38600982f1e5bbe9c414e11e8a016f729d70ff9ded84`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:26 GMT
ADD file:9f8ce83cf3e75c63cb351ec688378ffe29d7105ff8e8892b3cef95aeacbf6779 in / 
# Wed, 01 Mar 2023 01:57:27 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:28:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:29:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c5d14f15cd67359c9f8d5dbc636ce6ffee972aa4acbeb663e40e865b0dd7dee`  
		Last Modified: Wed, 01 Mar 2023 02:01:54 GMT  
		Size: 45.8 MB (45843301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925df4d36e5e8049cacb403582ac8832aed842417020be560ab0398e08c8fb67`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 8.1 MB (8140837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5921afe59294ea6e26c9a0c8c143bce276da4ba83ef2f7194b96d034a2b463d`  
		Last Modified: Wed, 01 Mar 2023 03:08:02 GMT  
		Size: 10.7 MB (10687660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daffa30bd41618c0f8d8bc932ac6b2e541af6a12c3462963570690c046fb0eb`  
		Last Modified: Wed, 01 Mar 2023 03:08:25 GMT  
		Size: 59.2 MB (59228783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:707d81e8f30e61d9f2aaa457f83a07eae8b2a592a62b58d3d7e9d83da5975f8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133469946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f6c7e35dd573abe7c4284cb4996d045b058236c5962edd7424453357d4c3c5a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:13 GMT
ADD file:5b81699b80066f9e3bc967bdf130a67f54ebe15cd80df6c952262d6132b1cabf in / 
# Wed, 01 Mar 2023 02:20:14 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:46:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:47:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf639a903cc04a00c81ac77b3b9f9a79644c51b7f515895fd60403c20ff34a80`  
		Last Modified: Wed, 01 Mar 2023 02:23:22 GMT  
		Size: 49.3 MB (49273990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42632d5ac93ac504d393018f5e0f56f02bedd9cd2df6e1d91da9fc0ef4806d9b`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 8.9 MB (8882130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c0a0685e10806d6ca5aac08337a76d9fd6a47f16f665f5d3a2e692eabfeb3f`  
		Last Modified: Wed, 01 Mar 2023 02:55:25 GMT  
		Size: 11.4 MB (11371530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1ccc2a9c1e986768a01b08e1009a75262c8bac308f9c9d414685034ce162c1`  
		Last Modified: Wed, 01 Mar 2023 02:55:40 GMT  
		Size: 63.9 MB (63942296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ae8e961a9e40fd1cc67a16b2eeb562541342ae4bdaa1e6a49ac66fb1484f8e96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137251175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c2068c6e1d78739e77ceabcc05f5cb988caed03f0c045bd5c99279abfe372a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:38:40 GMT
ADD file:0ccdbb7b1f104c23abcf77c506eed771d5759d210c2284a95f85e558405a5390 in / 
# Wed, 01 Mar 2023 01:38:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:05:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:05:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b5ba6d7d02dd42cc6291ae5b4e129956756f664662a78db71f320107a1b6d189`  
		Last Modified: Wed, 01 Mar 2023 01:43:30 GMT  
		Size: 50.3 MB (50273396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f35c12f0528f81569a1c99e040f4d3527ee4391aa4079d740a4c6638bcece0`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 9.2 MB (9230996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319f35836381f914f3bbf4d55b955e9cf90a83165b64e829c72b52051b5e5c5`  
		Last Modified: Wed, 01 Mar 2023 02:22:07 GMT  
		Size: 11.8 MB (11808790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a8ff813204e629160f019ffdb45960b87b39f586133418d3fd5f36323e5f03`  
		Last Modified: Wed, 01 Mar 2023 02:22:30 GMT  
		Size: 65.9 MB (65937993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:58f7776ae5802beb5ff95c124b893ff3a2ce121f93e98d305337e9feeeb340d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131875223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dde5105ffa4ba49e36c8a2afa67c343d1f83bde2ad9dde91a2a56b5056c6d4f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:43:09 GMT
ADD file:bff5ae942e6561f2afffbbd0267d57706f7fdd71ebe43c64b369b20940d55f00 in / 
# Thu, 09 Feb 2023 02:43:14 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:31:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:32:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:33:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aa6addfe979ac43879ea9517851622f7a6c1516568fbd6a0c101c3b86cc1163`  
		Last Modified: Thu, 09 Feb 2023 02:51:51 GMT  
		Size: 49.1 MB (49063446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6db93799880bf6f9525fc696324e0d450fd37ebbb37d356955a9057236da38`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 8.4 MB (8399010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b19fed47eb69b023968097b12ef67cad0d7e15a03675cc16e3efc9b67a44e4`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 11.1 MB (11105521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7152f2a237e2d177c5dc02d27a4b1e0433902b36280eb92369c2a9e5620678e`  
		Last Modified: Thu, 09 Feb 2023 07:57:24 GMT  
		Size: 63.3 MB (63307246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ebef91cd94f5561186fb0b696247790d031846171cfc5662c9592c36adce5858
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144588786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524c9ee0845a8c69cf6771af7edf1490f94ce4d0dda21968e413a26752e9b320`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:46:00 GMT
ADD file:311d9174b941eeaaa2babe3a94b035ab7c3880d5908d630bdec420f42eff6a06 in / 
# Wed, 01 Mar 2023 04:46:05 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:18:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:18:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:20:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6b61b4a96c9a944bd44d67cc885cdb2ef5f9aa35a0a94dba6ea2b6372ad27e48`  
		Last Modified: Wed, 01 Mar 2023 04:52:26 GMT  
		Size: 53.3 MB (53250230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a057e1f93c20f3bf648ce49e3455619f0854aef331a7d297c7425e435adfcb8`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 9.6 MB (9631581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb4683b31216d30e252186c2c0cb6f06f69d737321cb3d95c8f1036adca0bea`  
		Last Modified: Wed, 01 Mar 2023 05:37:40 GMT  
		Size: 12.2 MB (12168325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18e9322efa86ed752abe3ce6c6627d95fb158f9e6fc57b15a1dd5c4eeac07ae`  
		Last Modified: Wed, 01 Mar 2023 05:38:09 GMT  
		Size: 69.5 MB (69538650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:70d660b84d8823209adb0b68ba88f2b2bec7a47b14c638270edbc9242cb64841
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130649917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e1f38dc04be68c2fbe7138cf87bcdf1c061ef8a1f11fb0e2353575347e48b18`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:49:37 GMT
ADD file:55baf50ca3524103dfcb38a8784744d482a5cdb19f66a7baa92d44dc18483a58 in / 
# Wed, 01 Mar 2023 02:49:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:12:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e95e47ef2a5cde1145fe4af2db22dbfe40c09cf83dbb9ff00d400d23e6dd5331`  
		Last Modified: Wed, 01 Mar 2023 02:53:58 GMT  
		Size: 47.6 MB (47608102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf204e7b8be3c288518bf65a248e94d7d77b56c235d30b3eb93058f663337226`  
		Last Modified: Wed, 01 Mar 2023 03:21:19 GMT  
		Size: 8.7 MB (8684339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca66d3959e328f7d96d65cb0b1a3f79c9c7f949a2fefecdadb692344f6e8a5b`  
		Last Modified: Wed, 01 Mar 2023 03:21:18 GMT  
		Size: 11.3 MB (11268858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb5857b88499838945e97d7c6a6c6ebe9e8cedf2f9e53fd3969022b50bafb3c`  
		Last Modified: Wed, 01 Mar 2023 03:21:34 GMT  
		Size: 63.1 MB (63088618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:a8e1957e6cdefeacc8d7a0099162f76da0746af71529e78f7d56e4e60ab1b44e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4cf68c882cee9b417142c8f85e20e26fcdb0fa83cc0f991801de65462df2f4cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.8 MB (344815719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f756652badfd81aa904ebea98fc74ac8af051853f59e0e07e17c01a6fe5fd60`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:57 GMT
ADD file:742621d60641957542e01d843bc130e616ba577a7135783b21e53d3a5d77ad5b in / 
# Wed, 01 Mar 2023 04:10:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:46:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:46:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:47:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d80cbe2ffd4f13cce276662ea5b4fa412791129d545137a4bea79fc41c446e0b`  
		Last Modified: Wed, 01 Mar 2023 04:15:57 GMT  
		Size: 49.3 MB (49261286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414a406365e2c651e77ea1d2dedd2c2fe7317552757dfc2701d2cdf6a578a51e`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 9.1 MB (9063535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515af3674ccc4fa7b84288322c2d1250d4de5952aafb54a33baeaf74fb694632`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 11.4 MB (11405848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4328fcba3826a509a956e5614c022c05ed89b4e718a69b607176d4a8f97f0e86`  
		Last Modified: Wed, 01 Mar 2023 04:52:36 GMT  
		Size: 64.2 MB (64156733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf5761bef1786d1a3043cfdd4502ded7b68eb76cddebebdfd5e61420f1ab445`  
		Last Modified: Wed, 01 Mar 2023 04:53:10 GMT  
		Size: 210.9 MB (210928317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cfab3ca8a8f26671e80ccdb59dd4ba9f96d324240fab5eca7fda5b7282e680d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.5 MB (313512864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98658392247eaba632e8d135986bbf3cb581ed4c064c7c09cc42508038e13052`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:01 GMT
ADD file:4fadb88d3ead8d91349c79d7e903bbb8f6130b292bda6cb8099131210a815bc1 in / 
# Wed, 01 Mar 2023 01:49:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:21:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:21:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:22:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03e1abdb2ebe924d64faf35eb6563891039999ec54a62f65419caf539ba6a88`  
		Last Modified: Wed, 01 Mar 2023 01:53:21 GMT  
		Size: 48.1 MB (48107781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d446d9cfc1201a906803d21a6e36423e22e9bebf24cf64bd16a4a3a73af61a2`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 8.5 MB (8514426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dc22595c5f06cd6d232ff8a3594b9aadef31095cb355dffad2b48a861717bf`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 11.1 MB (11051502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0760e34b5fee30fa55ba71775caf6a3b2e755775ea03be4db0c03e5d83ff0a3`  
		Last Modified: Wed, 01 Mar 2023 02:26:32 GMT  
		Size: 61.6 MB (61563988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0bee41572d3fd2c79c2cec17ba9f302c4197090c7cd926637454ea269c1fcf`  
		Last Modified: Wed, 01 Mar 2023 02:27:08 GMT  
		Size: 184.3 MB (184275167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4fd065ebb7280f186e201ef931745f11b0ed5709bb74ebfce845fa07383b77de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.9 MB (298924502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb866bf86688fd657c0d0bbb77f601dc7b5b740627aacc2b35cdb24985d07cd5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:39 GMT
ADD file:2cc322ac43103c8e367e39beaccf285da593ce4935ec4b1c90ae321a43b7123b in / 
# Wed, 01 Mar 2023 01:58:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:37:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:37:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:38:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e5967747d4d88696bd5d5f37c0b5b8bcf8b29f3b448f6d1dd9623bdcc655965`  
		Last Modified: Wed, 01 Mar 2023 02:04:52 GMT  
		Size: 45.9 MB (45878967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00c059161524278c4c36c19bc9e15f881a76d35dfa7907d64e5368fa08cfabe`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 8.2 MB (8158629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e2cef807b62672343d701b6833953bd521a7ce41702624f45d2d796b0748e2`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 10.7 MB (10687679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aec6c2a63ff15795fd7235464c074e62a01aab27b66c75e51aca4b22d1ec07`  
		Last Modified: Wed, 01 Mar 2023 03:11:48 GMT  
		Size: 59.3 MB (59272951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47368484dc827d2541150d970d099cbc827331cba4014efcecf477781757c153`  
		Last Modified: Wed, 01 Mar 2023 03:12:21 GMT  
		Size: 174.9 MB (174926276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:844c8028a9815c68e30fdb0e3c1284cdd82ca2e3b6d6c93da5ddd5c6fc929502
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335903373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932509bb66171d164ed37159485c8587937293e2a8149266b757ba8858fe5483`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:21:20 GMT
ADD file:83e31d97e59fa435e4367903bc4de14c4bc67178b21cea27910cd23f23eb3a80 in / 
# Wed, 01 Mar 2023 02:21:20 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:52:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:53:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4362be0bd44228649833bb1416738fd1e9e110c9b44995dc7b36d6f6c712645f`  
		Last Modified: Wed, 01 Mar 2023 02:25:46 GMT  
		Size: 49.3 MB (49295339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2110847b2a04ab78caa763031ad2defabdaf9d626dbfcec71b215d35f0b70f09`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 8.9 MB (8900926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd381966a1347f9482594ca89251700a2fc3c4cfc23300a89d68207091e90084`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 11.4 MB (11371514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade03fa0cf349d2c4310e97b9776862ea961b32865410ca43789d56b255550f`  
		Last Modified: Wed, 01 Mar 2023 02:58:24 GMT  
		Size: 64.0 MB (64013118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dd468c1139187176cb306ea33f3fa3f4b68fed6a00e7d0835793454ce00e1b`  
		Last Modified: Wed, 01 Mar 2023 02:58:52 GMT  
		Size: 202.3 MB (202322476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:631c6b61580c0129c1a56f05b9a93618a0a1afdabbcf59f3a128367f86d855d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.2 MB (347248309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:046c7b891ef4ccee961ced21d3fe4461e8ea27d47b2529539f9c33b23fdbb62b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:40:05 GMT
ADD file:6282b025bbfdc732e0b90ff88ecdc7d48b84ec602874ef46e276d0250551f12e in / 
# Wed, 01 Mar 2023 01:40:06 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:14:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:15:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:417b7bc42b68fb696c2efa25377639c22c351f4705d5168da4f5695d53e4ba47`  
		Last Modified: Wed, 01 Mar 2023 01:46:43 GMT  
		Size: 50.3 MB (50314271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b68a1e6101c58260f889183e2e061e123bbc07a479a4ee59fff5649daa51d`  
		Last Modified: Wed, 01 Mar 2023 02:26:18 GMT  
		Size: 9.3 MB (9251109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63437f1cf3bc2a6cddc930ecd9a659ccfbcce779ac90a9c50efc7e8c1f56b42`  
		Last Modified: Wed, 01 Mar 2023 02:26:17 GMT  
		Size: 11.8 MB (11808756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd353cc8e971b20a47938912dda14d6fec9624aa9880053413a451cb3bc0f60`  
		Last Modified: Wed, 01 Mar 2023 02:26:41 GMT  
		Size: 66.0 MB (66012422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b99a677370160cefe862644ca09270260b636f9de7ee445839ef305d8857f6`  
		Last Modified: Wed, 01 Mar 2023 02:27:28 GMT  
		Size: 209.9 MB (209861751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a82507a1277c2124e09e887dfd7b4a31b0b1a1fc8bdec1f883b117f297e76d2c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.0 MB (324036580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d50a394cea62448159f423b39c3070b86d3314f1423d507654ecb0497d9c0d7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:46:00 GMT
ADD file:e14c7d6714484cc404ef7af2c7e0fcb17120cc8c1b631e9ac731a3be75da22b8 in / 
# Thu, 09 Feb 2023 02:46:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:48:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:55:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84e1d5547cbc284ab87d41eaa50711a7148e6080522c4ba245d27048c9d0fe70`  
		Last Modified: Thu, 09 Feb 2023 02:54:32 GMT  
		Size: 49.1 MB (49094289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16034fc732dcaff117d4120f724155ad39c461a2791c8bc488000dd93d88467c`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 8.4 MB (8414070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cc8b6e8bd467b0d1e27bfaf0bf0138f2e690aa8dd7eeddcc636d65c4b0ac34`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 11.2 MB (11153733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23789f2ae164d9a3f26a9a0663d938660993a4ba223713b5bde1aa34f68d35dc`  
		Last Modified: Thu, 09 Feb 2023 08:03:53 GMT  
		Size: 63.3 MB (63305330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd03ad3d3e89587274ed0844975c8ff2700fd1f95b056d7346b990bf970c894`  
		Last Modified: Thu, 09 Feb 2023 08:06:05 GMT  
		Size: 192.1 MB (192069158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:270e720c1a0ba1d7fadc6591991b8d7f9984f5aea254d2191222f1caae76c910
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.7 MB (358677337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a4b45352ad5e080d3923b7fec61af29c23f2d69f6a6616fd50b10fd0c9e8385`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:54 GMT
ADD file:2c1195fd765d1da7082bf383b9c5ef0b244e5398006d53897d5ea40e919399f1 in / 
# Wed, 01 Mar 2023 04:47:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:31:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:31:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:34:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6800c47237e7f7a1e5340856e56ba98e2b69a475b2458bb2416fdb0582d8c28`  
		Last Modified: Wed, 01 Mar 2023 04:54:24 GMT  
		Size: 53.3 MB (53273011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff0fff502cf707b8386c45c579606a759f85d3b49c007814826ad27212fdf5`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 9.7 MB (9652015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ef4d32b9b5d605909945396d9e13b86c238ff2ea6c800b63cef6d06dc2d6a3`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 12.2 MB (12168382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecf54311632074a960030227c6fca18a718af9b2631164c5c93529e814a5f50`  
		Last Modified: Wed, 01 Mar 2023 05:41:38 GMT  
		Size: 69.6 MB (69617831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48046f9759059f8abfcf3bf8b3ff28b67f3df1bd9cc3a2d31dcbee40947822d6`  
		Last Modified: Wed, 01 Mar 2023 05:42:40 GMT  
		Size: 214.0 MB (213966098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f36f7686751e847a8c69af8eba89a80c31e16ec89434ba40ebccec03984464e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.8 MB (313760190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a70710ffc9aeb0b1ef9ecfdbb6a892cec5ccdd05e291bf44c01c504fb8cfe`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:42 GMT
ADD file:a35d410eeff51ff3b7d9c823bc5ba421ef11373fb29ee93e8256efcbcdcee908 in / 
# Wed, 01 Mar 2023 02:50:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:16:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:16:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:17:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57e87143a56f85b3245b752ff94d616ef62e6372c0bcd9338b791267ea20f326`  
		Last Modified: Wed, 01 Mar 2023 02:55:04 GMT  
		Size: 47.6 MB (47629137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07cda735865838550e6455f8a76e842211afddfe8503e32aa744121e3435ae0`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 8.7 MB (8700269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c406447e84cbeb09410da5fd14cb6601c6f124b564b303a89c89e53406f68863`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 11.3 MB (11268803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b0879a47bff8d8b52a41d4dd0ceb2fa4313863026dfe04be33a743663128f8`  
		Last Modified: Wed, 01 Mar 2023 03:23:22 GMT  
		Size: 63.2 MB (63158949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a52b22ad7915c526a6a5a76890d098c9218f26db48004203de3a4630e03a54`  
		Last Modified: Wed, 01 Mar 2023 03:23:50 GMT  
		Size: 183.0 MB (183003032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:f6ef54d09fc53d24d449af6a6a8400f9d4056aab7a21396f3e85e3e9a973720e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:93738b56202c447b2ea0eef8020a8d4664e3712974058a408730f1218abb1830
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69730669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712e351b2bc9d7d841a9fcc1bb27278f12cb09bb4240cdc6338503b846bf87e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:57 GMT
ADD file:742621d60641957542e01d843bc130e616ba577a7135783b21e53d3a5d77ad5b in / 
# Wed, 01 Mar 2023 04:10:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:46:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:46:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d80cbe2ffd4f13cce276662ea5b4fa412791129d545137a4bea79fc41c446e0b`  
		Last Modified: Wed, 01 Mar 2023 04:15:57 GMT  
		Size: 49.3 MB (49261286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414a406365e2c651e77ea1d2dedd2c2fe7317552757dfc2701d2cdf6a578a51e`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 9.1 MB (9063535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515af3674ccc4fa7b84288322c2d1250d4de5952aafb54a33baeaf74fb694632`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 11.4 MB (11405848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b130af12e26d3c5dbafb04dcbcf75f0e751bb8327318a85a088aa317ab591e69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67673709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa3339472cc907f434562326764e3c0a37312ea0c737ab2fe67f577e10abf020`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:01 GMT
ADD file:4fadb88d3ead8d91349c79d7e903bbb8f6130b292bda6cb8099131210a815bc1 in / 
# Wed, 01 Mar 2023 01:49:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:21:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a03e1abdb2ebe924d64faf35eb6563891039999ec54a62f65419caf539ba6a88`  
		Last Modified: Wed, 01 Mar 2023 01:53:21 GMT  
		Size: 48.1 MB (48107781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d446d9cfc1201a906803d21a6e36423e22e9bebf24cf64bd16a4a3a73af61a2`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 8.5 MB (8514426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dc22595c5f06cd6d232ff8a3594b9aadef31095cb355dffad2b48a861717bf`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 11.1 MB (11051502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c9f72e9a500675032dd14939ac68f619ef7378e2ba5fa0bbe71d9f4e138b1413
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64725275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5849c538e7b742ecab1b90a01e25aac9dcef8e7de5b52969e2db8b217418209`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:39 GMT
ADD file:2cc322ac43103c8e367e39beaccf285da593ce4935ec4b1c90ae321a43b7123b in / 
# Wed, 01 Mar 2023 01:58:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:37:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4e5967747d4d88696bd5d5f37c0b5b8bcf8b29f3b448f6d1dd9623bdcc655965`  
		Last Modified: Wed, 01 Mar 2023 02:04:52 GMT  
		Size: 45.9 MB (45878967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00c059161524278c4c36c19bc9e15f881a76d35dfa7907d64e5368fa08cfabe`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 8.2 MB (8158629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e2cef807b62672343d701b6833953bd521a7ce41702624f45d2d796b0748e2`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 10.7 MB (10687679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4e04b288f31813639ec17e2ea31d111af553db8e47d7f70b166a0772f57544bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69567779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f267da9f91af76c93bff56ed319ac711d450951f634b99b0aff5950a94ccc3c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:21:20 GMT
ADD file:83e31d97e59fa435e4367903bc4de14c4bc67178b21cea27910cd23f23eb3a80 in / 
# Wed, 01 Mar 2023 02:21:20 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:52:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4362be0bd44228649833bb1416738fd1e9e110c9b44995dc7b36d6f6c712645f`  
		Last Modified: Wed, 01 Mar 2023 02:25:46 GMT  
		Size: 49.3 MB (49295339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2110847b2a04ab78caa763031ad2defabdaf9d626dbfcec71b215d35f0b70f09`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 8.9 MB (8900926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd381966a1347f9482594ca89251700a2fc3c4cfc23300a89d68207091e90084`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 11.4 MB (11371514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:75ed184206d2a35482c7d7f4648ce76a7ff1ca43e067a606c00b50aa756c8a2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71374136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b3d805c3fa51b65df72429839a1b714ea37b5e2d1916b81f60bd136aa385b9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:40:05 GMT
ADD file:6282b025bbfdc732e0b90ff88ecdc7d48b84ec602874ef46e276d0250551f12e in / 
# Wed, 01 Mar 2023 01:40:06 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:417b7bc42b68fb696c2efa25377639c22c351f4705d5168da4f5695d53e4ba47`  
		Last Modified: Wed, 01 Mar 2023 01:46:43 GMT  
		Size: 50.3 MB (50314271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b68a1e6101c58260f889183e2e061e123bbc07a479a4ee59fff5649daa51d`  
		Last Modified: Wed, 01 Mar 2023 02:26:18 GMT  
		Size: 9.3 MB (9251109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63437f1cf3bc2a6cddc930ecd9a659ccfbcce779ac90a9c50efc7e8c1f56b42`  
		Last Modified: Wed, 01 Mar 2023 02:26:17 GMT  
		Size: 11.8 MB (11808756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:31fbd48d97655e5743ae24d79f322184b28fe3e464b6ed9b4413ed1ffbea4648
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68662092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c4ec537af7ac1217076c5de461da3049f4b71d1e970249041e8a4abcdf3f1e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:46:00 GMT
ADD file:e14c7d6714484cc404ef7af2c7e0fcb17120cc8c1b631e9ac731a3be75da22b8 in / 
# Thu, 09 Feb 2023 02:46:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:48:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:84e1d5547cbc284ab87d41eaa50711a7148e6080522c4ba245d27048c9d0fe70`  
		Last Modified: Thu, 09 Feb 2023 02:54:32 GMT  
		Size: 49.1 MB (49094289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16034fc732dcaff117d4120f724155ad39c461a2791c8bc488000dd93d88467c`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 8.4 MB (8414070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cc8b6e8bd467b0d1e27bfaf0bf0138f2e690aa8dd7eeddcc636d65c4b0ac34`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 11.2 MB (11153733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f9a20d8078e12b97c3af8d9cdf1430e92499f23331fb4b029781ed5c46a2d4f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75093408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63aab7de5aecbad2363c5a0586046d3331cbdb0b8c3f89bf38833c6666ef81f4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:54 GMT
ADD file:2c1195fd765d1da7082bf383b9c5ef0b244e5398006d53897d5ea40e919399f1 in / 
# Wed, 01 Mar 2023 04:47:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:31:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b6800c47237e7f7a1e5340856e56ba98e2b69a475b2458bb2416fdb0582d8c28`  
		Last Modified: Wed, 01 Mar 2023 04:54:24 GMT  
		Size: 53.3 MB (53273011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff0fff502cf707b8386c45c579606a759f85d3b49c007814826ad27212fdf5`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 9.7 MB (9652015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ef4d32b9b5d605909945396d9e13b86c238ff2ea6c800b63cef6d06dc2d6a3`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 12.2 MB (12168382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7d8971371d1f0e05a21c043ffe902ef04946af99350b31cd8f69abcdf9c17aa1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67598209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c301055db6d45991d5c906e7e43bace2c2bbd2050ca71189ea3d370259f5b54`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:42 GMT
ADD file:a35d410eeff51ff3b7d9c823bc5ba421ef11373fb29ee93e8256efcbcdcee908 in / 
# Wed, 01 Mar 2023 02:50:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:16:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:57e87143a56f85b3245b752ff94d616ef62e6372c0bcd9338b791267ea20f326`  
		Last Modified: Wed, 01 Mar 2023 02:55:04 GMT  
		Size: 47.6 MB (47629137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07cda735865838550e6455f8a76e842211afddfe8503e32aa744121e3435ae0`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 8.7 MB (8700269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c406447e84cbeb09410da5fd14cb6601c6f124b564b303a89c89e53406f68863`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 11.3 MB (11268803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:a656a4057c545394d275f9a2401b1212207ae6b365880a71f1bdac8ce7acb84e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:61e869911246ffffe7006b0cf40b8e69c786397789246c1d7f0c362b4f77f0a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133887402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea16ba12d186d3aa3a15eccbe528665df5a6182d3e781f14d550e664cad9220`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:57 GMT
ADD file:742621d60641957542e01d843bc130e616ba577a7135783b21e53d3a5d77ad5b in / 
# Wed, 01 Mar 2023 04:10:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:46:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:46:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 04:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d80cbe2ffd4f13cce276662ea5b4fa412791129d545137a4bea79fc41c446e0b`  
		Last Modified: Wed, 01 Mar 2023 04:15:57 GMT  
		Size: 49.3 MB (49261286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414a406365e2c651e77ea1d2dedd2c2fe7317552757dfc2701d2cdf6a578a51e`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 9.1 MB (9063535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515af3674ccc4fa7b84288322c2d1250d4de5952aafb54a33baeaf74fb694632`  
		Last Modified: Wed, 01 Mar 2023 04:52:19 GMT  
		Size: 11.4 MB (11405848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4328fcba3826a509a956e5614c022c05ed89b4e718a69b607176d4a8f97f0e86`  
		Last Modified: Wed, 01 Mar 2023 04:52:36 GMT  
		Size: 64.2 MB (64156733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:769b660d04142b0b50dc374c44a0b6f21f9c173ee6da78112733f53722b345b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129237697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edd56cc8039bae242894637cb565ef5a4685943100e6e52d22630c1fe20fb1f8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:01 GMT
ADD file:4fadb88d3ead8d91349c79d7e903bbb8f6130b292bda6cb8099131210a815bc1 in / 
# Wed, 01 Mar 2023 01:49:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:21:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:21:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03e1abdb2ebe924d64faf35eb6563891039999ec54a62f65419caf539ba6a88`  
		Last Modified: Wed, 01 Mar 2023 01:53:21 GMT  
		Size: 48.1 MB (48107781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d446d9cfc1201a906803d21a6e36423e22e9bebf24cf64bd16a4a3a73af61a2`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 8.5 MB (8514426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dc22595c5f06cd6d232ff8a3594b9aadef31095cb355dffad2b48a861717bf`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 11.1 MB (11051502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0760e34b5fee30fa55ba71775caf6a3b2e755775ea03be4db0c03e5d83ff0a3`  
		Last Modified: Wed, 01 Mar 2023 02:26:32 GMT  
		Size: 61.6 MB (61563988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eec8b1e8acf1938703616b1dd5e636aafaf9a348da0a8b4f760abadf820d5f02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123998226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4711888af9d924bb6d81ff35c959c48dc8dd3764331e7e8f75c4be9208721f1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:39 GMT
ADD file:2cc322ac43103c8e367e39beaccf285da593ce4935ec4b1c90ae321a43b7123b in / 
# Wed, 01 Mar 2023 01:58:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:37:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:37:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e5967747d4d88696bd5d5f37c0b5b8bcf8b29f3b448f6d1dd9623bdcc655965`  
		Last Modified: Wed, 01 Mar 2023 02:04:52 GMT  
		Size: 45.9 MB (45878967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00c059161524278c4c36c19bc9e15f881a76d35dfa7907d64e5368fa08cfabe`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 8.2 MB (8158629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e2cef807b62672343d701b6833953bd521a7ce41702624f45d2d796b0748e2`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 10.7 MB (10687679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aec6c2a63ff15795fd7235464c074e62a01aab27b66c75e51aca4b22d1ec07`  
		Last Modified: Wed, 01 Mar 2023 03:11:48 GMT  
		Size: 59.3 MB (59272951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:79a54877762e7ec47749ccafef71d6e63006d42146126ffde09fa7cd30f3571b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133580897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:280a9022e0a86f89746caefe50eaaece1019298b65d05471d89f1afde4acd87e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:21:20 GMT
ADD file:83e31d97e59fa435e4367903bc4de14c4bc67178b21cea27910cd23f23eb3a80 in / 
# Wed, 01 Mar 2023 02:21:20 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:52:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4362be0bd44228649833bb1416738fd1e9e110c9b44995dc7b36d6f6c712645f`  
		Last Modified: Wed, 01 Mar 2023 02:25:46 GMT  
		Size: 49.3 MB (49295339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2110847b2a04ab78caa763031ad2defabdaf9d626dbfcec71b215d35f0b70f09`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 8.9 MB (8900926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd381966a1347f9482594ca89251700a2fc3c4cfc23300a89d68207091e90084`  
		Last Modified: Wed, 01 Mar 2023 02:58:08 GMT  
		Size: 11.4 MB (11371514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade03fa0cf349d2c4310e97b9776862ea961b32865410ca43789d56b255550f`  
		Last Modified: Wed, 01 Mar 2023 02:58:24 GMT  
		Size: 64.0 MB (64013118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6cde2155211d3f4d8d5db27af2fcc9954e9dbbe93b2e7a4208d6d145acb510de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137386558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed49974f31df5dbc1da3062aa51816dadfe02a8052b7def49df2b41c34fd9ff7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:40:05 GMT
ADD file:6282b025bbfdc732e0b90ff88ecdc7d48b84ec602874ef46e276d0250551f12e in / 
# Wed, 01 Mar 2023 01:40:06 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:14:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:417b7bc42b68fb696c2efa25377639c22c351f4705d5168da4f5695d53e4ba47`  
		Last Modified: Wed, 01 Mar 2023 01:46:43 GMT  
		Size: 50.3 MB (50314271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b68a1e6101c58260f889183e2e061e123bbc07a479a4ee59fff5649daa51d`  
		Last Modified: Wed, 01 Mar 2023 02:26:18 GMT  
		Size: 9.3 MB (9251109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63437f1cf3bc2a6cddc930ecd9a659ccfbcce779ac90a9c50efc7e8c1f56b42`  
		Last Modified: Wed, 01 Mar 2023 02:26:17 GMT  
		Size: 11.8 MB (11808756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd353cc8e971b20a47938912dda14d6fec9624aa9880053413a451cb3bc0f60`  
		Last Modified: Wed, 01 Mar 2023 02:26:41 GMT  
		Size: 66.0 MB (66012422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0abaabff52c976ed8f5fad72ca4d2637d4a6156591f7273dd926406bf5ab1b78
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131967422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9530e0dcd15bd60dd08d51b5a5cce11f7dd40d377205a10ef937708bfd716fce`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:46:00 GMT
ADD file:e14c7d6714484cc404ef7af2c7e0fcb17120cc8c1b631e9ac731a3be75da22b8 in / 
# Thu, 09 Feb 2023 02:46:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:48:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84e1d5547cbc284ab87d41eaa50711a7148e6080522c4ba245d27048c9d0fe70`  
		Last Modified: Thu, 09 Feb 2023 02:54:32 GMT  
		Size: 49.1 MB (49094289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16034fc732dcaff117d4120f724155ad39c461a2791c8bc488000dd93d88467c`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 8.4 MB (8414070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cc8b6e8bd467b0d1e27bfaf0bf0138f2e690aa8dd7eeddcc636d65c4b0ac34`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 11.2 MB (11153733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23789f2ae164d9a3f26a9a0663d938660993a4ba223713b5bde1aa34f68d35dc`  
		Last Modified: Thu, 09 Feb 2023 08:03:53 GMT  
		Size: 63.3 MB (63305330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0f7a8b3c9b4996e2ee9e65041bb5c8ea311482213b54d004d43cfa0da3bcf469
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144711239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a4114106d760615f32f4b575122bc6f8862f40d4c00e8535a1aa756c7b5014`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:54 GMT
ADD file:2c1195fd765d1da7082bf383b9c5ef0b244e5398006d53897d5ea40e919399f1 in / 
# Wed, 01 Mar 2023 04:47:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:31:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:31:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6800c47237e7f7a1e5340856e56ba98e2b69a475b2458bb2416fdb0582d8c28`  
		Last Modified: Wed, 01 Mar 2023 04:54:24 GMT  
		Size: 53.3 MB (53273011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff0fff502cf707b8386c45c579606a759f85d3b49c007814826ad27212fdf5`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 9.7 MB (9652015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ef4d32b9b5d605909945396d9e13b86c238ff2ea6c800b63cef6d06dc2d6a3`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 12.2 MB (12168382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecf54311632074a960030227c6fca18a718af9b2631164c5c93529e814a5f50`  
		Last Modified: Wed, 01 Mar 2023 05:41:38 GMT  
		Size: 69.6 MB (69617831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:384e64893747febf163fb0367883ec34308fc83212306707553bdb6011615410
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130757158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e16e9c63e3d82f943d4f4c6e591119c775a9709ea0848fa6fa822c3cf9f942`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:42 GMT
ADD file:a35d410eeff51ff3b7d9c823bc5ba421ef11373fb29ee93e8256efcbcdcee908 in / 
# Wed, 01 Mar 2023 02:50:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:16:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 03:16:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57e87143a56f85b3245b752ff94d616ef62e6372c0bcd9338b791267ea20f326`  
		Last Modified: Wed, 01 Mar 2023 02:55:04 GMT  
		Size: 47.6 MB (47629137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07cda735865838550e6455f8a76e842211afddfe8503e32aa744121e3435ae0`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 8.7 MB (8700269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c406447e84cbeb09410da5fd14cb6601c6f124b564b303a89c89e53406f68863`  
		Last Modified: Wed, 01 Mar 2023 03:23:06 GMT  
		Size: 11.3 MB (11268803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b0879a47bff8d8b52a41d4dd0ceb2fa4313863026dfe04be33a743663128f8`  
		Last Modified: Wed, 01 Mar 2023 03:23:22 GMT  
		Size: 63.2 MB (63158949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
