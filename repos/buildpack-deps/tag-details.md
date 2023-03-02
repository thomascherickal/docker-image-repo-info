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
$ docker pull buildpack-deps@sha256:03240023737a69d26df22a353956e98e4af4fe6d91d700e10fd1e325cb67c762
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
$ docker pull buildpack-deps@sha256:bc6401af10396327da867114d7fa9e07ecc1fb018a0615961855e71cabd808f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221420553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0dfd86882423e6676ece77a524ae6979a584ed3b331070f0fc4919c9c7d0d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:22:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:24:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f64811d5f9e93d0cbbbaa74de2730a6dffbc3772747117377b98c979a5524e2`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 6.6 MB (6617385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed2ab5e0f15f7f6389f01ef48d5599f61173bb6c946ae3b9ece6d809e2708e5`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f631ab33a755e153343352043423161c6232b94c3be5472cd780d6fb66fea8c`  
		Last Modified: Thu, 02 Mar 2023 03:42:24 GMT  
		Size: 45.5 MB (45513091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3693810db0c477f5e446bed1c9a3f9865d9639040e32bd4f1b2c250f64c80`  
		Last Modified: Thu, 02 Mar 2023 03:42:51 GMT  
		Size: 139.6 MB (139552796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:74c75dac160e6a6002151711537eefa6221e1a817509f02c3a6ebb8f0a1d2fe4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189574487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be6314f5a99b1f96f4d5a67b9be2dc68d22a8a0b30b9db139bce7ab1504cab6f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:29:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:30:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:31:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:34:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6903cded2b3516e50f5bfdefd273774820e65f03bae3d1539678d6109df4e0b`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 5.7 MB (5679883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d900ce5096b9d98c4eacd5931071e9cf5fcc5869f19310d1c2fff7d3ed6806c5`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 2.6 MB (2585896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672070d854b2efbf7e9d5720a994ded06c4e58c97060013aed2981fd327517c`  
		Last Modified: Thu, 02 Mar 2023 11:54:45 GMT  
		Size: 40.7 MB (40712962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b18ca116489a29fab0bb7155fcb39757b6e5fdb884a900b7c2d82cd03ab0a7c`  
		Last Modified: Thu, 02 Mar 2023 11:55:11 GMT  
		Size: 118.3 MB (118291676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c4cd38688fc0d2dc220ac8ff6ce7b091691936713d7be77487926e5205d67d4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (206007032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a4b2640ef9ab7a7e44c1a782ebb8e68971a25d26f2d300bead677825ec2bf2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:15:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527f5e352ac533cdac8c50ce47e4185b349d1de4d8799f7529bb5d2524e4cb47`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 6.1 MB (6056649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea801ed12cc0807ef6ee95dca6e04d01bd2d6359efc54635d38d8a0516f55784`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 2.8 MB (2789532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491410c5ebb78636109cdab447342140dc9a4facbc978baa236f142ea8e9d64c`  
		Last Modified: Thu, 02 Mar 2023 02:35:57 GMT  
		Size: 43.3 MB (43312084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a641b744032c31a727a19848af95648856083d9ee3b2ddf4e6131d3b8906acfb`  
		Last Modified: Thu, 02 Mar 2023 02:36:19 GMT  
		Size: 130.1 MB (130115229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; 386

```console
$ docker pull buildpack-deps@sha256:23c1ee63e808b3015de5980d721e4f9af625420fbcf9252ac708b3f26db8b8b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218708206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfda599ee4752c06f38d2471001e45a94a340d988b3650bd203fd5a1588c358`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:14:52 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:14:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:14:54 GMT
ADD file:765a9704b3961cee9523a98bfd0de0f97b6075431287fa7b8acd276145cb28c5 in / 
# Wed, 01 Mar 2023 03:14:54 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 14:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 14:26:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 14:27:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 14:31:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08886b8b414bd4d4f6a196c5ea7306887e23ed3e5d83e9bde2bfe0cc2af99325`  
		Last Modified: Thu, 02 Mar 2023 14:23:47 GMT  
		Size: 27.2 MB (27164837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16105d5c202ba8ceca010766befe9c0bae4ef06768c5649bbdebe34feeff56c0`  
		Last Modified: Thu, 02 Mar 2023 14:32:49 GMT  
		Size: 6.9 MB (6907843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606120c77dd0e4dc08e0829cd5fda3c301d68a11a8561df02368984d18c27e87`  
		Last Modified: Thu, 02 Mar 2023 14:32:48 GMT  
		Size: 3.3 MB (3255738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd34df470431bd99fe8348a0b7488317fd90179a50fc094b1bc09cfdfff0f651`  
		Last Modified: Thu, 02 Mar 2023 14:33:08 GMT  
		Size: 47.1 MB (47097279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cc969ea617066b06bd1d2af21a782f627a3f869a71f0cfa604137bade66456`  
		Last Modified: Thu, 02 Mar 2023 14:33:44 GMT  
		Size: 134.3 MB (134282509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:67fa38311170cdba88af20aa1b89395545f3efab0a3834c4664d8e8a340919d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246443180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44bd848f8d90d8dcb294a19721d764751f19869aa2cd2088193c7cbc90598830`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:15:24 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:15:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:15:27 GMT
ADD file:ca5a453351fddb6d7937e334f0331321829a5bebca3d726ef3dddad1f23b35c8 in / 
# Wed, 01 Mar 2023 03:15:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:12:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:12:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:18:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:27fbc2bd86045e72ba8d9901b237295e3094b37f456824337175e24a0f0afe98`  
		Last Modified: Thu, 02 Mar 2023 03:09:44 GMT  
		Size: 30.4 MB (30442026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fe4259cc8ab209d172cd6c47536773db4959cf18257a7d3d47b35257e3547`  
		Last Modified: Thu, 02 Mar 2023 03:54:32 GMT  
		Size: 7.0 MB (7036861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1d5bf7bb9bbef4a44b4363f1e0fa9ed98fe35bd78d986830c40d35c1641e5`  
		Last Modified: Thu, 02 Mar 2023 03:54:31 GMT  
		Size: 3.7 MB (3740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68956dba4cc03b50dc85a017a1231e5796aa790462edfefff2e29d810938fac5`  
		Last Modified: Thu, 02 Mar 2023 03:54:58 GMT  
		Size: 53.7 MB (53737565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4b2678c674974ef6a718cfeeb751759ca159ee0b9fcad54a313bc2df75c588`  
		Last Modified: Thu, 02 Mar 2023 03:55:45 GMT  
		Size: 151.5 MB (151486173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7b015c146106a9d5bed63ce8160f10f595371332c37d694c7735dba418cd8154
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205761889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36218dc4a0ffa429ceecdc8268fc8a5f31517d1706b5e6a208e4f08a4b2f1d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:09 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:11 GMT
ADD file:49b5368b8703fe0aa128fe923b83da7ab2a30a7a1c0395682c905b9271e7f503 in / 
# Wed, 01 Mar 2023 03:18:11 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:02:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:03:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:03:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:05:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:306d1b363f89f239f5dc6314e0033094c067617b584ce004fd8db99402dab321`  
		Last Modified: Thu, 02 Mar 2023 02:21:31 GMT  
		Size: 25.4 MB (25371412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb206f9ee26b21514bd7026ed97956b03f4175d0d2096d5f87471b82c21903e8`  
		Last Modified: Thu, 02 Mar 2023 02:21:28 GMT  
		Size: 6.3 MB (6310489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732358426922e371a7b325dcc12fdff47050775aafd32bcf8884ed1ad12f120`  
		Last Modified: Thu, 02 Mar 2023 02:21:27 GMT  
		Size: 3.0 MB (2976715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f95174d0c3f8fa7400f2fe1baa0a15756c66695199991cb0126f6cd6586899`  
		Last Modified: Thu, 02 Mar 2023 02:21:45 GMT  
		Size: 45.0 MB (45039451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d6cdbea8d41a3597e61ccc469c9ed2051271cff3c92e5e98d2519cf49acb69`  
		Last Modified: Thu, 02 Mar 2023 02:22:09 GMT  
		Size: 126.1 MB (126063822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-curl`

```console
$ docker pull buildpack-deps@sha256:73601edcb84c68e3c11b715ffee8e797dd05f0b388a2168c2301c4d90c3fc90d
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
$ docker pull buildpack-deps@sha256:99f85c256072d05e9bb8e3656852ae30bddc97653de13c5eb17cdc8b6dafd6f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36354666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111158ec462cd995c4c3e243b17f67d14fb75461904858179cf76df85ab57959`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f64811d5f9e93d0cbbbaa74de2730a6dffbc3772747117377b98c979a5524e2`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 6.6 MB (6617385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed2ab5e0f15f7f6389f01ef48d5599f61173bb6c946ae3b9ece6d809e2708e5`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9927f426d766fa71f28ffb9fdc683468b8289aa35a0ca6a188fe99b89131c37e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30569849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c454cb60b9b4cb6c88a731a1efe79dd872854170ce9ef7e0a743c199f56c2a5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:29:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:30:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6903cded2b3516e50f5bfdefd273774820e65f03bae3d1539678d6109df4e0b`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 5.7 MB (5679883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d900ce5096b9d98c4eacd5931071e9cf5fcc5869f19310d1c2fff7d3ed6806c5`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 2.6 MB (2585896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f7da0ac25d1397e53a187cd55f39a39a896c2cf7cc959c9cd02267a0f44e7d8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32579719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dda8439f80b101956498824b42467ff97d1b014933c44c7453c440a794eb6b48`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527f5e352ac533cdac8c50ce47e4185b349d1de4d8799f7529bb5d2524e4cb47`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 6.1 MB (6056649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea801ed12cc0807ef6ee95dca6e04d01bd2d6359efc54635d38d8a0516f55784`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 2.8 MB (2789532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e2b59c4e7bae90368ddf432e1950431ad277793049e5c6a436864b0e52ac95ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37328418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aab4d33e0dc6612a7eedbdd04c8e78eb35854e44466e8d83e7697737af98f25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:14:52 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:14:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:14:54 GMT
ADD file:765a9704b3961cee9523a98bfd0de0f97b6075431287fa7b8acd276145cb28c5 in / 
# Wed, 01 Mar 2023 03:14:54 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 14:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 14:26:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:08886b8b414bd4d4f6a196c5ea7306887e23ed3e5d83e9bde2bfe0cc2af99325`  
		Last Modified: Thu, 02 Mar 2023 14:23:47 GMT  
		Size: 27.2 MB (27164837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16105d5c202ba8ceca010766befe9c0bae4ef06768c5649bbdebe34feeff56c0`  
		Last Modified: Thu, 02 Mar 2023 14:32:49 GMT  
		Size: 6.9 MB (6907843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606120c77dd0e4dc08e0829cd5fda3c301d68a11a8561df02368984d18c27e87`  
		Last Modified: Thu, 02 Mar 2023 14:32:48 GMT  
		Size: 3.3 MB (3255738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b3626e1fc0df781ffdcd5858ddfd7e32cfd9a727dd64393d293bfa412fb7ed3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41219442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:969499ba388db8062c83aa23fbf2d2e1c8380f9bb88195a6da9832b5a5e02a73`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:15:24 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:15:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:15:27 GMT
ADD file:ca5a453351fddb6d7937e334f0331321829a5bebca3d726ef3dddad1f23b35c8 in / 
# Wed, 01 Mar 2023 03:15:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:12:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:12:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:27fbc2bd86045e72ba8d9901b237295e3094b37f456824337175e24a0f0afe98`  
		Last Modified: Thu, 02 Mar 2023 03:09:44 GMT  
		Size: 30.4 MB (30442026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fe4259cc8ab209d172cd6c47536773db4959cf18257a7d3d47b35257e3547`  
		Last Modified: Thu, 02 Mar 2023 03:54:32 GMT  
		Size: 7.0 MB (7036861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1d5bf7bb9bbef4a44b4363f1e0fa9ed98fe35bd78d986830c40d35c1641e5`  
		Last Modified: Thu, 02 Mar 2023 03:54:31 GMT  
		Size: 3.7 MB (3740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:774b1f4c6014651f88a0b380963c333bd8be99ad1c574dd6b97fe702508e3fef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34658616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d4a9dc5198a5458700a926e8863d1585e7baf6439d74278b821316e46bec3e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:09 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:11 GMT
ADD file:49b5368b8703fe0aa128fe923b83da7ab2a30a7a1c0395682c905b9271e7f503 in / 
# Wed, 01 Mar 2023 03:18:11 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:02:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:03:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:306d1b363f89f239f5dc6314e0033094c067617b584ce004fd8db99402dab321`  
		Last Modified: Thu, 02 Mar 2023 02:21:31 GMT  
		Size: 25.4 MB (25371412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb206f9ee26b21514bd7026ed97956b03f4175d0d2096d5f87471b82c21903e8`  
		Last Modified: Thu, 02 Mar 2023 02:21:28 GMT  
		Size: 6.3 MB (6310489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732358426922e371a7b325dcc12fdff47050775aafd32bcf8884ed1ad12f120`  
		Last Modified: Thu, 02 Mar 2023 02:21:27 GMT  
		Size: 3.0 MB (2976715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-scm`

```console
$ docker pull buildpack-deps@sha256:bdbeb92cdb417dfefa084dc354ebb292bc3d80354b576d57918b117d81af1984
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
$ docker pull buildpack-deps@sha256:bc9e9bbd14e8a837e30009807718c317555b3585704c270ca0544ef30f322d48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81867757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd2ec34b02293026aee8b871a2ae86c29c797aa05892297f3a307185c275e28c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:22:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f64811d5f9e93d0cbbbaa74de2730a6dffbc3772747117377b98c979a5524e2`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 6.6 MB (6617385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed2ab5e0f15f7f6389f01ef48d5599f61173bb6c946ae3b9ece6d809e2708e5`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f631ab33a755e153343352043423161c6232b94c3be5472cd780d6fb66fea8c`  
		Last Modified: Thu, 02 Mar 2023 03:42:24 GMT  
		Size: 45.5 MB (45513091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c945aafe1fad15d38e1188cc1844f06e144bab7335c3db05f2caa56f3ca460ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71282811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34ca2769a55b83b9eb31be2f63bed94363f1630e19ee1d39e592aad1851a18bc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:29:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:30:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:31:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6903cded2b3516e50f5bfdefd273774820e65f03bae3d1539678d6109df4e0b`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 5.7 MB (5679883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d900ce5096b9d98c4eacd5931071e9cf5fcc5869f19310d1c2fff7d3ed6806c5`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 2.6 MB (2585896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672070d854b2efbf7e9d5720a994ded06c4e58c97060013aed2981fd327517c`  
		Last Modified: Thu, 02 Mar 2023 11:54:45 GMT  
		Size: 40.7 MB (40712962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:dc66d659df3c4d980bfd741e281c52d81cfab1027cdb9d0449f4d054806fdf77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75891803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4349a1a66435e325994ec9e6ec99ad5776cd7ea349f06b3e79c091f197bda134`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527f5e352ac533cdac8c50ce47e4185b349d1de4d8799f7529bb5d2524e4cb47`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 6.1 MB (6056649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea801ed12cc0807ef6ee95dca6e04d01bd2d6359efc54635d38d8a0516f55784`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 2.8 MB (2789532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491410c5ebb78636109cdab447342140dc9a4facbc978baa236f142ea8e9d64c`  
		Last Modified: Thu, 02 Mar 2023 02:35:57 GMT  
		Size: 43.3 MB (43312084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f8c35b10a7e33961c8ce0a4bb0387e1bb73fa5a4677e5d36f56be2dfd6ea1b7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84425697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc4a367ff17e24b264b6562eee2668fcff45fcd418f80cd1e43989d1f259f5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:14:52 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:14:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:14:54 GMT
ADD file:765a9704b3961cee9523a98bfd0de0f97b6075431287fa7b8acd276145cb28c5 in / 
# Wed, 01 Mar 2023 03:14:54 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 14:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 14:26:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 14:27:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08886b8b414bd4d4f6a196c5ea7306887e23ed3e5d83e9bde2bfe0cc2af99325`  
		Last Modified: Thu, 02 Mar 2023 14:23:47 GMT  
		Size: 27.2 MB (27164837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16105d5c202ba8ceca010766befe9c0bae4ef06768c5649bbdebe34feeff56c0`  
		Last Modified: Thu, 02 Mar 2023 14:32:49 GMT  
		Size: 6.9 MB (6907843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606120c77dd0e4dc08e0829cd5fda3c301d68a11a8561df02368984d18c27e87`  
		Last Modified: Thu, 02 Mar 2023 14:32:48 GMT  
		Size: 3.3 MB (3255738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd34df470431bd99fe8348a0b7488317fd90179a50fc094b1bc09cfdfff0f651`  
		Last Modified: Thu, 02 Mar 2023 14:33:08 GMT  
		Size: 47.1 MB (47097279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:61f125647b51960eaaa1628df14c40ad5596f9a0c8ca31b75db9663c5ff8007f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94957007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ae7f36d16db90652afad8c37a9ea6b419e7b1ad7a94291093ec62e326ab0e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:15:24 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:15:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:15:27 GMT
ADD file:ca5a453351fddb6d7937e334f0331321829a5bebca3d726ef3dddad1f23b35c8 in / 
# Wed, 01 Mar 2023 03:15:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:12:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:12:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:27fbc2bd86045e72ba8d9901b237295e3094b37f456824337175e24a0f0afe98`  
		Last Modified: Thu, 02 Mar 2023 03:09:44 GMT  
		Size: 30.4 MB (30442026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fe4259cc8ab209d172cd6c47536773db4959cf18257a7d3d47b35257e3547`  
		Last Modified: Thu, 02 Mar 2023 03:54:32 GMT  
		Size: 7.0 MB (7036861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1d5bf7bb9bbef4a44b4363f1e0fa9ed98fe35bd78d986830c40d35c1641e5`  
		Last Modified: Thu, 02 Mar 2023 03:54:31 GMT  
		Size: 3.7 MB (3740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68956dba4cc03b50dc85a017a1231e5796aa790462edfefff2e29d810938fac5`  
		Last Modified: Thu, 02 Mar 2023 03:54:58 GMT  
		Size: 53.7 MB (53737565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:54ddd0cd0622a5cd6cf1b28c3cb01a126d011f4d8e4c29ce1903761bfc7da58d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79698067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:206911be72a3fb03d2417b774c512074beef855e16b0cd2235cf6e178d1a1736`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:09 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:11 GMT
ADD file:49b5368b8703fe0aa128fe923b83da7ab2a30a7a1c0395682c905b9271e7f503 in / 
# Wed, 01 Mar 2023 03:18:11 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:02:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:03:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:03:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:306d1b363f89f239f5dc6314e0033094c067617b584ce004fd8db99402dab321`  
		Last Modified: Thu, 02 Mar 2023 02:21:31 GMT  
		Size: 25.4 MB (25371412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb206f9ee26b21514bd7026ed97956b03f4175d0d2096d5f87471b82c21903e8`  
		Last Modified: Thu, 02 Mar 2023 02:21:28 GMT  
		Size: 6.3 MB (6310489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732358426922e371a7b325dcc12fdff47050775aafd32bcf8884ed1ad12f120`  
		Last Modified: Thu, 02 Mar 2023 02:21:27 GMT  
		Size: 3.0 MB (2976715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f95174d0c3f8fa7400f2fe1baa0a15756c66695199991cb0126f6cd6586899`  
		Last Modified: Thu, 02 Mar 2023 02:21:45 GMT  
		Size: 45.0 MB (45039451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04`

```console
$ docker pull buildpack-deps@sha256:a935aae0569e82652a65d88ac7a1996d83bad092a346da4999eb73d34cb0f23d
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
$ docker pull buildpack-deps@sha256:595b2e444543064db2180320b4a521621630b3086acc881d4e1a7a5c6bfede96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245779275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee045173ae74b7b44140d6bc57447da87c62d5054c11aa5a88d9f2a06155c09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:25:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:25:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b7d3f3b016944c7eeeee37880c5c274cfc06cccd337b282c382d036852f921`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 7.7 MB (7739318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7712ac161458ffa37dfe485734ac5bfbc45c78512bfc1bca4479eb5b6f2aa64e`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 3.6 MB (3627267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf762b78d7137d4905242d9e25291e630f6926d0bd5cada5e7072817f61748`  
		Last Modified: Thu, 02 Mar 2023 03:43:20 GMT  
		Size: 60.7 MB (60740440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc356f49ea441894a0ae1bc758258a040d5375f2bd1e7ff2185f00e77198185`  
		Last Modified: Thu, 02 Mar 2023 03:43:48 GMT  
		Size: 145.1 MB (145094248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6d158f6d184a97d1dfef9b4edb82d7dd489d520b9252589ef7c13283a79361bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211781714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3a5fd39b47359ac607eded26d7b0108b92f150304a4e5dbaceaa5f4285a3b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:34:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:35:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:38:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cdafdb2f80a4c0460861f9220f045255f35eca62f6c065d24d65d3950a8c93`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 6.7 MB (6726138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eec04ad18d2253a95f5fcfcdd36aa4f470211a830af52b3e5856b8a8fd0ca7`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 3.1 MB (3104511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b743206528cfc301cf72ca17581201c8ca2e513bfa66b8795a8c9f58530f979`  
		Last Modified: Thu, 02 Mar 2023 11:55:43 GMT  
		Size: 55.4 MB (55433524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9d1daa72ce9f63ee0d3b940a6b63549facf2bbdf6c0fb8315a6105e99c36f3`  
		Last Modified: Thu, 02 Mar 2023 11:56:10 GMT  
		Size: 121.9 MB (121931093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:07f23c18b827305b81c5f727176b832ce798bd5da415fc7d073faf506b3ed0a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (236000423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408e406aadc361d174f2857e983a863b7ab799b75aa0fcb77e9c346923a498a0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:15:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:17:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:20:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eb13d431eb1ef5f774a4d14dafd7895d0061c2b77e3d613eed550a0245407e`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 7.6 MB (7601140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffe806a7e8e21e8288df2fed964181acc22875517099563c835fab72df366a5`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 3.6 MB (3616335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b02b41f50d1324e472bd6f2983f88f54704cdbd4af160efbc6e42e9a30c202`  
		Last Modified: Thu, 02 Mar 2023 02:36:46 GMT  
		Size: 60.8 MB (60817897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751575f78c3732573ab9aece852eadcb0d9a48e7b0eced95b9d7890ccc8c29d`  
		Last Modified: Thu, 02 Mar 2023 02:37:09 GMT  
		Size: 136.8 MB (136770530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1b5295e484925905b7e3b18f0e115ecfba46ec1673f7d2cc02016c9537015642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269626587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f809b1eaa3bb5cdb30f6a1553650cc08b4fe3dd4f58aa9ed33d923da8f63a4ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:25:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:25:25 GMT
ADD file:8ec53343ee3a54689d663a250c785fbf7b8ac0c74de561582d2e54878e2d73b5 in / 
# Wed, 01 Mar 2023 05:25:25 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:27:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ecbbabc4a8d11d32aa94bd1d645cba73ad91f59060b872eaf684de51310281b`  
		Last Modified: Thu, 02 Mar 2023 03:56:04 GMT  
		Size: 33.3 MB (33300379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ae83340e2c9ec8730a49a2c9aea2b21377b8a13b0c84c4b76cda0b29f82b4`  
		Last Modified: Thu, 02 Mar 2023 03:55:58 GMT  
		Size: 8.7 MB (8692716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b6ac479d5a474eedb2bd6b11d64e8b631ccce4beb6e06c84f00b6a2401fe5`  
		Last Modified: Thu, 02 Mar 2023 03:55:56 GMT  
		Size: 4.5 MB (4486858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7463e49960ae08f87f90376abcd19653c97a0752f8ccec05d042697e537f29f7`  
		Last Modified: Thu, 02 Mar 2023 03:56:33 GMT  
		Size: 69.6 MB (69553064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8eb87abfba2b370ecf10fd2cad3a672ca67bb51c2986a4b91ba814d27ada36`  
		Last Modified: Thu, 02 Mar 2023 03:57:23 GMT  
		Size: 153.6 MB (153593570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4c565e2587257fbb8d803086ed497597cb90115d36588b7a1a7428fa1ae02143
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226385332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e7e156764c073cc753dc89b15d097126091bb9ed5040bbadb7c371bd2f8a8cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:17 GMT
ADD file:859bfd657725af24f17d4e3c5b3b583b4b29d55f5f7f2f44fbdd6fbc83c6952d in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:06:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:06:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:07:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:09:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6ac74ab42247b9491b6986614b9868ce755dc1c84611543400690873aa73416`  
		Last Modified: Thu, 02 Mar 2023 02:22:20 GMT  
		Size: 27.0 MB (27016384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc17b063ad8d756ac72af0baf660b2a167389eae787139cf93b4069d0c6b99e6`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 7.4 MB (7379145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed830f413f3cae573689a1c936a49883bbb291424264e382dcc1da4590763d7`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 3.5 MB (3542220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb456cc7a06a826274d0489333373e503b4847ae4f5e22a50abf74ea87444a`  
		Last Modified: Thu, 02 Mar 2023 02:22:37 GMT  
		Size: 60.0 MB (60020217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31af2011810d962a8ab70a00f570ad12418f8a477135869fb1a0776eb1a149ac`  
		Last Modified: Thu, 02 Mar 2023 02:23:01 GMT  
		Size: 128.4 MB (128427366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:984dc5c11cde1a5d03a678d8aac00aca49775dca4ea7d9944789e27d289c64cf
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
$ docker pull buildpack-deps@sha256:c4824dc0e30a785dd034a6ba5ded770e6f50c8bd8d9075e44a4bd853b3877215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39944587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5caab55bf6d1a9670b35b8708c155221d41b0494671f44dce30a46726e341d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:25:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:25:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b7d3f3b016944c7eeeee37880c5c274cfc06cccd337b282c382d036852f921`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 7.7 MB (7739318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7712ac161458ffa37dfe485734ac5bfbc45c78512bfc1bca4479eb5b6f2aa64e`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 3.6 MB (3627267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c87787b92e2117d7b7a33eb5dabe78904f745298e10d43755236acd5b8914118
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34417097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4ec684782764d6ba26a275ce1f732fac70f18b5de92501502f1b2a42e279f82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:34:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cdafdb2f80a4c0460861f9220f045255f35eca62f6c065d24d65d3950a8c93`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 6.7 MB (6726138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eec04ad18d2253a95f5fcfcdd36aa4f470211a830af52b3e5856b8a8fd0ca7`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 3.1 MB (3104511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c595692763bde705e8e32ea772ba5e033189fc44826e95715cdf8f8a3cb7d5bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38411996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1be97e4a549deb271895519fd7cfebdbff011498ae4679449cea44653528df5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:15:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eb13d431eb1ef5f774a4d14dafd7895d0061c2b77e3d613eed550a0245407e`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 7.6 MB (7601140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffe806a7e8e21e8288df2fed964181acc22875517099563c835fab72df366a5`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 3.6 MB (3616335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4ababf7fb20ae1801b2a6e85ceb554ad08e24c87cc993d0ba8fba7c9182f3219
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46479953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e64276e03515e980c104a27b52c96227de1789f094240a143f53258907492dd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:25:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:25:25 GMT
ADD file:8ec53343ee3a54689d663a250c785fbf7b8ac0c74de561582d2e54878e2d73b5 in / 
# Wed, 01 Mar 2023 05:25:25 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4ecbbabc4a8d11d32aa94bd1d645cba73ad91f59060b872eaf684de51310281b`  
		Last Modified: Thu, 02 Mar 2023 03:56:04 GMT  
		Size: 33.3 MB (33300379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ae83340e2c9ec8730a49a2c9aea2b21377b8a13b0c84c4b76cda0b29f82b4`  
		Last Modified: Thu, 02 Mar 2023 03:55:58 GMT  
		Size: 8.7 MB (8692716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b6ac479d5a474eedb2bd6b11d64e8b631ccce4beb6e06c84f00b6a2401fe5`  
		Last Modified: Thu, 02 Mar 2023 03:55:56 GMT  
		Size: 4.5 MB (4486858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0343330c438e6f2403980ca7d2e3b3561187c0cd05366b52540e2544be7d7a0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37937749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a223df0c64acbbf14d7148eac1e5a3566119146af7d66bcb1bcc702412b9abc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:17 GMT
ADD file:859bfd657725af24f17d4e3c5b3b583b4b29d55f5f7f2f44fbdd6fbc83c6952d in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:06:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:06:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d6ac74ab42247b9491b6986614b9868ce755dc1c84611543400690873aa73416`  
		Last Modified: Thu, 02 Mar 2023 02:22:20 GMT  
		Size: 27.0 MB (27016384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc17b063ad8d756ac72af0baf660b2a167389eae787139cf93b4069d0c6b99e6`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 7.4 MB (7379145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed830f413f3cae573689a1c936a49883bbb291424264e382dcc1da4590763d7`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 3.5 MB (3542220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:79af9774ce5575c78d3cb87f01db10be2d14c83c432d98d38cd9c46d089bcd00
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
$ docker pull buildpack-deps@sha256:35d4677d74ee38e81499ccfe32c1d9234fc0c0ade83ea095f3c36d9830c4ed18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100685027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cbe0a30857b0e0810b34b6fc2a6137c37e3261e8101890646c44da76ec86db6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:25:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:25:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b7d3f3b016944c7eeeee37880c5c274cfc06cccd337b282c382d036852f921`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 7.7 MB (7739318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7712ac161458ffa37dfe485734ac5bfbc45c78512bfc1bca4479eb5b6f2aa64e`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 3.6 MB (3627267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf762b78d7137d4905242d9e25291e630f6926d0bd5cada5e7072817f61748`  
		Last Modified: Thu, 02 Mar 2023 03:43:20 GMT  
		Size: 60.7 MB (60740440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:38ef378fe4ad8b7f3d9489034e7f61b5347c531c2b986b4d889b4608ed124cde
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89850621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417c12900a3dd87706ff12eb9e4370b09bc22988769f3df9028cfb36346b496c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:34:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:35:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cdafdb2f80a4c0460861f9220f045255f35eca62f6c065d24d65d3950a8c93`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 6.7 MB (6726138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eec04ad18d2253a95f5fcfcdd36aa4f470211a830af52b3e5856b8a8fd0ca7`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 3.1 MB (3104511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b743206528cfc301cf72ca17581201c8ca2e513bfa66b8795a8c9f58530f979`  
		Last Modified: Thu, 02 Mar 2023 11:55:43 GMT  
		Size: 55.4 MB (55433524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2d9ba385e19d2fe67be14f111c916e1b28326e57d73b9ce143a20a1716f4fc24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99229893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e480fce56055355bcd1dbcd9b0383ab3052ed0a7f921bd2eee5f16ad138b8f71`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:15:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:17:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eb13d431eb1ef5f774a4d14dafd7895d0061c2b77e3d613eed550a0245407e`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 7.6 MB (7601140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffe806a7e8e21e8288df2fed964181acc22875517099563c835fab72df366a5`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 3.6 MB (3616335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b02b41f50d1324e472bd6f2983f88f54704cdbd4af160efbc6e42e9a30c202`  
		Last Modified: Thu, 02 Mar 2023 02:36:46 GMT  
		Size: 60.8 MB (60817897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:097e0ff2bf42901bcb9a769ba497f752b671df6f9f096e69d646c0e1fed9169d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116033017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e8553668a9ab292bc90a0129e3925d4dc4a30a334691b732744e17a6456965d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:25:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:25:25 GMT
ADD file:8ec53343ee3a54689d663a250c785fbf7b8ac0c74de561582d2e54878e2d73b5 in / 
# Wed, 01 Mar 2023 05:25:25 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ecbbabc4a8d11d32aa94bd1d645cba73ad91f59060b872eaf684de51310281b`  
		Last Modified: Thu, 02 Mar 2023 03:56:04 GMT  
		Size: 33.3 MB (33300379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ae83340e2c9ec8730a49a2c9aea2b21377b8a13b0c84c4b76cda0b29f82b4`  
		Last Modified: Thu, 02 Mar 2023 03:55:58 GMT  
		Size: 8.7 MB (8692716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b6ac479d5a474eedb2bd6b11d64e8b631ccce4beb6e06c84f00b6a2401fe5`  
		Last Modified: Thu, 02 Mar 2023 03:55:56 GMT  
		Size: 4.5 MB (4486858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7463e49960ae08f87f90376abcd19653c97a0752f8ccec05d042697e537f29f7`  
		Last Modified: Thu, 02 Mar 2023 03:56:33 GMT  
		Size: 69.6 MB (69553064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:38bd61dec26f3d8c377aa42023d084418de54f0f11ddf9eddeaa945b46b2f5bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (97957966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be039469f9caf4b3cf6f0c5c7d8b6e28cf93f6dde713bd55edc8b23513950c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:17 GMT
ADD file:859bfd657725af24f17d4e3c5b3b583b4b29d55f5f7f2f44fbdd6fbc83c6952d in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:06:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:06:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:07:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6ac74ab42247b9491b6986614b9868ce755dc1c84611543400690873aa73416`  
		Last Modified: Thu, 02 Mar 2023 02:22:20 GMT  
		Size: 27.0 MB (27016384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc17b063ad8d756ac72af0baf660b2a167389eae787139cf93b4069d0c6b99e6`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 7.4 MB (7379145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed830f413f3cae573689a1c936a49883bbb291424264e382dcc1da4590763d7`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 3.5 MB (3542220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb456cc7a06a826274d0489333373e503b4847ae4f5e22a50abf74ea87444a`  
		Last Modified: Thu, 02 Mar 2023 02:22:37 GMT  
		Size: 60.0 MB (60020217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04`

```console
$ docker pull buildpack-deps@sha256:9a5858bbf22b934014c6d0cacb9e2e8281868a5315445da65574541a919dba32
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
$ docker pull buildpack-deps@sha256:c6097317ab952d1afb8c1199bdf70c7d1bcacdc64a3319ca0228eef74c9532c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (250025364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d5252a78e69dbf7e7b1785eb3482824865a2d45e2be1a51928e796fa19efc58`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:33:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b17938a1a752564000a3a0aeed04eafc6958f178a7fcc09094daa31ec80767`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.8 MB (3788644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51ade0caaff8e59d92682e80d534ad83b8bc2d760bbe60eb56dc0363c60b4d6`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.6 MB (3561585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b8264f0fdf1f57cc3ac8b5b09faac810a388350812478b3dc2ab19727db68`  
		Last Modified: Thu, 02 Mar 2023 03:44:15 GMT  
		Size: 39.4 MB (39353140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985addd9038004b289a1cd2d449d95f1a7d1292f38b3ba6a8627732be72d20db`  
		Last Modified: Thu, 02 Mar 2023 03:44:45 GMT  
		Size: 172.9 MB (172891993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c315b1fd3deb39e15675ded20c0eff07feefa72c495f2c400ce5da57a7b3b5ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216668610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08db3cf9b75c32f87a7066a58928c9b1d8312e8d1807a3ded7a02ec539aab5af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:45:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:45:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:45:58 GMT
ADD file:d8e0c2340f91ec5973c8459c1a917be69f6530fe7f88da02eb5b4dd562c31730 in / 
# Wed, 01 Mar 2023 04:45:59 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:38:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:38:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:39:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:42:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5909c79a6169dfa05f978dbe7f8dfeadbb92a0d4a3a4d792314b3afe271dd793`  
		Last Modified: Wed, 01 Mar 2023 08:59:31 GMT  
		Size: 27.0 MB (27024489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e834b31ec46c994de883b1d8fd540229984065b7116dc8dab706aa6969bd5bff`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.5 MB (3539420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2617d031bbc0245044288b2afe503e376a8d9b8ded256246d64c969d12c85e7c`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.7 MB (3713780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffb58fb6ee1096d3a9785f5fd877bff68fdae04f23374b1f8753549f2dfa0e8`  
		Last Modified: Thu, 02 Mar 2023 11:56:38 GMT  
		Size: 41.9 MB (41907681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7871bf146ef1fecfbd6d2edf4122cf98e93d0007dc7f6c20f0dc4e032cbb6c`  
		Last Modified: Thu, 02 Mar 2023 11:57:06 GMT  
		Size: 140.5 MB (140483240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8c0e084a35a14526bcdbd462f399caa72f94e93c1e45d2dd6826c6c30b6686f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241331257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d42d4ee258d3bbea3b7c73ea09047bd5770942302d55947c411142e80fa2b03`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:21:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:22:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:25:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ecb6dff9238e75e6877b0624e8c0054bcb5d51c97f5f178a8a699de3e06572`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.8 MB (3760955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb16d0d18eaee62625a39492bf99dabbc71b2e3d6278c10a2080894ebe562b`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.5 MB (3536614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088d8f170fef46d01bbb6cd7b616c91b38f4fcad2ab1b42e1d93e9d86a7febe9`  
		Last Modified: Thu, 02 Mar 2023 02:37:34 GMT  
		Size: 39.2 MB (39242827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3373b535e41981b6538ebc53657679e880b4981c2c0626a29e4b14fb40459ae`  
		Last Modified: Thu, 02 Mar 2023 02:38:00 GMT  
		Size: 166.4 MB (166402939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:45e74d13a22728db4b4ec36070d857f369a226970a67390997b958f21ea1f6ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271848633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4ed251594f077f2874d4b7f9391ab978d7cbcf5a0d69ab768031bec032b3c1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:09:57 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:09:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:01 GMT
ADD file:e4d45fbda8cf3ca1613a11d2b929670e0e12b43c66818636afa9ebcbf6b48b59 in / 
# Wed, 01 Mar 2023 05:10:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:28:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:36:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:062a5dd6f1a8faa2ffa6ca3db2cdb7e930e5f49f52c8647b30709399b759b1cb`  
		Last Modified: Thu, 02 Mar 2023 03:35:30 GMT  
		Size: 35.7 MB (35711589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387fa66f2465a45a4bf52efe7a70d02b4b563ea79f4a05b59a132253b6fd192c`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.3 MB (4262192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3313c961eddc996b17782dfb540ee65ee6801254d9ee09d82691b5a9f66f7431`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.2 MB (4234903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ba7916137f91162c1002b749a8a79118a1565f3a770f8d4d9415bd64e78b8b`  
		Last Modified: Thu, 02 Mar 2023 03:58:05 GMT  
		Size: 43.8 MB (43768446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbee4b59613644150cb1c5f30f7909c912cae5d9a2bbfd41fc3e4fe91a0286a`  
		Last Modified: Thu, 02 Mar 2023 03:59:00 GMT  
		Size: 183.9 MB (183871503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:12b2add676326f2ab7c9553ca93e55ceb7640c89c52e5bcdc60e9484b4b9c6e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223696347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399d1ff49dcb964c6fe2e7466d4807493aa3b92c5a22902cec1a41816285b263`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:10:39 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:10:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:41 GMT
ADD file:db14dc9a9d330115a6699be3c4a344f5fe366ec17e7d3649c4ecb2711605e52b in / 
# Wed, 01 Mar 2023 05:10:41 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:09:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:10:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:10:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:12:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:905ef75a23211c85ea45c3aa7f7e77bc95a94ff8c250e03412ef8c50b5fb9f49`  
		Last Modified: Thu, 02 Mar 2023 02:23:13 GMT  
		Size: 28.6 MB (28647596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f21104d1d70c25a181a183058f1061378e9d8c535e59e4c939c4231cbc970c`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.8 MB (3792871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8e321da5315972e394da4ba438abe2fd4085876b6ea43578a0324a68aeb100`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.5 MB (3472941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67223d18224c8c78226be471d16442159e0754a6cda26186d8d1c072820e289`  
		Last Modified: Thu, 02 Mar 2023 02:23:25 GMT  
		Size: 39.3 MB (39283485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21d051fa1c50a914eaa8e87cb3231ff4fc1430fd743c0041c286058b0aede2`  
		Last Modified: Thu, 02 Mar 2023 02:23:51 GMT  
		Size: 148.5 MB (148499454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-curl`

```console
$ docker pull buildpack-deps@sha256:46d4df86174ba0e17a6931431f2f0caecdae8ec50baf93c22de21a4e985cd39a
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
$ docker pull buildpack-deps@sha256:7c4181266db1c499d5050004a6bd81130b4c69a731b3b0f3132946a33813175e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37780231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c24181609005d131d0d93aad7eda4e076a45e610fd9e7e734349f901c88fb89e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b17938a1a752564000a3a0aeed04eafc6958f178a7fcc09094daa31ec80767`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.8 MB (3788644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51ade0caaff8e59d92682e80d534ad83b8bc2d760bbe60eb56dc0363c60b4d6`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.6 MB (3561585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:79d98c78e452391dc6f0dc841826fb7db37e2210bc46c84b842aa5170dd1cbda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34277689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f47a341c042acdfabe711f0519c94b2421c00a3ac0cf4f275853ad071a7a7b1c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:45:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:45:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:45:58 GMT
ADD file:d8e0c2340f91ec5973c8459c1a917be69f6530fe7f88da02eb5b4dd562c31730 in / 
# Wed, 01 Mar 2023 04:45:59 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:38:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:38:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5909c79a6169dfa05f978dbe7f8dfeadbb92a0d4a3a4d792314b3afe271dd793`  
		Last Modified: Wed, 01 Mar 2023 08:59:31 GMT  
		Size: 27.0 MB (27024489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e834b31ec46c994de883b1d8fd540229984065b7116dc8dab706aa6969bd5bff`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.5 MB (3539420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2617d031bbc0245044288b2afe503e376a8d9b8ded256246d64c969d12c85e7c`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.7 MB (3713780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:38af74bfc05f15a56d777c62d1184b40ec93ce4d4c5d7d2fe990ed9b898cfb5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35685491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6749e86ca4413cec2f058d6100e25f4dc008d155670d61e528de5f43d1dcd5e0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:21:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ecb6dff9238e75e6877b0624e8c0054bcb5d51c97f5f178a8a699de3e06572`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.8 MB (3760955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb16d0d18eaee62625a39492bf99dabbc71b2e3d6278c10a2080894ebe562b`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.5 MB (3536614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ec09f10603891c397a34727e768f3669e5f99ddd77f3e82242399bb18f778d89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44208684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c1fea401154387820e29c3d48abd9cd1a45519ae1df49fffce659c7057defe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:09:57 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:09:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:01 GMT
ADD file:e4d45fbda8cf3ca1613a11d2b929670e0e12b43c66818636afa9ebcbf6b48b59 in / 
# Wed, 01 Mar 2023 05:10:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:28:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:062a5dd6f1a8faa2ffa6ca3db2cdb7e930e5f49f52c8647b30709399b759b1cb`  
		Last Modified: Thu, 02 Mar 2023 03:35:30 GMT  
		Size: 35.7 MB (35711589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387fa66f2465a45a4bf52efe7a70d02b4b563ea79f4a05b59a132253b6fd192c`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.3 MB (4262192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3313c961eddc996b17782dfb540ee65ee6801254d9ee09d82691b5a9f66f7431`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.2 MB (4234903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d3dbf3f2437dac5abae4e64090c5389d96c98ea170f5cdca2e3fef799054f757
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35913408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad46ce92dd1a41929e464c3d4f34611b73f1494aef4327fce99ab635e5976d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:10:39 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:10:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:41 GMT
ADD file:db14dc9a9d330115a6699be3c4a344f5fe366ec17e7d3649c4ecb2711605e52b in / 
# Wed, 01 Mar 2023 05:10:41 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:09:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:10:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:905ef75a23211c85ea45c3aa7f7e77bc95a94ff8c250e03412ef8c50b5fb9f49`  
		Last Modified: Thu, 02 Mar 2023 02:23:13 GMT  
		Size: 28.6 MB (28647596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f21104d1d70c25a181a183058f1061378e9d8c535e59e4c939c4231cbc970c`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.8 MB (3792871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8e321da5315972e394da4ba438abe2fd4085876b6ea43578a0324a68aeb100`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.5 MB (3472941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-scm`

```console
$ docker pull buildpack-deps@sha256:309fa57d4ff4c368763213a7e066d1b87cc15fe0949c124f3a7ed8430c4bcd1c
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
$ docker pull buildpack-deps@sha256:3483a701ce591a55e4782a4fb689bd1e0385394d2485d7785a88b9887508be2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77133371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bfb7a7ac339b586fd2b8395f35c7994ba14c08eaf2062e13ef0dfa8eeb378b5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b17938a1a752564000a3a0aeed04eafc6958f178a7fcc09094daa31ec80767`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.8 MB (3788644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51ade0caaff8e59d92682e80d534ad83b8bc2d760bbe60eb56dc0363c60b4d6`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.6 MB (3561585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b8264f0fdf1f57cc3ac8b5b09faac810a388350812478b3dc2ab19727db68`  
		Last Modified: Thu, 02 Mar 2023 03:44:15 GMT  
		Size: 39.4 MB (39353140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:62d7932743dea29053da8801145b2aeae07aa06c8644a0b1ae37169877a25931
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76185370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3983d506885a6b142e0303d98015fc347be1fd11dcad071209eac93543f226a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:45:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:45:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:45:58 GMT
ADD file:d8e0c2340f91ec5973c8459c1a917be69f6530fe7f88da02eb5b4dd562c31730 in / 
# Wed, 01 Mar 2023 04:45:59 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:38:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:38:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:39:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5909c79a6169dfa05f978dbe7f8dfeadbb92a0d4a3a4d792314b3afe271dd793`  
		Last Modified: Wed, 01 Mar 2023 08:59:31 GMT  
		Size: 27.0 MB (27024489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e834b31ec46c994de883b1d8fd540229984065b7116dc8dab706aa6969bd5bff`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.5 MB (3539420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2617d031bbc0245044288b2afe503e376a8d9b8ded256246d64c969d12c85e7c`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.7 MB (3713780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffb58fb6ee1096d3a9785f5fd877bff68fdae04f23374b1f8753549f2dfa0e8`  
		Last Modified: Thu, 02 Mar 2023 11:56:38 GMT  
		Size: 41.9 MB (41907681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c3524bdfa214bd2069033b2a4d4338b5d9d4d33b164980d265a64999c9ca18df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74928318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82fbeb6451e8bf8f6ebe5aaf0501691761c3562fff522fc1c688f5c76d97492`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:21:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:22:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ecb6dff9238e75e6877b0624e8c0054bcb5d51c97f5f178a8a699de3e06572`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.8 MB (3760955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb16d0d18eaee62625a39492bf99dabbc71b2e3d6278c10a2080894ebe562b`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.5 MB (3536614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088d8f170fef46d01bbb6cd7b616c91b38f4fcad2ab1b42e1d93e9d86a7febe9`  
		Last Modified: Thu, 02 Mar 2023 02:37:34 GMT  
		Size: 39.2 MB (39242827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:de685636ac1d95144c9e8a8c6e6a46b21dc77204fffc1f53622024051a964e0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87977130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab13bb48e1dc22e897444373d0821d94c43a5d25afb1701dbaf505970e8637e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:09:57 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:09:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:01 GMT
ADD file:e4d45fbda8cf3ca1613a11d2b929670e0e12b43c66818636afa9ebcbf6b48b59 in / 
# Wed, 01 Mar 2023 05:10:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:28:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:062a5dd6f1a8faa2ffa6ca3db2cdb7e930e5f49f52c8647b30709399b759b1cb`  
		Last Modified: Thu, 02 Mar 2023 03:35:30 GMT  
		Size: 35.7 MB (35711589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387fa66f2465a45a4bf52efe7a70d02b4b563ea79f4a05b59a132253b6fd192c`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.3 MB (4262192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3313c961eddc996b17782dfb540ee65ee6801254d9ee09d82691b5a9f66f7431`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.2 MB (4234903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ba7916137f91162c1002b749a8a79118a1565f3a770f8d4d9415bd64e78b8b`  
		Last Modified: Thu, 02 Mar 2023 03:58:05 GMT  
		Size: 43.8 MB (43768446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b9176765891a17832f7daca48b461c8953219e5f2188240da03d66f1191bcfdf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75196893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b4d8150feeab5b80dcb010823460e54fcfd72b565b3e8820923c650ef60d391`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:10:39 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:10:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:41 GMT
ADD file:db14dc9a9d330115a6699be3c4a344f5fe366ec17e7d3649c4ecb2711605e52b in / 
# Wed, 01 Mar 2023 05:10:41 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:09:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:10:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:10:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:905ef75a23211c85ea45c3aa7f7e77bc95a94ff8c250e03412ef8c50b5fb9f49`  
		Last Modified: Thu, 02 Mar 2023 02:23:13 GMT  
		Size: 28.6 MB (28647596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f21104d1d70c25a181a183058f1061378e9d8c535e59e4c939c4231cbc970c`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.8 MB (3792871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8e321da5315972e394da4ba438abe2fd4085876b6ea43578a0324a68aeb100`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.5 MB (3472941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67223d18224c8c78226be471d16442159e0754a6cda26186d8d1c072820e289`  
		Last Modified: Thu, 02 Mar 2023 02:23:25 GMT  
		Size: 39.3 MB (39283485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10`

```console
$ docker pull buildpack-deps@sha256:3de898d7deb52f63ea659a9406465b2011f5e5d9c42bdbd02c3986a636fdfc85
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
$ docker pull buildpack-deps@sha256:495e9e8ec9026b48115b0d3f8d00ec6f5bf85d394a2b182f021ac0e53b031832
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.7 MB (258747951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba0b089f69567a45c75ccfcde23ba31fa81898eb602bd9a598942df1988a767`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:43:07 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:43:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:43:09 GMT
ADD file:18f562911635a03a9bf9e5fc22863fc2a78a64f7d35c7daa59f2d609b7ca055a in / 
# Mon, 20 Feb 2023 11:43:10 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:33:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:34:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:34:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a10df61efde6b7f0cf3fbf848a5bed1c943a54e13566f30ef6a0cc6f259a2f33`  
		Last Modified: Thu, 02 Mar 2023 03:44:58 GMT  
		Size: 27.5 MB (27479398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9f9f71b0155b4b832dcb9bfbf542389507996cd93239b78300535c9421961`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 6.8 MB (6770219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710e0dcd6284a414a9f90e76d5555002980ba77c51b01d6a812e56d2c2d94d2e`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 3.6 MB (3635116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c20cf6be4d508b2c166988b50c5ae18cead28e74cf5a620d56202faabfe64a`  
		Last Modified: Thu, 02 Mar 2023 03:45:14 GMT  
		Size: 39.7 MB (39740010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050e88152487e2ad34afbd56fbc9c0f572f844c942044c6340d15392d91a0952`  
		Last Modified: Thu, 02 Mar 2023 03:45:47 GMT  
		Size: 181.1 MB (181123208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f636fdcf52a029e7d45340728ba354563227e08d26f89e19c7ab7d6b0021388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221869394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26553e21166cc99d3951d5842347777794fc253327acdb39b126f177bdd39e0f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 12:11:32 GMT
ARG RELEASE
# Mon, 20 Feb 2023 12:11:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 12:11:42 GMT
ADD file:f77393d0d614b99f7ca8de09afc58a2e98d9d25c84c5ff69b50e94e7f191f7bb in / 
# Mon, 20 Feb 2023 12:11:43 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:43:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:43:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:44:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:47:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e07337a9bc2a6220f565efbaf0abbba7718bb8478f0af5b255df655e98cacc06`  
		Last Modified: Thu, 02 Mar 2023 11:57:20 GMT  
		Size: 25.9 MB (25893079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84854174ca4e4c0ad5221cd0bface3a62279cc1659c26e61319a54c79f28a32`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 5.9 MB (5941095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcf439bd51bffc866ae5a81a2764cc54c7f76949d34e14d2ef5666243a5c9e6`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 3.8 MB (3801108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f989583c8ba595c2fb646ad093cc454bdb75e54ffe38ddcab4b7dc16bdb7e049`  
		Last Modified: Thu, 02 Mar 2023 11:57:37 GMT  
		Size: 42.6 MB (42607751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295db91297f7f8abb0622ff7a5f4c016e6ac8ee683a7b68eb6cd5b3acc813cfe`  
		Last Modified: Thu, 02 Mar 2023 11:58:07 GMT  
		Size: 143.6 MB (143626361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c58b5202654dafd061c9cea886f8415d96e7944c8edcf5c8080c0a0891595872
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.7 MB (246708749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d03b850f658d961584bce6f1511e1c4d58e7334d4dba0ab3ab1ad8d1f9bce2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:58:05 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:58:13 GMT
ADD file:7e756337f8554849df664b30203a26f6c39dc303e277292de31fd784b9ff471b in / 
# Mon, 20 Feb 2023 11:58:13 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:26:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:27:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:30:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30762c7e5d854e6efb956328165eb8c43cbcf6c0be6766a45d3a13fc1e1f56d3`  
		Last Modified: Thu, 02 Mar 2023 02:38:12 GMT  
		Size: 26.7 MB (26699035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a3333370dc8d23b791b4a6098f7f5a10c7edf844266e90f4027f4e85981b72`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 6.6 MB (6598072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f663586508fee1a498937d0779dfdbae3bcdd16334d54ee9295ca50aae552925`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 3.6 MB (3601892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce67b0569d875d7056824c4c9c02ac70786fa3b8901c3ba0c6a858c857ce0bd`  
		Last Modified: Thu, 02 Mar 2023 02:38:26 GMT  
		Size: 39.5 MB (39513912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0db24a7a1ff9ccf851045d646cb819453ab387ed800c01a3a0f234fa8c71c3`  
		Last Modified: Thu, 02 Mar 2023 02:38:52 GMT  
		Size: 170.3 MB (170295838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:da85a6b734638362d2f993972e3b8ec68846eb431f3f2fdeedf687d8ac682289
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281316326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f776e0dbfe7e0b9c9603f7c9158b78045c957cc54cef4b5ea1b4a69a99d04fb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:56:23 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:56:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:56:27 GMT
ADD file:541d2da8938972bd21842a8a4c8d2074a201f6f70eec4400110f90f1bc28f0e1 in / 
# Mon, 20 Feb 2023 11:56:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:39:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:afd8565abf9be19b25020425f0eef75bc6822497a915ac2ad7e299221258381b`  
		Last Modified: Thu, 02 Mar 2023 03:59:19 GMT  
		Size: 32.1 MB (32109672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c606979686591e3e15c259fedc8c72d14b5f5cb30789d4ac4fc1e7b2344079`  
		Last Modified: Thu, 02 Mar 2023 03:59:13 GMT  
		Size: 7.7 MB (7747700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30e23fe35619983be2169d8e199c937a090ab1f2c783261d342664a3574b67`  
		Last Modified: Thu, 02 Mar 2023 03:59:12 GMT  
		Size: 4.4 MB (4362546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738d753846623f2bf928d9c5ee5e40f7f523f14dd1df06fa8cb96528ab78ea3d`  
		Last Modified: Thu, 02 Mar 2023 03:59:42 GMT  
		Size: 44.1 MB (44141551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4808e644763bc63b9e5a0012ee36f28595205b8ba752baa09653edc02b649d9`  
		Last Modified: Thu, 02 Mar 2023 04:00:40 GMT  
		Size: 193.0 MB (192954857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8f715a88742ef8c20c9effa99fd07f25badf877ba6c4b81a7dbcca330da9f3a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228623596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4de103be19308a9f31f03e0d9527d2b7acda4dcae2f487b70ae0d2fe2d3ac6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:44:03 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:44:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:44:05 GMT
ADD file:9d71356e3a29a835345254e233ddbd3a67941764476c2c7a5a2d0f8a61a84115 in / 
# Mon, 20 Feb 2023 11:44:05 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:13:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:13:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:15:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bcfec0e313701229d74107ece843bd247955551cd676760c2ab56d6fbf1b157`  
		Last Modified: Thu, 02 Mar 2023 02:24:05 GMT  
		Size: 26.0 MB (26029678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741bf338192206d205e17575928e1ec37123b068da0fbfb2c33ff60198620f61`  
		Last Modified: Thu, 02 Mar 2023 02:23:59 GMT  
		Size: 6.5 MB (6461557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19aa30c75a1427834711cd28f44ba117f910f7b5c4e50f923f34ea300cd0cd`  
		Last Modified: Thu, 02 Mar 2023 02:23:58 GMT  
		Size: 3.6 MB (3625033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810d2ec3d82d4c030df6fc52d887b2bb1e9a1c9f01e957fe9dfcdea137a33d2`  
		Last Modified: Thu, 02 Mar 2023 02:24:19 GMT  
		Size: 39.6 MB (39555093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550cbac5a853fefec1b90b7e5a36dd208f74c615aaa79029f1a99c6fc499c3e2`  
		Last Modified: Thu, 02 Mar 2023 02:24:46 GMT  
		Size: 153.0 MB (152952235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-curl`

```console
$ docker pull buildpack-deps@sha256:90955da3a53928299fa7a945b4072d569c0739bcce57a8472b481888082d4e99
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
$ docker pull buildpack-deps@sha256:c1bef77a747c1b0d0e2e1943063d242d97b14090c6fa5a4396872c2e5e86cd7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37884733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f070e17b881f324f200c61c5d2fbd431ae10cc95570becf16c69abab64af58b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:43:07 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:43:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:43:09 GMT
ADD file:18f562911635a03a9bf9e5fc22863fc2a78a64f7d35c7daa59f2d609b7ca055a in / 
# Mon, 20 Feb 2023 11:43:10 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:33:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:34:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a10df61efde6b7f0cf3fbf848a5bed1c943a54e13566f30ef6a0cc6f259a2f33`  
		Last Modified: Thu, 02 Mar 2023 03:44:58 GMT  
		Size: 27.5 MB (27479398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9f9f71b0155b4b832dcb9bfbf542389507996cd93239b78300535c9421961`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 6.8 MB (6770219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710e0dcd6284a414a9f90e76d5555002980ba77c51b01d6a812e56d2c2d94d2e`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 3.6 MB (3635116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b87d2b37a07f2b3373c8b775d1355e3139b302bd1713c89dcdbe11519b218229
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35635282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d205c4c1777db2634384c44cf05affec171465def20dbcbf581b53881c97c8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 12:11:32 GMT
ARG RELEASE
# Mon, 20 Feb 2023 12:11:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 12:11:42 GMT
ADD file:f77393d0d614b99f7ca8de09afc58a2e98d9d25c84c5ff69b50e94e7f191f7bb in / 
# Mon, 20 Feb 2023 12:11:43 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:43:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:43:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e07337a9bc2a6220f565efbaf0abbba7718bb8478f0af5b255df655e98cacc06`  
		Last Modified: Thu, 02 Mar 2023 11:57:20 GMT  
		Size: 25.9 MB (25893079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84854174ca4e4c0ad5221cd0bface3a62279cc1659c26e61319a54c79f28a32`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 5.9 MB (5941095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcf439bd51bffc866ae5a81a2764cc54c7f76949d34e14d2ef5666243a5c9e6`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 3.8 MB (3801108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3c113e07442a77b7e938f4bc9ef5b846f44b9cbbdc3cfc058ba264eb8738928d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36898999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caca0113519d729a4a7c61672a55b06acb176ea63c6920446e280ef75b4dca74`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:58:05 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:58:13 GMT
ADD file:7e756337f8554849df664b30203a26f6c39dc303e277292de31fd784b9ff471b in / 
# Mon, 20 Feb 2023 11:58:13 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:26:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:30762c7e5d854e6efb956328165eb8c43cbcf6c0be6766a45d3a13fc1e1f56d3`  
		Last Modified: Thu, 02 Mar 2023 02:38:12 GMT  
		Size: 26.7 MB (26699035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a3333370dc8d23b791b4a6098f7f5a10c7edf844266e90f4027f4e85981b72`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 6.6 MB (6598072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f663586508fee1a498937d0779dfdbae3bcdd16334d54ee9295ca50aae552925`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 3.6 MB (3601892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:28895716799511a352dbc3b87633877569c448c91716b07fafceed861075e0ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44219918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb34ae855f68523ba0fb2c64a0473de1fc81baf2afdac185774fc659174ca56f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:56:23 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:56:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:56:27 GMT
ADD file:541d2da8938972bd21842a8a4c8d2074a201f6f70eec4400110f90f1bc28f0e1 in / 
# Mon, 20 Feb 2023 11:56:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:afd8565abf9be19b25020425f0eef75bc6822497a915ac2ad7e299221258381b`  
		Last Modified: Thu, 02 Mar 2023 03:59:19 GMT  
		Size: 32.1 MB (32109672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c606979686591e3e15c259fedc8c72d14b5f5cb30789d4ac4fc1e7b2344079`  
		Last Modified: Thu, 02 Mar 2023 03:59:13 GMT  
		Size: 7.7 MB (7747700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30e23fe35619983be2169d8e199c937a090ab1f2c783261d342664a3574b67`  
		Last Modified: Thu, 02 Mar 2023 03:59:12 GMT  
		Size: 4.4 MB (4362546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b0150ef7049140aa70bbf29415a11063465c948a00c24d38fa2fbb671f63a581
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36116268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:493a98847f6a760a3d453b6d316eb112b0f292f9513022c75fa6a97376df7fe4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:44:03 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:44:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:44:05 GMT
ADD file:9d71356e3a29a835345254e233ddbd3a67941764476c2c7a5a2d0f8a61a84115 in / 
# Mon, 20 Feb 2023 11:44:05 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:13:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:13:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8bcfec0e313701229d74107ece843bd247955551cd676760c2ab56d6fbf1b157`  
		Last Modified: Thu, 02 Mar 2023 02:24:05 GMT  
		Size: 26.0 MB (26029678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741bf338192206d205e17575928e1ec37123b068da0fbfb2c33ff60198620f61`  
		Last Modified: Thu, 02 Mar 2023 02:23:59 GMT  
		Size: 6.5 MB (6461557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19aa30c75a1427834711cd28f44ba117f910f7b5c4e50f923f34ea300cd0cd`  
		Last Modified: Thu, 02 Mar 2023 02:23:58 GMT  
		Size: 3.6 MB (3625033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-scm`

```console
$ docker pull buildpack-deps@sha256:b0e53314b314ebf0ffb12bb21dd7d20a6a45fca68be9c9775074c8769779be87
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
$ docker pull buildpack-deps@sha256:047a981c3c4d581bea16d7a0cd289b348dfa07629f24b6cc7f6add1dcc94d1aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77624743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc182bbb00ba8809b6ffb1c35841b67fd97eba00c6901a88c09dde29acd761f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:43:07 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:43:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:43:09 GMT
ADD file:18f562911635a03a9bf9e5fc22863fc2a78a64f7d35c7daa59f2d609b7ca055a in / 
# Mon, 20 Feb 2023 11:43:10 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:33:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:34:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:34:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a10df61efde6b7f0cf3fbf848a5bed1c943a54e13566f30ef6a0cc6f259a2f33`  
		Last Modified: Thu, 02 Mar 2023 03:44:58 GMT  
		Size: 27.5 MB (27479398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9f9f71b0155b4b832dcb9bfbf542389507996cd93239b78300535c9421961`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 6.8 MB (6770219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710e0dcd6284a414a9f90e76d5555002980ba77c51b01d6a812e56d2c2d94d2e`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 3.6 MB (3635116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c20cf6be4d508b2c166988b50c5ae18cead28e74cf5a620d56202faabfe64a`  
		Last Modified: Thu, 02 Mar 2023 03:45:14 GMT  
		Size: 39.7 MB (39740010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:40dd970891c5342e622abad06cef1abb7a1028fba4ea2e2cac5ba2e86654970d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78243033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b55dc8cebae19b3759058aa86d016dbd0c5b250a29ad01f961ea9507b3a27e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 12:11:32 GMT
ARG RELEASE
# Mon, 20 Feb 2023 12:11:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 12:11:42 GMT
ADD file:f77393d0d614b99f7ca8de09afc58a2e98d9d25c84c5ff69b50e94e7f191f7bb in / 
# Mon, 20 Feb 2023 12:11:43 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:43:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:43:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:44:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e07337a9bc2a6220f565efbaf0abbba7718bb8478f0af5b255df655e98cacc06`  
		Last Modified: Thu, 02 Mar 2023 11:57:20 GMT  
		Size: 25.9 MB (25893079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84854174ca4e4c0ad5221cd0bface3a62279cc1659c26e61319a54c79f28a32`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 5.9 MB (5941095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcf439bd51bffc866ae5a81a2764cc54c7f76949d34e14d2ef5666243a5c9e6`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 3.8 MB (3801108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f989583c8ba595c2fb646ad093cc454bdb75e54ffe38ddcab4b7dc16bdb7e049`  
		Last Modified: Thu, 02 Mar 2023 11:57:37 GMT  
		Size: 42.6 MB (42607751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:88e78a3e652b4b1af808021cb0b7be8e51482011249ba472e8c57ca4c852bdce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76412911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b558fd4728f4339d55d53189136d2d8d5681ab84008e295f189ebb8e86b603e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:58:05 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:58:13 GMT
ADD file:7e756337f8554849df664b30203a26f6c39dc303e277292de31fd784b9ff471b in / 
# Mon, 20 Feb 2023 11:58:13 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:26:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:27:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30762c7e5d854e6efb956328165eb8c43cbcf6c0be6766a45d3a13fc1e1f56d3`  
		Last Modified: Thu, 02 Mar 2023 02:38:12 GMT  
		Size: 26.7 MB (26699035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a3333370dc8d23b791b4a6098f7f5a10c7edf844266e90f4027f4e85981b72`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 6.6 MB (6598072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f663586508fee1a498937d0779dfdbae3bcdd16334d54ee9295ca50aae552925`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 3.6 MB (3601892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce67b0569d875d7056824c4c9c02ac70786fa3b8901c3ba0c6a858c857ce0bd`  
		Last Modified: Thu, 02 Mar 2023 02:38:26 GMT  
		Size: 39.5 MB (39513912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:88398a25e6df8710f62c22d86345a8fa3f84e0713a6ac0c996896c2bcac959ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88361469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1049a1bbcae803adb4a16ecc2adb582978810a7ddfb5ea9ec24da206f4be1ce1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:56:23 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:56:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:56:27 GMT
ADD file:541d2da8938972bd21842a8a4c8d2074a201f6f70eec4400110f90f1bc28f0e1 in / 
# Mon, 20 Feb 2023 11:56:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:39:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:afd8565abf9be19b25020425f0eef75bc6822497a915ac2ad7e299221258381b`  
		Last Modified: Thu, 02 Mar 2023 03:59:19 GMT  
		Size: 32.1 MB (32109672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c606979686591e3e15c259fedc8c72d14b5f5cb30789d4ac4fc1e7b2344079`  
		Last Modified: Thu, 02 Mar 2023 03:59:13 GMT  
		Size: 7.7 MB (7747700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30e23fe35619983be2169d8e199c937a090ab1f2c783261d342664a3574b67`  
		Last Modified: Thu, 02 Mar 2023 03:59:12 GMT  
		Size: 4.4 MB (4362546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738d753846623f2bf928d9c5ee5e40f7f523f14dd1df06fa8cb96528ab78ea3d`  
		Last Modified: Thu, 02 Mar 2023 03:59:42 GMT  
		Size: 44.1 MB (44141551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fb2be6a90e849d0cee6c46ce77e713c60d83023e6b19401fffbdaf695bc333a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75671361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecf79aedb1597b523736958d2e35a21cb919903f602fc38c3a7ac2730bd0d59`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:44:03 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:44:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:44:05 GMT
ADD file:9d71356e3a29a835345254e233ddbd3a67941764476c2c7a5a2d0f8a61a84115 in / 
# Mon, 20 Feb 2023 11:44:05 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:13:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:13:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bcfec0e313701229d74107ece843bd247955551cd676760c2ab56d6fbf1b157`  
		Last Modified: Thu, 02 Mar 2023 02:24:05 GMT  
		Size: 26.0 MB (26029678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741bf338192206d205e17575928e1ec37123b068da0fbfb2c33ff60198620f61`  
		Last Modified: Thu, 02 Mar 2023 02:23:59 GMT  
		Size: 6.5 MB (6461557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19aa30c75a1427834711cd28f44ba117f910f7b5c4e50f923f34ea300cd0cd`  
		Last Modified: Thu, 02 Mar 2023 02:23:58 GMT  
		Size: 3.6 MB (3625033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810d2ec3d82d4c030df6fc52d887b2bb1e9a1c9f01e957fe9dfcdea137a33d2`  
		Last Modified: Thu, 02 Mar 2023 02:24:19 GMT  
		Size: 39.6 MB (39555093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04`

```console
$ docker pull buildpack-deps@sha256:8c345dca9c9fc0c22ebf88e7b956b00b5e91fcc28bb20ed50f22942cfccb0b9e
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
$ docker pull buildpack-deps@sha256:dd059c3bad41c1793f0bda5fc655d3f11e84347d773ad26d8f8f9e33c667ff84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.4 MB (279400819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1152e1ec96916d1e0da389234ee993c5d6910729d6c68faaefec28f6ffb24d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:14 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:16 GMT
ADD file:a99f804e480d9a1b56aff6406b4da5a3dea89f11f968e5e02cd4ba5a25e9a7bc in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:38:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:41:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6347900c239eb6451b578d272779198ff2efe221eb716c1ee35bb33b3d36c805`  
		Last Modified: Thu, 02 Mar 2023 03:45:59 GMT  
		Size: 27.5 MB (27450641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fc9b499f00984f063653ce41c5bcd7a2101d4709bde16211c9cd61cf53c97`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 6.6 MB (6637316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583126b5de1692321379f3ac3c479e60776c2630177157537ce16c3b5310534c`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 3.7 MB (3690222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4e53abb79424a77d128c854eb7fbd2dc2baf538b9618ecdc1377d5c513a4d`  
		Last Modified: Thu, 02 Mar 2023 03:46:14 GMT  
		Size: 44.5 MB (44515661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a67102021c513567e5ad98778b40b5627ec23a5472f9c98da44bd4a7a1529`  
		Last Modified: Thu, 02 Mar 2023 03:46:53 GMT  
		Size: 197.1 MB (197106979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4b44c93e90c08a0c8ebe34455d42edaee9ca6bbc11842ce669bb625fc4076c8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.4 MB (230379620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca6c0fae7a4451d14049e9b225c0e7940914f5ca0a2808b4cf73cd9f97e1462`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:43 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:44 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:53 GMT
ADD file:e4ec0e899927e1fe0388f3524f3382183df8c74bcf9de0e35e1c8120acbc2b7a in / 
# Wed, 01 Mar 2023 05:41:53 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:48:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:48:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:49:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:51:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3149fccce04237916ad21629e6497df2edac53a12b13cf63470e4ee5833f8e4`  
		Last Modified: Thu, 02 Mar 2023 11:58:22 GMT  
		Size: 26.2 MB (26236811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1c91da9e0e927655ec912d3e65425143bf9d0dc2bde931112305247aa3dca7`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 5.8 MB (5809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee07824f253241f1cd1a7d308e85f8d6bfdb3649f0d1db1d5c49d1b1ff337a`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 3.9 MB (3852238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307ab9ceb5b6a487ea64bb9ab76e4c75483c4dd388afefcc036953ad0170c750`  
		Last Modified: Thu, 02 Mar 2023 11:58:40 GMT  
		Size: 48.6 MB (48604125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d587719a598d516477984ca010b771e6121e70f384a8612c804c4cbac316a`  
		Last Modified: Thu, 02 Mar 2023 11:59:09 GMT  
		Size: 145.9 MB (145877278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d8524c1c281222c12d123a4dc95c47e7b344cba0f7b944e9db5a7b76901c8e91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269571646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d507b30adaf2193c1c4e65e7384e76f5769f09ecb89a38418b845784e49b1599`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:57:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:57:22 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 04:57:30 GMT
ADD file:54e98f6282fdf165c9986b859ed60d05e28d3f9575c1c4915537cba24c6ec95c in / 
# Wed, 01 Mar 2023 04:57:31 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:30:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:31:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:34:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6700b5ef6bf750ef532062fc9dec24b7d9247840b877f26af1f339df77db5ba1`  
		Last Modified: Thu, 02 Mar 2023 02:39:03 GMT  
		Size: 26.9 MB (26899339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01eb5985b1759d7a00fafb6eaa0426c9ba33b24bab18656ae5ed19b74869bd3`  
		Last Modified: Thu, 02 Mar 2023 02:39:02 GMT  
		Size: 6.5 MB (6468687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136aa3449032f883f29b10908230ca4a5c79c1a4fcf12f1c28fa763b07ac0db`  
		Last Modified: Thu, 02 Mar 2023 02:39:01 GMT  
		Size: 3.6 MB (3649336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99899628512ddfc061595eb4f812d31ea2842eb378a4f491eb3ab8c133270a51`  
		Last Modified: Thu, 02 Mar 2023 02:39:17 GMT  
		Size: 44.4 MB (44350881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe305ba6cd09ca5b32809bcb5cbb3c76cfb40ef0bb6c985399edbe3a38611745`  
		Last Modified: Thu, 02 Mar 2023 02:39:45 GMT  
		Size: 188.2 MB (188203403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2c247cf6ae7ab7790b2e6ef7b6f22e062c03be67c2e6ec746c9e3028d4d9fdac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.6 MB (304625782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e1e8fb8f901f6cc5bea34fb55d0d589b98d798b4d46f5efa69fa124e3f78e10`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:58 GMT
ADD file:dd48763269678622cf7a1219a8b87a1222a24048b5cc1ab133a42cbb854c7f78 in / 
# Wed, 01 Mar 2023 05:00:58 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:52:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434ae6294eb01eccffad6e8e39b3f373d83e33cfedaa3f3cb70962a1122776f0`  
		Last Modified: Thu, 02 Mar 2023 04:01:02 GMT  
		Size: 31.9 MB (31897489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316ed6bd69a08f1739325fc66aebcc6c5bf34087b52b0f3a2e4bfca0c109e76d`  
		Last Modified: Thu, 02 Mar 2023 04:00:56 GMT  
		Size: 7.6 MB (7606587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba7fe918b6d86615ad6aaad9cb8d4e29030952575a61624dbb8f5e15f5ca8f9`  
		Last Modified: Thu, 02 Mar 2023 04:00:55 GMT  
		Size: 4.4 MB (4409088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0e010afca98d127a9b0d8607ac999fc79b19e8d612c6fc6e3a9e1ee1a1de76`  
		Last Modified: Thu, 02 Mar 2023 04:01:28 GMT  
		Size: 49.3 MB (49321485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf0a080521e887133fd7499f1530a995a4cd125cee300dc695cb79d843c68bb`  
		Last Modified: Thu, 02 Mar 2023 04:02:28 GMT  
		Size: 211.4 MB (211391133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e7e0da949a243441e9689733560d210e4400951613c1d2b5d97c7bb40587fa65
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.8 MB (250781790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a2a2bae085525070f7daabc96186ad663394847a35d43f5afe2d72617c073b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:55 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:57 GMT
ADD file:88bec1acfbc8ba8a59354ff2c1f510d9e301748628aa39527cca86d8150209e8 in / 
# Wed, 01 Mar 2023 05:00:57 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:16:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:17:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:19:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e8382b8ddc15579f4e533ad8581d16988174176dacd958bc0572d8e6417518f`  
		Last Modified: Thu, 02 Mar 2023 02:24:57 GMT  
		Size: 26.1 MB (26072339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2428ddac9d5ad4baa24cd9a8735e4aa63591aa90c5e18869189f772ac106cd2`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 6.3 MB (6319521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b57b8f1cbfb3971975200f23660e4e6bb616038be4ec693552ebd91f202ed1`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 3.7 MB (3674671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f1225557f2081b054aaa9ce9fa92db7eaf86f05602bd00bb497082952dd77c`  
		Last Modified: Thu, 02 Mar 2023 02:25:13 GMT  
		Size: 44.3 MB (44337360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787d7f0ffdc1c3dc79e056d7f534a0f5485a77be47f876d2965e7e4b1303ed1`  
		Last Modified: Thu, 02 Mar 2023 02:25:42 GMT  
		Size: 170.4 MB (170377899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-curl`

```console
$ docker pull buildpack-deps@sha256:ea0932754db65dc7cdd16c157b662925e1812053f5bd5bc536549998bdf2a2fd
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
$ docker pull buildpack-deps@sha256:4e65f9beff33426d8e782c4e765e86c5b79c6ff355c07b850a10a11557439a93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37778179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e37d1b86e663a732896bf3d39af7f0224e89bee8471e9c1bba9e4e100eaf04a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:14 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:16 GMT
ADD file:a99f804e480d9a1b56aff6406b4da5a3dea89f11f968e5e02cd4ba5a25e9a7bc in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6347900c239eb6451b578d272779198ff2efe221eb716c1ee35bb33b3d36c805`  
		Last Modified: Thu, 02 Mar 2023 03:45:59 GMT  
		Size: 27.5 MB (27450641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fc9b499f00984f063653ce41c5bcd7a2101d4709bde16211c9cd61cf53c97`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 6.6 MB (6637316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583126b5de1692321379f3ac3c479e60776c2630177157537ce16c3b5310534c`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 3.7 MB (3690222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a94b128e1356b799bc1441e88a775175a23a1ab09e255182bdf025735ab65a24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35898217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:393d2f7b0cbdfaba72c5950beec03aac8c5c421b400119d520b1541476804dc9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:43 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:44 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:53 GMT
ADD file:e4ec0e899927e1fe0388f3524f3382183df8c74bcf9de0e35e1c8120acbc2b7a in / 
# Wed, 01 Mar 2023 05:41:53 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:48:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:48:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f3149fccce04237916ad21629e6497df2edac53a12b13cf63470e4ee5833f8e4`  
		Last Modified: Thu, 02 Mar 2023 11:58:22 GMT  
		Size: 26.2 MB (26236811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1c91da9e0e927655ec912d3e65425143bf9d0dc2bde931112305247aa3dca7`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 5.8 MB (5809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee07824f253241f1cd1a7d308e85f8d6bfdb3649f0d1db1d5c49d1b1ff337a`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 3.9 MB (3852238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:29528af07c334f5ec5040c5656f9ff1b25e6a8fd192b3f2a05a2cb91c8ba94ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (37017362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b36694a82191fe66369b4b4b6a2d3d01d64ae1342857f637441504de865ca45a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:57:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:57:22 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 04:57:30 GMT
ADD file:54e98f6282fdf165c9986b859ed60d05e28d3f9575c1c4915537cba24c6ec95c in / 
# Wed, 01 Mar 2023 04:57:31 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:30:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6700b5ef6bf750ef532062fc9dec24b7d9247840b877f26af1f339df77db5ba1`  
		Last Modified: Thu, 02 Mar 2023 02:39:03 GMT  
		Size: 26.9 MB (26899339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01eb5985b1759d7a00fafb6eaa0426c9ba33b24bab18656ae5ed19b74869bd3`  
		Last Modified: Thu, 02 Mar 2023 02:39:02 GMT  
		Size: 6.5 MB (6468687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136aa3449032f883f29b10908230ca4a5c79c1a4fcf12f1c28fa763b07ac0db`  
		Last Modified: Thu, 02 Mar 2023 02:39:01 GMT  
		Size: 3.6 MB (3649336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:969acb495b97e4865f3a4be732f30166c4c8d498c36c2aa550561dbb09811de0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43913164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff2d43f367892255637542904d83ecd5cd4f07e36220da96cd5ec7e64cf1e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:58 GMT
ADD file:dd48763269678622cf7a1219a8b87a1222a24048b5cc1ab133a42cbb854c7f78 in / 
# Wed, 01 Mar 2023 05:00:58 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:434ae6294eb01eccffad6e8e39b3f373d83e33cfedaa3f3cb70962a1122776f0`  
		Last Modified: Thu, 02 Mar 2023 04:01:02 GMT  
		Size: 31.9 MB (31897489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316ed6bd69a08f1739325fc66aebcc6c5bf34087b52b0f3a2e4bfca0c109e76d`  
		Last Modified: Thu, 02 Mar 2023 04:00:56 GMT  
		Size: 7.6 MB (7606587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba7fe918b6d86615ad6aaad9cb8d4e29030952575a61624dbb8f5e15f5ca8f9`  
		Last Modified: Thu, 02 Mar 2023 04:00:55 GMT  
		Size: 4.4 MB (4409088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f899ac870d7e9fddcf8aa13caff6163265029ce5ce54986e8b09b54e73c198e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36066531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c53d3d23aef5fdf01fc69c9886733334a4d214bdfb2827d16fcc812fa5857d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:55 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:57 GMT
ADD file:88bec1acfbc8ba8a59354ff2c1f510d9e301748628aa39527cca86d8150209e8 in / 
# Wed, 01 Mar 2023 05:00:57 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:16:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9e8382b8ddc15579f4e533ad8581d16988174176dacd958bc0572d8e6417518f`  
		Last Modified: Thu, 02 Mar 2023 02:24:57 GMT  
		Size: 26.1 MB (26072339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2428ddac9d5ad4baa24cd9a8735e4aa63591aa90c5e18869189f772ac106cd2`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 6.3 MB (6319521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b57b8f1cbfb3971975200f23660e4e6bb616038be4ec693552ebd91f202ed1`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 3.7 MB (3674671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-scm`

```console
$ docker pull buildpack-deps@sha256:e2ce24a28c5ffa329922d8a7fd842b4f01e5dedae68529b743195ef776b5bdd2
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
$ docker pull buildpack-deps@sha256:dfca8dc06d26d3a6045ceef176d672df2185198782833ce82c81f3417487b7e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82293840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11db010a0e4873cf66ebbbaeb58004ef354ea6507c99ebed518c311dd06e6fe4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:14 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:16 GMT
ADD file:a99f804e480d9a1b56aff6406b4da5a3dea89f11f968e5e02cd4ba5a25e9a7bc in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:38:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6347900c239eb6451b578d272779198ff2efe221eb716c1ee35bb33b3d36c805`  
		Last Modified: Thu, 02 Mar 2023 03:45:59 GMT  
		Size: 27.5 MB (27450641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fc9b499f00984f063653ce41c5bcd7a2101d4709bde16211c9cd61cf53c97`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 6.6 MB (6637316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583126b5de1692321379f3ac3c479e60776c2630177157537ce16c3b5310534c`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 3.7 MB (3690222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4e53abb79424a77d128c854eb7fbd2dc2baf538b9618ecdc1377d5c513a4d`  
		Last Modified: Thu, 02 Mar 2023 03:46:14 GMT  
		Size: 44.5 MB (44515661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:13ccc3def0daf769539fd0ca304f2a28da88d5bb794c46c1f93916f458251517
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84502342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a304d21e8dd95ea8eeb55ef412cc1ac9bbd4acf5075c01142941f14b6f9005ce`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:43 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:44 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:53 GMT
ADD file:e4ec0e899927e1fe0388f3524f3382183df8c74bcf9de0e35e1c8120acbc2b7a in / 
# Wed, 01 Mar 2023 05:41:53 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:48:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:48:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:49:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3149fccce04237916ad21629e6497df2edac53a12b13cf63470e4ee5833f8e4`  
		Last Modified: Thu, 02 Mar 2023 11:58:22 GMT  
		Size: 26.2 MB (26236811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1c91da9e0e927655ec912d3e65425143bf9d0dc2bde931112305247aa3dca7`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 5.8 MB (5809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee07824f253241f1cd1a7d308e85f8d6bfdb3649f0d1db1d5c49d1b1ff337a`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 3.9 MB (3852238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307ab9ceb5b6a487ea64bb9ab76e4c75483c4dd388afefcc036953ad0170c750`  
		Last Modified: Thu, 02 Mar 2023 11:58:40 GMT  
		Size: 48.6 MB (48604125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4d2316040e83fb85fcf5553a00d9884e58bc4ae0ac45f809513198b31164f7a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81368243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78899799edcb9bb2076bbcfe6bcfb75f1dffa05836b5c21617593bc97cd03734`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:57:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:57:22 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 04:57:30 GMT
ADD file:54e98f6282fdf165c9986b859ed60d05e28d3f9575c1c4915537cba24c6ec95c in / 
# Wed, 01 Mar 2023 04:57:31 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:30:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:31:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6700b5ef6bf750ef532062fc9dec24b7d9247840b877f26af1f339df77db5ba1`  
		Last Modified: Thu, 02 Mar 2023 02:39:03 GMT  
		Size: 26.9 MB (26899339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01eb5985b1759d7a00fafb6eaa0426c9ba33b24bab18656ae5ed19b74869bd3`  
		Last Modified: Thu, 02 Mar 2023 02:39:02 GMT  
		Size: 6.5 MB (6468687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136aa3449032f883f29b10908230ca4a5c79c1a4fcf12f1c28fa763b07ac0db`  
		Last Modified: Thu, 02 Mar 2023 02:39:01 GMT  
		Size: 3.6 MB (3649336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99899628512ddfc061595eb4f812d31ea2842eb378a4f491eb3ab8c133270a51`  
		Last Modified: Thu, 02 Mar 2023 02:39:17 GMT  
		Size: 44.4 MB (44350881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:39d5d1468937ce1cd50fdd52cb7dfc5d713f2a7494ac3925626f12ee6e417278
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93234649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7fbab15a93c2f95048c838e9d8a6e32252fb4b63ec05dd2b4fec7ba3acaf270`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:58 GMT
ADD file:dd48763269678622cf7a1219a8b87a1222a24048b5cc1ab133a42cbb854c7f78 in / 
# Wed, 01 Mar 2023 05:00:58 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434ae6294eb01eccffad6e8e39b3f373d83e33cfedaa3f3cb70962a1122776f0`  
		Last Modified: Thu, 02 Mar 2023 04:01:02 GMT  
		Size: 31.9 MB (31897489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316ed6bd69a08f1739325fc66aebcc6c5bf34087b52b0f3a2e4bfca0c109e76d`  
		Last Modified: Thu, 02 Mar 2023 04:00:56 GMT  
		Size: 7.6 MB (7606587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba7fe918b6d86615ad6aaad9cb8d4e29030952575a61624dbb8f5e15f5ca8f9`  
		Last Modified: Thu, 02 Mar 2023 04:00:55 GMT  
		Size: 4.4 MB (4409088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0e010afca98d127a9b0d8607ac999fc79b19e8d612c6fc6e3a9e1ee1a1de76`  
		Last Modified: Thu, 02 Mar 2023 04:01:28 GMT  
		Size: 49.3 MB (49321485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d2881270036984bf5335b8711121ff83ff86c5a2728ced037c770bedde7b192b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80403891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a23c0ce9ee9418f0b679ceeecc5514d7858bc439fcffeb582fb2d84c7f6a80c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:55 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:57 GMT
ADD file:88bec1acfbc8ba8a59354ff2c1f510d9e301748628aa39527cca86d8150209e8 in / 
# Wed, 01 Mar 2023 05:00:57 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:16:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:17:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e8382b8ddc15579f4e533ad8581d16988174176dacd958bc0572d8e6417518f`  
		Last Modified: Thu, 02 Mar 2023 02:24:57 GMT  
		Size: 26.1 MB (26072339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2428ddac9d5ad4baa24cd9a8735e4aa63591aa90c5e18869189f772ac106cd2`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 6.3 MB (6319521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b57b8f1cbfb3971975200f23660e4e6bb616038be4ec693552ebd91f202ed1`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 3.7 MB (3674671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f1225557f2081b054aaa9ce9fa92db7eaf86f05602bd00bb497082952dd77c`  
		Last Modified: Thu, 02 Mar 2023 02:25:13 GMT  
		Size: 44.3 MB (44337360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:03240023737a69d26df22a353956e98e4af4fe6d91d700e10fd1e325cb67c762
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
$ docker pull buildpack-deps@sha256:bc6401af10396327da867114d7fa9e07ecc1fb018a0615961855e71cabd808f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221420553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0dfd86882423e6676ece77a524ae6979a584ed3b331070f0fc4919c9c7d0d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:22:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:24:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f64811d5f9e93d0cbbbaa74de2730a6dffbc3772747117377b98c979a5524e2`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 6.6 MB (6617385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed2ab5e0f15f7f6389f01ef48d5599f61173bb6c946ae3b9ece6d809e2708e5`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f631ab33a755e153343352043423161c6232b94c3be5472cd780d6fb66fea8c`  
		Last Modified: Thu, 02 Mar 2023 03:42:24 GMT  
		Size: 45.5 MB (45513091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3693810db0c477f5e446bed1c9a3f9865d9639040e32bd4f1b2c250f64c80`  
		Last Modified: Thu, 02 Mar 2023 03:42:51 GMT  
		Size: 139.6 MB (139552796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:74c75dac160e6a6002151711537eefa6221e1a817509f02c3a6ebb8f0a1d2fe4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189574487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be6314f5a99b1f96f4d5a67b9be2dc68d22a8a0b30b9db139bce7ab1504cab6f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:29:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:30:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:31:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:34:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6903cded2b3516e50f5bfdefd273774820e65f03bae3d1539678d6109df4e0b`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 5.7 MB (5679883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d900ce5096b9d98c4eacd5931071e9cf5fcc5869f19310d1c2fff7d3ed6806c5`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 2.6 MB (2585896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672070d854b2efbf7e9d5720a994ded06c4e58c97060013aed2981fd327517c`  
		Last Modified: Thu, 02 Mar 2023 11:54:45 GMT  
		Size: 40.7 MB (40712962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b18ca116489a29fab0bb7155fcb39757b6e5fdb884a900b7c2d82cd03ab0a7c`  
		Last Modified: Thu, 02 Mar 2023 11:55:11 GMT  
		Size: 118.3 MB (118291676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c4cd38688fc0d2dc220ac8ff6ce7b091691936713d7be77487926e5205d67d4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (206007032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a4b2640ef9ab7a7e44c1a782ebb8e68971a25d26f2d300bead677825ec2bf2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:15:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527f5e352ac533cdac8c50ce47e4185b349d1de4d8799f7529bb5d2524e4cb47`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 6.1 MB (6056649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea801ed12cc0807ef6ee95dca6e04d01bd2d6359efc54635d38d8a0516f55784`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 2.8 MB (2789532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491410c5ebb78636109cdab447342140dc9a4facbc978baa236f142ea8e9d64c`  
		Last Modified: Thu, 02 Mar 2023 02:35:57 GMT  
		Size: 43.3 MB (43312084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a641b744032c31a727a19848af95648856083d9ee3b2ddf4e6131d3b8906acfb`  
		Last Modified: Thu, 02 Mar 2023 02:36:19 GMT  
		Size: 130.1 MB (130115229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:23c1ee63e808b3015de5980d721e4f9af625420fbcf9252ac708b3f26db8b8b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218708206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfda599ee4752c06f38d2471001e45a94a340d988b3650bd203fd5a1588c358`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:14:52 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:14:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:14:54 GMT
ADD file:765a9704b3961cee9523a98bfd0de0f97b6075431287fa7b8acd276145cb28c5 in / 
# Wed, 01 Mar 2023 03:14:54 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 14:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 14:26:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 14:27:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 14:31:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08886b8b414bd4d4f6a196c5ea7306887e23ed3e5d83e9bde2bfe0cc2af99325`  
		Last Modified: Thu, 02 Mar 2023 14:23:47 GMT  
		Size: 27.2 MB (27164837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16105d5c202ba8ceca010766befe9c0bae4ef06768c5649bbdebe34feeff56c0`  
		Last Modified: Thu, 02 Mar 2023 14:32:49 GMT  
		Size: 6.9 MB (6907843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606120c77dd0e4dc08e0829cd5fda3c301d68a11a8561df02368984d18c27e87`  
		Last Modified: Thu, 02 Mar 2023 14:32:48 GMT  
		Size: 3.3 MB (3255738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd34df470431bd99fe8348a0b7488317fd90179a50fc094b1bc09cfdfff0f651`  
		Last Modified: Thu, 02 Mar 2023 14:33:08 GMT  
		Size: 47.1 MB (47097279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cc969ea617066b06bd1d2af21a782f627a3f869a71f0cfa604137bade66456`  
		Last Modified: Thu, 02 Mar 2023 14:33:44 GMT  
		Size: 134.3 MB (134282509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:67fa38311170cdba88af20aa1b89395545f3efab0a3834c4664d8e8a340919d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246443180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44bd848f8d90d8dcb294a19721d764751f19869aa2cd2088193c7cbc90598830`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:15:24 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:15:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:15:27 GMT
ADD file:ca5a453351fddb6d7937e334f0331321829a5bebca3d726ef3dddad1f23b35c8 in / 
# Wed, 01 Mar 2023 03:15:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:12:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:12:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:18:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:27fbc2bd86045e72ba8d9901b237295e3094b37f456824337175e24a0f0afe98`  
		Last Modified: Thu, 02 Mar 2023 03:09:44 GMT  
		Size: 30.4 MB (30442026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fe4259cc8ab209d172cd6c47536773db4959cf18257a7d3d47b35257e3547`  
		Last Modified: Thu, 02 Mar 2023 03:54:32 GMT  
		Size: 7.0 MB (7036861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1d5bf7bb9bbef4a44b4363f1e0fa9ed98fe35bd78d986830c40d35c1641e5`  
		Last Modified: Thu, 02 Mar 2023 03:54:31 GMT  
		Size: 3.7 MB (3740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68956dba4cc03b50dc85a017a1231e5796aa790462edfefff2e29d810938fac5`  
		Last Modified: Thu, 02 Mar 2023 03:54:58 GMT  
		Size: 53.7 MB (53737565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4b2678c674974ef6a718cfeeb751759ca159ee0b9fcad54a313bc2df75c588`  
		Last Modified: Thu, 02 Mar 2023 03:55:45 GMT  
		Size: 151.5 MB (151486173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7b015c146106a9d5bed63ce8160f10f595371332c37d694c7735dba418cd8154
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205761889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36218dc4a0ffa429ceecdc8268fc8a5f31517d1706b5e6a208e4f08a4b2f1d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:09 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:11 GMT
ADD file:49b5368b8703fe0aa128fe923b83da7ab2a30a7a1c0395682c905b9271e7f503 in / 
# Wed, 01 Mar 2023 03:18:11 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:02:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:03:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:03:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:05:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:306d1b363f89f239f5dc6314e0033094c067617b584ce004fd8db99402dab321`  
		Last Modified: Thu, 02 Mar 2023 02:21:31 GMT  
		Size: 25.4 MB (25371412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb206f9ee26b21514bd7026ed97956b03f4175d0d2096d5f87471b82c21903e8`  
		Last Modified: Thu, 02 Mar 2023 02:21:28 GMT  
		Size: 6.3 MB (6310489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732358426922e371a7b325dcc12fdff47050775aafd32bcf8884ed1ad12f120`  
		Last Modified: Thu, 02 Mar 2023 02:21:27 GMT  
		Size: 3.0 MB (2976715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f95174d0c3f8fa7400f2fe1baa0a15756c66695199991cb0126f6cd6586899`  
		Last Modified: Thu, 02 Mar 2023 02:21:45 GMT  
		Size: 45.0 MB (45039451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d6cdbea8d41a3597e61ccc469c9ed2051271cff3c92e5e98d2519cf49acb69`  
		Last Modified: Thu, 02 Mar 2023 02:22:09 GMT  
		Size: 126.1 MB (126063822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:73601edcb84c68e3c11b715ffee8e797dd05f0b388a2168c2301c4d90c3fc90d
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
$ docker pull buildpack-deps@sha256:99f85c256072d05e9bb8e3656852ae30bddc97653de13c5eb17cdc8b6dafd6f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36354666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111158ec462cd995c4c3e243b17f67d14fb75461904858179cf76df85ab57959`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f64811d5f9e93d0cbbbaa74de2730a6dffbc3772747117377b98c979a5524e2`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 6.6 MB (6617385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed2ab5e0f15f7f6389f01ef48d5599f61173bb6c946ae3b9ece6d809e2708e5`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9927f426d766fa71f28ffb9fdc683468b8289aa35a0ca6a188fe99b89131c37e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30569849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c454cb60b9b4cb6c88a731a1efe79dd872854170ce9ef7e0a743c199f56c2a5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:29:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:30:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6903cded2b3516e50f5bfdefd273774820e65f03bae3d1539678d6109df4e0b`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 5.7 MB (5679883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d900ce5096b9d98c4eacd5931071e9cf5fcc5869f19310d1c2fff7d3ed6806c5`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 2.6 MB (2585896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f7da0ac25d1397e53a187cd55f39a39a896c2cf7cc959c9cd02267a0f44e7d8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32579719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dda8439f80b101956498824b42467ff97d1b014933c44c7453c440a794eb6b48`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527f5e352ac533cdac8c50ce47e4185b349d1de4d8799f7529bb5d2524e4cb47`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 6.1 MB (6056649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea801ed12cc0807ef6ee95dca6e04d01bd2d6359efc54635d38d8a0516f55784`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 2.8 MB (2789532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e2b59c4e7bae90368ddf432e1950431ad277793049e5c6a436864b0e52ac95ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37328418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aab4d33e0dc6612a7eedbdd04c8e78eb35854e44466e8d83e7697737af98f25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:14:52 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:14:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:14:54 GMT
ADD file:765a9704b3961cee9523a98bfd0de0f97b6075431287fa7b8acd276145cb28c5 in / 
# Wed, 01 Mar 2023 03:14:54 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 14:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 14:26:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:08886b8b414bd4d4f6a196c5ea7306887e23ed3e5d83e9bde2bfe0cc2af99325`  
		Last Modified: Thu, 02 Mar 2023 14:23:47 GMT  
		Size: 27.2 MB (27164837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16105d5c202ba8ceca010766befe9c0bae4ef06768c5649bbdebe34feeff56c0`  
		Last Modified: Thu, 02 Mar 2023 14:32:49 GMT  
		Size: 6.9 MB (6907843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606120c77dd0e4dc08e0829cd5fda3c301d68a11a8561df02368984d18c27e87`  
		Last Modified: Thu, 02 Mar 2023 14:32:48 GMT  
		Size: 3.3 MB (3255738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b3626e1fc0df781ffdcd5858ddfd7e32cfd9a727dd64393d293bfa412fb7ed3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41219442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:969499ba388db8062c83aa23fbf2d2e1c8380f9bb88195a6da9832b5a5e02a73`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:15:24 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:15:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:15:27 GMT
ADD file:ca5a453351fddb6d7937e334f0331321829a5bebca3d726ef3dddad1f23b35c8 in / 
# Wed, 01 Mar 2023 03:15:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:12:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:12:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:27fbc2bd86045e72ba8d9901b237295e3094b37f456824337175e24a0f0afe98`  
		Last Modified: Thu, 02 Mar 2023 03:09:44 GMT  
		Size: 30.4 MB (30442026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fe4259cc8ab209d172cd6c47536773db4959cf18257a7d3d47b35257e3547`  
		Last Modified: Thu, 02 Mar 2023 03:54:32 GMT  
		Size: 7.0 MB (7036861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1d5bf7bb9bbef4a44b4363f1e0fa9ed98fe35bd78d986830c40d35c1641e5`  
		Last Modified: Thu, 02 Mar 2023 03:54:31 GMT  
		Size: 3.7 MB (3740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:774b1f4c6014651f88a0b380963c333bd8be99ad1c574dd6b97fe702508e3fef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34658616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d4a9dc5198a5458700a926e8863d1585e7baf6439d74278b821316e46bec3e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:09 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:11 GMT
ADD file:49b5368b8703fe0aa128fe923b83da7ab2a30a7a1c0395682c905b9271e7f503 in / 
# Wed, 01 Mar 2023 03:18:11 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:02:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:03:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:306d1b363f89f239f5dc6314e0033094c067617b584ce004fd8db99402dab321`  
		Last Modified: Thu, 02 Mar 2023 02:21:31 GMT  
		Size: 25.4 MB (25371412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb206f9ee26b21514bd7026ed97956b03f4175d0d2096d5f87471b82c21903e8`  
		Last Modified: Thu, 02 Mar 2023 02:21:28 GMT  
		Size: 6.3 MB (6310489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732358426922e371a7b325dcc12fdff47050775aafd32bcf8884ed1ad12f120`  
		Last Modified: Thu, 02 Mar 2023 02:21:27 GMT  
		Size: 3.0 MB (2976715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:bdbeb92cdb417dfefa084dc354ebb292bc3d80354b576d57918b117d81af1984
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
$ docker pull buildpack-deps@sha256:bc9e9bbd14e8a837e30009807718c317555b3585704c270ca0544ef30f322d48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81867757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd2ec34b02293026aee8b871a2ae86c29c797aa05892297f3a307185c275e28c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:22:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f64811d5f9e93d0cbbbaa74de2730a6dffbc3772747117377b98c979a5524e2`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 6.6 MB (6617385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed2ab5e0f15f7f6389f01ef48d5599f61173bb6c946ae3b9ece6d809e2708e5`  
		Last Modified: Thu, 02 Mar 2023 03:42:09 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f631ab33a755e153343352043423161c6232b94c3be5472cd780d6fb66fea8c`  
		Last Modified: Thu, 02 Mar 2023 03:42:24 GMT  
		Size: 45.5 MB (45513091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c945aafe1fad15d38e1188cc1844f06e144bab7335c3db05f2caa56f3ca460ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71282811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34ca2769a55b83b9eb31be2f63bed94363f1630e19ee1d39e592aad1851a18bc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:29:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:30:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:31:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6903cded2b3516e50f5bfdefd273774820e65f03bae3d1539678d6109df4e0b`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 5.7 MB (5679883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d900ce5096b9d98c4eacd5931071e9cf5fcc5869f19310d1c2fff7d3ed6806c5`  
		Last Modified: Thu, 02 Mar 2023 11:54:25 GMT  
		Size: 2.6 MB (2585896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672070d854b2efbf7e9d5720a994ded06c4e58c97060013aed2981fd327517c`  
		Last Modified: Thu, 02 Mar 2023 11:54:45 GMT  
		Size: 40.7 MB (40712962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:dc66d659df3c4d980bfd741e281c52d81cfab1027cdb9d0449f4d054806fdf77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75891803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4349a1a66435e325994ec9e6ec99ad5776cd7ea349f06b3e79c091f197bda134`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527f5e352ac533cdac8c50ce47e4185b349d1de4d8799f7529bb5d2524e4cb47`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 6.1 MB (6056649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea801ed12cc0807ef6ee95dca6e04d01bd2d6359efc54635d38d8a0516f55784`  
		Last Modified: Thu, 02 Mar 2023 02:35:43 GMT  
		Size: 2.8 MB (2789532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491410c5ebb78636109cdab447342140dc9a4facbc978baa236f142ea8e9d64c`  
		Last Modified: Thu, 02 Mar 2023 02:35:57 GMT  
		Size: 43.3 MB (43312084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f8c35b10a7e33961c8ce0a4bb0387e1bb73fa5a4677e5d36f56be2dfd6ea1b7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84425697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc4a367ff17e24b264b6562eee2668fcff45fcd418f80cd1e43989d1f259f5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:14:52 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:14:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:14:52 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:14:54 GMT
ADD file:765a9704b3961cee9523a98bfd0de0f97b6075431287fa7b8acd276145cb28c5 in / 
# Wed, 01 Mar 2023 03:14:54 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 14:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 14:26:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 14:27:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08886b8b414bd4d4f6a196c5ea7306887e23ed3e5d83e9bde2bfe0cc2af99325`  
		Last Modified: Thu, 02 Mar 2023 14:23:47 GMT  
		Size: 27.2 MB (27164837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16105d5c202ba8ceca010766befe9c0bae4ef06768c5649bbdebe34feeff56c0`  
		Last Modified: Thu, 02 Mar 2023 14:32:49 GMT  
		Size: 6.9 MB (6907843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606120c77dd0e4dc08e0829cd5fda3c301d68a11a8561df02368984d18c27e87`  
		Last Modified: Thu, 02 Mar 2023 14:32:48 GMT  
		Size: 3.3 MB (3255738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd34df470431bd99fe8348a0b7488317fd90179a50fc094b1bc09cfdfff0f651`  
		Last Modified: Thu, 02 Mar 2023 14:33:08 GMT  
		Size: 47.1 MB (47097279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:61f125647b51960eaaa1628df14c40ad5596f9a0c8ca31b75db9663c5ff8007f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94957007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ae7f36d16db90652afad8c37a9ea6b419e7b1ad7a94291093ec62e326ab0e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:15:24 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:15:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:15:24 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:15:27 GMT
ADD file:ca5a453351fddb6d7937e334f0331321829a5bebca3d726ef3dddad1f23b35c8 in / 
# Wed, 01 Mar 2023 03:15:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:12:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:12:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:27fbc2bd86045e72ba8d9901b237295e3094b37f456824337175e24a0f0afe98`  
		Last Modified: Thu, 02 Mar 2023 03:09:44 GMT  
		Size: 30.4 MB (30442026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fe4259cc8ab209d172cd6c47536773db4959cf18257a7d3d47b35257e3547`  
		Last Modified: Thu, 02 Mar 2023 03:54:32 GMT  
		Size: 7.0 MB (7036861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1d5bf7bb9bbef4a44b4363f1e0fa9ed98fe35bd78d986830c40d35c1641e5`  
		Last Modified: Thu, 02 Mar 2023 03:54:31 GMT  
		Size: 3.7 MB (3740555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68956dba4cc03b50dc85a017a1231e5796aa790462edfefff2e29d810938fac5`  
		Last Modified: Thu, 02 Mar 2023 03:54:58 GMT  
		Size: 53.7 MB (53737565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:54ddd0cd0622a5cd6cf1b28c3cb01a126d011f4d8e4c29ce1903761bfc7da58d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79698067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:206911be72a3fb03d2417b774c512074beef855e16b0cd2235cf6e178d1a1736`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:09 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:09 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:11 GMT
ADD file:49b5368b8703fe0aa128fe923b83da7ab2a30a7a1c0395682c905b9271e7f503 in / 
# Wed, 01 Mar 2023 03:18:11 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:02:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:03:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:03:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:306d1b363f89f239f5dc6314e0033094c067617b584ce004fd8db99402dab321`  
		Last Modified: Thu, 02 Mar 2023 02:21:31 GMT  
		Size: 25.4 MB (25371412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb206f9ee26b21514bd7026ed97956b03f4175d0d2096d5f87471b82c21903e8`  
		Last Modified: Thu, 02 Mar 2023 02:21:28 GMT  
		Size: 6.3 MB (6310489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732358426922e371a7b325dcc12fdff47050775aafd32bcf8884ed1ad12f120`  
		Last Modified: Thu, 02 Mar 2023 02:21:27 GMT  
		Size: 3.0 MB (2976715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f95174d0c3f8fa7400f2fe1baa0a15756c66695199991cb0126f6cd6586899`  
		Last Modified: Thu, 02 Mar 2023 02:21:45 GMT  
		Size: 45.0 MB (45039451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:9212e46cdbd63c438f51632df2951c70ccd898648a5ba90e82adf0fc03a6786c
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
$ docker pull buildpack-deps@sha256:26ae81f0d87b16da338ff5e9aaa7d9401fd2e69444797c89e96130cf4042b3c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321235599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:131ecc0b55080b3773d14fd12cb1b4d190b56336d637a82e5348fac7737471f0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:09:05 GMT
ADD file:77abd413b6799ae4f1f24f3bcc389dd12515fc4f732e81239d8c25475bc37fac in / 
# Wed, 01 Mar 2023 02:09:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:07:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:07:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:09:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:15:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65f9863fa983221d5b14b7a7e06e92e49a04fbced0e7af12bdafbdfcbc7a2deb`  
		Last Modified: Wed, 01 Mar 2023 02:16:56 GMT  
		Size: 49.2 MB (49245473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bcf13485e3ee0cadac8054427f8f6f3a08a8542574c273072b5a938746e826`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 8.4 MB (8414213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56e46e1c6aaa24d965fe76a54803920eb56ce4ab2092a6993067da3dd253f8`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 11.2 MB (11153696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e391ddfe06a9169f7cea164ba5cd6836dce99ef8ba4fc6f3cb9b0b3b79f63f`  
		Last Modified: Wed, 01 Mar 2023 14:33:39 GMT  
		Size: 62.9 MB (62920983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee394f8b54a43ab6674140143e254f3b40806874e56d6b59eca1035e6308e7b2`  
		Last Modified: Wed, 01 Mar 2023 14:35:40 GMT  
		Size: 189.5 MB (189501234 bytes)  
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
$ docker pull buildpack-deps@sha256:4a5f77cacf83c9f3c521015d89b61490036eab8481ac4d91e454f207fc666512
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
$ docker pull buildpack-deps@sha256:3a972cbb1aa6f0bf3842a0b059977a9d854135a4f95bfda1e4aac50feea75fb9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68813382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84bc6ab63e76ee0ebb37779fc3faacb153b7561e4475d7901826171b7a28e86`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:09:05 GMT
ADD file:77abd413b6799ae4f1f24f3bcc389dd12515fc4f732e81239d8c25475bc37fac in / 
# Wed, 01 Mar 2023 02:09:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:07:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:07:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:65f9863fa983221d5b14b7a7e06e92e49a04fbced0e7af12bdafbdfcbc7a2deb`  
		Last Modified: Wed, 01 Mar 2023 02:16:56 GMT  
		Size: 49.2 MB (49245473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bcf13485e3ee0cadac8054427f8f6f3a08a8542574c273072b5a938746e826`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 8.4 MB (8414213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56e46e1c6aaa24d965fe76a54803920eb56ce4ab2092a6993067da3dd253f8`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 11.2 MB (11153696 bytes)  
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
$ docker pull buildpack-deps@sha256:f9571020b467313c668d9cfbe8ebaa011f376e998adf9c90d32071626d0a07fa
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
$ docker pull buildpack-deps@sha256:7160ec99476b0a2468b9e7a2eb492fcc969b360833f5ccd8ef15e62729232c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131734365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2ccbb6f9934bc8cabfebd1553a774f9b2b06bb6a6162921a03743859ff60482`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:09:05 GMT
ADD file:77abd413b6799ae4f1f24f3bcc389dd12515fc4f732e81239d8c25475bc37fac in / 
# Wed, 01 Mar 2023 02:09:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:07:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:07:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:09:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65f9863fa983221d5b14b7a7e06e92e49a04fbced0e7af12bdafbdfcbc7a2deb`  
		Last Modified: Wed, 01 Mar 2023 02:16:56 GMT  
		Size: 49.2 MB (49245473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bcf13485e3ee0cadac8054427f8f6f3a08a8542574c273072b5a938746e826`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 8.4 MB (8414213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56e46e1c6aaa24d965fe76a54803920eb56ce4ab2092a6993067da3dd253f8`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 11.2 MB (11153696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e391ddfe06a9169f7cea164ba5cd6836dce99ef8ba4fc6f3cb9b0b3b79f63f`  
		Last Modified: Wed, 01 Mar 2023 14:33:39 GMT  
		Size: 62.9 MB (62920983 bytes)  
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
$ docker pull buildpack-deps@sha256:6f2703639d3d17f70288d4ba212d55e159b682a990c20fc2a6562b098f01a1e7
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
$ docker pull buildpack-deps@sha256:478bf93abb60da60c1188a076991f4dc9638195df95ba30b3377b06e7196d247
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301085570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23f7a118464453742cb6c2f3bd831c8193e5f35cc52d2f9c0f6b179d3309f2a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:23:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef506d17f8897590ad73117349f3d5a00bf1d49e9df07123ad9e5f62bdc1b9c`  
		Last Modified: Wed, 01 Mar 2023 14:35:52 GMT  
		Size: 4.9 MB (4922204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcd4f409b03d9914948b724b57835b18c4640aab6bc493cc80b3a874ffcc31`  
		Last Modified: Wed, 01 Mar 2023 14:35:54 GMT  
		Size: 10.7 MB (10662168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df25173951f289c64515ba71fb87f8b90d9d1951e7287d8fc1a6b5f12c5c567`  
		Last Modified: Wed, 01 Mar 2023 14:36:41 GMT  
		Size: 53.3 MB (53307045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaeb72ebe84fa1592a617e85865bdf44882a111fe77d3709017d0944f7666f9`  
		Last Modified: Wed, 01 Mar 2023 14:38:36 GMT  
		Size: 178.9 MB (178928978 bytes)  
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
$ docker pull buildpack-deps@sha256:1b0af9f90719ef87bfec766349df533e0b9051282d2cf845c6584fbc4412b70d
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
$ docker pull buildpack-deps@sha256:a6f2a19a68aa123aad96add6fc1b3303e711608e3f67ef461202424893602731
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68849547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335938bead68388bf68af487c365a97a41376b45ccc2f2d17893aab6ba39a233`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef506d17f8897590ad73117349f3d5a00bf1d49e9df07123ad9e5f62bdc1b9c`  
		Last Modified: Wed, 01 Mar 2023 14:35:52 GMT  
		Size: 4.9 MB (4922204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcd4f409b03d9914948b724b57835b18c4640aab6bc493cc80b3a874ffcc31`  
		Last Modified: Wed, 01 Mar 2023 14:35:54 GMT  
		Size: 10.7 MB (10662168 bytes)  
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
$ docker pull buildpack-deps@sha256:ca9b375648e50b4c26007c99cb7dca68626fc42863c01841d7232f41e166130e
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
$ docker pull buildpack-deps@sha256:a342b7a73b4c0cabe77fc12a63c608a8114dd750b757d720688dd114ddca8f98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122156592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f29263ab5584d0b1394d255686d09c9b9acec2b70d35751fc7e2b81f63e3202`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef506d17f8897590ad73117349f3d5a00bf1d49e9df07123ad9e5f62bdc1b9c`  
		Last Modified: Wed, 01 Mar 2023 14:35:52 GMT  
		Size: 4.9 MB (4922204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcd4f409b03d9914948b724b57835b18c4640aab6bc493cc80b3a874ffcc31`  
		Last Modified: Wed, 01 Mar 2023 14:35:54 GMT  
		Size: 10.7 MB (10662168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df25173951f289c64515ba71fb87f8b90d9d1951e7287d8fc1a6b5f12c5c567`  
		Last Modified: Wed, 01 Mar 2023 14:36:41 GMT  
		Size: 53.3 MB (53307045 bytes)  
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
$ docker pull buildpack-deps@sha256:1b0af9f90719ef87bfec766349df533e0b9051282d2cf845c6584fbc4412b70d
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
$ docker pull buildpack-deps@sha256:a6f2a19a68aa123aad96add6fc1b3303e711608e3f67ef461202424893602731
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68849547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335938bead68388bf68af487c365a97a41376b45ccc2f2d17893aab6ba39a233`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef506d17f8897590ad73117349f3d5a00bf1d49e9df07123ad9e5f62bdc1b9c`  
		Last Modified: Wed, 01 Mar 2023 14:35:52 GMT  
		Size: 4.9 MB (4922204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcd4f409b03d9914948b724b57835b18c4640aab6bc493cc80b3a874ffcc31`  
		Last Modified: Wed, 01 Mar 2023 14:35:54 GMT  
		Size: 10.7 MB (10662168 bytes)  
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
$ docker pull buildpack-deps@sha256:a935aae0569e82652a65d88ac7a1996d83bad092a346da4999eb73d34cb0f23d
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
$ docker pull buildpack-deps@sha256:595b2e444543064db2180320b4a521621630b3086acc881d4e1a7a5c6bfede96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245779275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee045173ae74b7b44140d6bc57447da87c62d5054c11aa5a88d9f2a06155c09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:25:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:25:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b7d3f3b016944c7eeeee37880c5c274cfc06cccd337b282c382d036852f921`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 7.7 MB (7739318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7712ac161458ffa37dfe485734ac5bfbc45c78512bfc1bca4479eb5b6f2aa64e`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 3.6 MB (3627267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf762b78d7137d4905242d9e25291e630f6926d0bd5cada5e7072817f61748`  
		Last Modified: Thu, 02 Mar 2023 03:43:20 GMT  
		Size: 60.7 MB (60740440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc356f49ea441894a0ae1bc758258a040d5375f2bd1e7ff2185f00e77198185`  
		Last Modified: Thu, 02 Mar 2023 03:43:48 GMT  
		Size: 145.1 MB (145094248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6d158f6d184a97d1dfef9b4edb82d7dd489d520b9252589ef7c13283a79361bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211781714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3a5fd39b47359ac607eded26d7b0108b92f150304a4e5dbaceaa5f4285a3b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:34:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:35:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:38:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cdafdb2f80a4c0460861f9220f045255f35eca62f6c065d24d65d3950a8c93`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 6.7 MB (6726138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eec04ad18d2253a95f5fcfcdd36aa4f470211a830af52b3e5856b8a8fd0ca7`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 3.1 MB (3104511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b743206528cfc301cf72ca17581201c8ca2e513bfa66b8795a8c9f58530f979`  
		Last Modified: Thu, 02 Mar 2023 11:55:43 GMT  
		Size: 55.4 MB (55433524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9d1daa72ce9f63ee0d3b940a6b63549facf2bbdf6c0fb8315a6105e99c36f3`  
		Last Modified: Thu, 02 Mar 2023 11:56:10 GMT  
		Size: 121.9 MB (121931093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:07f23c18b827305b81c5f727176b832ce798bd5da415fc7d073faf506b3ed0a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (236000423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408e406aadc361d174f2857e983a863b7ab799b75aa0fcb77e9c346923a498a0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:15:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:17:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:20:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eb13d431eb1ef5f774a4d14dafd7895d0061c2b77e3d613eed550a0245407e`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 7.6 MB (7601140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffe806a7e8e21e8288df2fed964181acc22875517099563c835fab72df366a5`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 3.6 MB (3616335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b02b41f50d1324e472bd6f2983f88f54704cdbd4af160efbc6e42e9a30c202`  
		Last Modified: Thu, 02 Mar 2023 02:36:46 GMT  
		Size: 60.8 MB (60817897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751575f78c3732573ab9aece852eadcb0d9a48e7b0eced95b9d7890ccc8c29d`  
		Last Modified: Thu, 02 Mar 2023 02:37:09 GMT  
		Size: 136.8 MB (136770530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1b5295e484925905b7e3b18f0e115ecfba46ec1673f7d2cc02016c9537015642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269626587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f809b1eaa3bb5cdb30f6a1553650cc08b4fe3dd4f58aa9ed33d923da8f63a4ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:25:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:25:25 GMT
ADD file:8ec53343ee3a54689d663a250c785fbf7b8ac0c74de561582d2e54878e2d73b5 in / 
# Wed, 01 Mar 2023 05:25:25 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:27:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ecbbabc4a8d11d32aa94bd1d645cba73ad91f59060b872eaf684de51310281b`  
		Last Modified: Thu, 02 Mar 2023 03:56:04 GMT  
		Size: 33.3 MB (33300379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ae83340e2c9ec8730a49a2c9aea2b21377b8a13b0c84c4b76cda0b29f82b4`  
		Last Modified: Thu, 02 Mar 2023 03:55:58 GMT  
		Size: 8.7 MB (8692716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b6ac479d5a474eedb2bd6b11d64e8b631ccce4beb6e06c84f00b6a2401fe5`  
		Last Modified: Thu, 02 Mar 2023 03:55:56 GMT  
		Size: 4.5 MB (4486858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7463e49960ae08f87f90376abcd19653c97a0752f8ccec05d042697e537f29f7`  
		Last Modified: Thu, 02 Mar 2023 03:56:33 GMT  
		Size: 69.6 MB (69553064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8eb87abfba2b370ecf10fd2cad3a672ca67bb51c2986a4b91ba814d27ada36`  
		Last Modified: Thu, 02 Mar 2023 03:57:23 GMT  
		Size: 153.6 MB (153593570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4c565e2587257fbb8d803086ed497597cb90115d36588b7a1a7428fa1ae02143
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226385332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e7e156764c073cc753dc89b15d097126091bb9ed5040bbadb7c371bd2f8a8cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:17 GMT
ADD file:859bfd657725af24f17d4e3c5b3b583b4b29d55f5f7f2f44fbdd6fbc83c6952d in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:06:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:06:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:07:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:09:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6ac74ab42247b9491b6986614b9868ce755dc1c84611543400690873aa73416`  
		Last Modified: Thu, 02 Mar 2023 02:22:20 GMT  
		Size: 27.0 MB (27016384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc17b063ad8d756ac72af0baf660b2a167389eae787139cf93b4069d0c6b99e6`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 7.4 MB (7379145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed830f413f3cae573689a1c936a49883bbb291424264e382dcc1da4590763d7`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 3.5 MB (3542220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb456cc7a06a826274d0489333373e503b4847ae4f5e22a50abf74ea87444a`  
		Last Modified: Thu, 02 Mar 2023 02:22:37 GMT  
		Size: 60.0 MB (60020217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31af2011810d962a8ab70a00f570ad12418f8a477135869fb1a0776eb1a149ac`  
		Last Modified: Thu, 02 Mar 2023 02:23:01 GMT  
		Size: 128.4 MB (128427366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:984dc5c11cde1a5d03a678d8aac00aca49775dca4ea7d9944789e27d289c64cf
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
$ docker pull buildpack-deps@sha256:c4824dc0e30a785dd034a6ba5ded770e6f50c8bd8d9075e44a4bd853b3877215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39944587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5caab55bf6d1a9670b35b8708c155221d41b0494671f44dce30a46726e341d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:25:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:25:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b7d3f3b016944c7eeeee37880c5c274cfc06cccd337b282c382d036852f921`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 7.7 MB (7739318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7712ac161458ffa37dfe485734ac5bfbc45c78512bfc1bca4479eb5b6f2aa64e`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 3.6 MB (3627267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c87787b92e2117d7b7a33eb5dabe78904f745298e10d43755236acd5b8914118
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34417097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4ec684782764d6ba26a275ce1f732fac70f18b5de92501502f1b2a42e279f82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:34:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cdafdb2f80a4c0460861f9220f045255f35eca62f6c065d24d65d3950a8c93`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 6.7 MB (6726138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eec04ad18d2253a95f5fcfcdd36aa4f470211a830af52b3e5856b8a8fd0ca7`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 3.1 MB (3104511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c595692763bde705e8e32ea772ba5e033189fc44826e95715cdf8f8a3cb7d5bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38411996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1be97e4a549deb271895519fd7cfebdbff011498ae4679449cea44653528df5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:15:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eb13d431eb1ef5f774a4d14dafd7895d0061c2b77e3d613eed550a0245407e`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 7.6 MB (7601140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffe806a7e8e21e8288df2fed964181acc22875517099563c835fab72df366a5`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 3.6 MB (3616335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4ababf7fb20ae1801b2a6e85ceb554ad08e24c87cc993d0ba8fba7c9182f3219
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46479953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e64276e03515e980c104a27b52c96227de1789f094240a143f53258907492dd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:25:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:25:25 GMT
ADD file:8ec53343ee3a54689d663a250c785fbf7b8ac0c74de561582d2e54878e2d73b5 in / 
# Wed, 01 Mar 2023 05:25:25 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4ecbbabc4a8d11d32aa94bd1d645cba73ad91f59060b872eaf684de51310281b`  
		Last Modified: Thu, 02 Mar 2023 03:56:04 GMT  
		Size: 33.3 MB (33300379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ae83340e2c9ec8730a49a2c9aea2b21377b8a13b0c84c4b76cda0b29f82b4`  
		Last Modified: Thu, 02 Mar 2023 03:55:58 GMT  
		Size: 8.7 MB (8692716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b6ac479d5a474eedb2bd6b11d64e8b631ccce4beb6e06c84f00b6a2401fe5`  
		Last Modified: Thu, 02 Mar 2023 03:55:56 GMT  
		Size: 4.5 MB (4486858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0343330c438e6f2403980ca7d2e3b3561187c0cd05366b52540e2544be7d7a0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37937749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a223df0c64acbbf14d7148eac1e5a3566119146af7d66bcb1bcc702412b9abc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:17 GMT
ADD file:859bfd657725af24f17d4e3c5b3b583b4b29d55f5f7f2f44fbdd6fbc83c6952d in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:06:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:06:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d6ac74ab42247b9491b6986614b9868ce755dc1c84611543400690873aa73416`  
		Last Modified: Thu, 02 Mar 2023 02:22:20 GMT  
		Size: 27.0 MB (27016384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc17b063ad8d756ac72af0baf660b2a167389eae787139cf93b4069d0c6b99e6`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 7.4 MB (7379145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed830f413f3cae573689a1c936a49883bbb291424264e382dcc1da4590763d7`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 3.5 MB (3542220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:79af9774ce5575c78d3cb87f01db10be2d14c83c432d98d38cd9c46d089bcd00
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
$ docker pull buildpack-deps@sha256:35d4677d74ee38e81499ccfe32c1d9234fc0c0ade83ea095f3c36d9830c4ed18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100685027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cbe0a30857b0e0810b34b6fc2a6137c37e3261e8101890646c44da76ec86db6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:25:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:25:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b7d3f3b016944c7eeeee37880c5c274cfc06cccd337b282c382d036852f921`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 7.7 MB (7739318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7712ac161458ffa37dfe485734ac5bfbc45c78512bfc1bca4479eb5b6f2aa64e`  
		Last Modified: Thu, 02 Mar 2023 03:43:00 GMT  
		Size: 3.6 MB (3627267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf762b78d7137d4905242d9e25291e630f6926d0bd5cada5e7072817f61748`  
		Last Modified: Thu, 02 Mar 2023 03:43:20 GMT  
		Size: 60.7 MB (60740440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:38ef378fe4ad8b7f3d9489034e7f61b5347c531c2b986b4d889b4608ed124cde
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89850621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417c12900a3dd87706ff12eb9e4370b09bc22988769f3df9028cfb36346b496c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:34:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:34:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:35:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cdafdb2f80a4c0460861f9220f045255f35eca62f6c065d24d65d3950a8c93`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 6.7 MB (6726138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eec04ad18d2253a95f5fcfcdd36aa4f470211a830af52b3e5856b8a8fd0ca7`  
		Last Modified: Thu, 02 Mar 2023 11:55:24 GMT  
		Size: 3.1 MB (3104511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b743206528cfc301cf72ca17581201c8ca2e513bfa66b8795a8c9f58530f979`  
		Last Modified: Thu, 02 Mar 2023 11:55:43 GMT  
		Size: 55.4 MB (55433524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2d9ba385e19d2fe67be14f111c916e1b28326e57d73b9ce143a20a1716f4fc24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99229893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e480fce56055355bcd1dbcd9b0383ab3052ed0a7f921bd2eee5f16ad138b8f71`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:15:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:17:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eb13d431eb1ef5f774a4d14dafd7895d0061c2b77e3d613eed550a0245407e`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 7.6 MB (7601140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffe806a7e8e21e8288df2fed964181acc22875517099563c835fab72df366a5`  
		Last Modified: Thu, 02 Mar 2023 02:36:28 GMT  
		Size: 3.6 MB (3616335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b02b41f50d1324e472bd6f2983f88f54704cdbd4af160efbc6e42e9a30c202`  
		Last Modified: Thu, 02 Mar 2023 02:36:46 GMT  
		Size: 60.8 MB (60817897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:097e0ff2bf42901bcb9a769ba497f752b671df6f9f096e69d646c0e1fed9169d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116033017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e8553668a9ab292bc90a0129e3925d4dc4a30a334691b732744e17a6456965d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:25:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:25:25 GMT
ADD file:8ec53343ee3a54689d663a250c785fbf7b8ac0c74de561582d2e54878e2d73b5 in / 
# Wed, 01 Mar 2023 05:25:25 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ecbbabc4a8d11d32aa94bd1d645cba73ad91f59060b872eaf684de51310281b`  
		Last Modified: Thu, 02 Mar 2023 03:56:04 GMT  
		Size: 33.3 MB (33300379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ae83340e2c9ec8730a49a2c9aea2b21377b8a13b0c84c4b76cda0b29f82b4`  
		Last Modified: Thu, 02 Mar 2023 03:55:58 GMT  
		Size: 8.7 MB (8692716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b6ac479d5a474eedb2bd6b11d64e8b631ccce4beb6e06c84f00b6a2401fe5`  
		Last Modified: Thu, 02 Mar 2023 03:55:56 GMT  
		Size: 4.5 MB (4486858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7463e49960ae08f87f90376abcd19653c97a0752f8ccec05d042697e537f29f7`  
		Last Modified: Thu, 02 Mar 2023 03:56:33 GMT  
		Size: 69.6 MB (69553064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:38bd61dec26f3d8c377aa42023d084418de54f0f11ddf9eddeaa945b46b2f5bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (97957966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be039469f9caf4b3cf6f0c5c7d8b6e28cf93f6dde713bd55edc8b23513950c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:15 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:17 GMT
ADD file:859bfd657725af24f17d4e3c5b3b583b4b29d55f5f7f2f44fbdd6fbc83c6952d in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:06:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:06:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:07:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6ac74ab42247b9491b6986614b9868ce755dc1c84611543400690873aa73416`  
		Last Modified: Thu, 02 Mar 2023 02:22:20 GMT  
		Size: 27.0 MB (27016384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc17b063ad8d756ac72af0baf660b2a167389eae787139cf93b4069d0c6b99e6`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 7.4 MB (7379145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed830f413f3cae573689a1c936a49883bbb291424264e382dcc1da4590763d7`  
		Last Modified: Thu, 02 Mar 2023 02:22:17 GMT  
		Size: 3.5 MB (3542220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb456cc7a06a826274d0489333373e503b4847ae4f5e22a50abf74ea87444a`  
		Last Modified: Thu, 02 Mar 2023 02:22:37 GMT  
		Size: 60.0 MB (60020217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy`

```console
$ docker pull buildpack-deps@sha256:9a5858bbf22b934014c6d0cacb9e2e8281868a5315445da65574541a919dba32
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
$ docker pull buildpack-deps@sha256:c6097317ab952d1afb8c1199bdf70c7d1bcacdc64a3319ca0228eef74c9532c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (250025364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d5252a78e69dbf7e7b1785eb3482824865a2d45e2be1a51928e796fa19efc58`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:33:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b17938a1a752564000a3a0aeed04eafc6958f178a7fcc09094daa31ec80767`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.8 MB (3788644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51ade0caaff8e59d92682e80d534ad83b8bc2d760bbe60eb56dc0363c60b4d6`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.6 MB (3561585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b8264f0fdf1f57cc3ac8b5b09faac810a388350812478b3dc2ab19727db68`  
		Last Modified: Thu, 02 Mar 2023 03:44:15 GMT  
		Size: 39.4 MB (39353140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985addd9038004b289a1cd2d449d95f1a7d1292f38b3ba6a8627732be72d20db`  
		Last Modified: Thu, 02 Mar 2023 03:44:45 GMT  
		Size: 172.9 MB (172891993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c315b1fd3deb39e15675ded20c0eff07feefa72c495f2c400ce5da57a7b3b5ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216668610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08db3cf9b75c32f87a7066a58928c9b1d8312e8d1807a3ded7a02ec539aab5af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:45:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:45:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:45:58 GMT
ADD file:d8e0c2340f91ec5973c8459c1a917be69f6530fe7f88da02eb5b4dd562c31730 in / 
# Wed, 01 Mar 2023 04:45:59 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:38:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:38:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:39:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:42:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5909c79a6169dfa05f978dbe7f8dfeadbb92a0d4a3a4d792314b3afe271dd793`  
		Last Modified: Wed, 01 Mar 2023 08:59:31 GMT  
		Size: 27.0 MB (27024489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e834b31ec46c994de883b1d8fd540229984065b7116dc8dab706aa6969bd5bff`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.5 MB (3539420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2617d031bbc0245044288b2afe503e376a8d9b8ded256246d64c969d12c85e7c`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.7 MB (3713780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffb58fb6ee1096d3a9785f5fd877bff68fdae04f23374b1f8753549f2dfa0e8`  
		Last Modified: Thu, 02 Mar 2023 11:56:38 GMT  
		Size: 41.9 MB (41907681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7871bf146ef1fecfbd6d2edf4122cf98e93d0007dc7f6c20f0dc4e032cbb6c`  
		Last Modified: Thu, 02 Mar 2023 11:57:06 GMT  
		Size: 140.5 MB (140483240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8c0e084a35a14526bcdbd462f399caa72f94e93c1e45d2dd6826c6c30b6686f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241331257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d42d4ee258d3bbea3b7c73ea09047bd5770942302d55947c411142e80fa2b03`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:21:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:22:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:25:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ecb6dff9238e75e6877b0624e8c0054bcb5d51c97f5f178a8a699de3e06572`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.8 MB (3760955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb16d0d18eaee62625a39492bf99dabbc71b2e3d6278c10a2080894ebe562b`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.5 MB (3536614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088d8f170fef46d01bbb6cd7b616c91b38f4fcad2ab1b42e1d93e9d86a7febe9`  
		Last Modified: Thu, 02 Mar 2023 02:37:34 GMT  
		Size: 39.2 MB (39242827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3373b535e41981b6538ebc53657679e880b4981c2c0626a29e4b14fb40459ae`  
		Last Modified: Thu, 02 Mar 2023 02:38:00 GMT  
		Size: 166.4 MB (166402939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:45e74d13a22728db4b4ec36070d857f369a226970a67390997b958f21ea1f6ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271848633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4ed251594f077f2874d4b7f9391ab978d7cbcf5a0d69ab768031bec032b3c1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:09:57 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:09:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:01 GMT
ADD file:e4d45fbda8cf3ca1613a11d2b929670e0e12b43c66818636afa9ebcbf6b48b59 in / 
# Wed, 01 Mar 2023 05:10:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:28:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:36:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:062a5dd6f1a8faa2ffa6ca3db2cdb7e930e5f49f52c8647b30709399b759b1cb`  
		Last Modified: Thu, 02 Mar 2023 03:35:30 GMT  
		Size: 35.7 MB (35711589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387fa66f2465a45a4bf52efe7a70d02b4b563ea79f4a05b59a132253b6fd192c`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.3 MB (4262192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3313c961eddc996b17782dfb540ee65ee6801254d9ee09d82691b5a9f66f7431`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.2 MB (4234903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ba7916137f91162c1002b749a8a79118a1565f3a770f8d4d9415bd64e78b8b`  
		Last Modified: Thu, 02 Mar 2023 03:58:05 GMT  
		Size: 43.8 MB (43768446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbee4b59613644150cb1c5f30f7909c912cae5d9a2bbfd41fc3e4fe91a0286a`  
		Last Modified: Thu, 02 Mar 2023 03:59:00 GMT  
		Size: 183.9 MB (183871503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:12b2add676326f2ab7c9553ca93e55ceb7640c89c52e5bcdc60e9484b4b9c6e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223696347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399d1ff49dcb964c6fe2e7466d4807493aa3b92c5a22902cec1a41816285b263`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:10:39 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:10:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:41 GMT
ADD file:db14dc9a9d330115a6699be3c4a344f5fe366ec17e7d3649c4ecb2711605e52b in / 
# Wed, 01 Mar 2023 05:10:41 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:09:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:10:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:10:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:12:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:905ef75a23211c85ea45c3aa7f7e77bc95a94ff8c250e03412ef8c50b5fb9f49`  
		Last Modified: Thu, 02 Mar 2023 02:23:13 GMT  
		Size: 28.6 MB (28647596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f21104d1d70c25a181a183058f1061378e9d8c535e59e4c939c4231cbc970c`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.8 MB (3792871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8e321da5315972e394da4ba438abe2fd4085876b6ea43578a0324a68aeb100`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.5 MB (3472941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67223d18224c8c78226be471d16442159e0754a6cda26186d8d1c072820e289`  
		Last Modified: Thu, 02 Mar 2023 02:23:25 GMT  
		Size: 39.3 MB (39283485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21d051fa1c50a914eaa8e87cb3231ff4fc1430fd743c0041c286058b0aede2`  
		Last Modified: Thu, 02 Mar 2023 02:23:51 GMT  
		Size: 148.5 MB (148499454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:46d4df86174ba0e17a6931431f2f0caecdae8ec50baf93c22de21a4e985cd39a
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
$ docker pull buildpack-deps@sha256:7c4181266db1c499d5050004a6bd81130b4c69a731b3b0f3132946a33813175e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37780231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c24181609005d131d0d93aad7eda4e076a45e610fd9e7e734349f901c88fb89e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b17938a1a752564000a3a0aeed04eafc6958f178a7fcc09094daa31ec80767`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.8 MB (3788644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51ade0caaff8e59d92682e80d534ad83b8bc2d760bbe60eb56dc0363c60b4d6`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.6 MB (3561585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:79d98c78e452391dc6f0dc841826fb7db37e2210bc46c84b842aa5170dd1cbda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34277689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f47a341c042acdfabe711f0519c94b2421c00a3ac0cf4f275853ad071a7a7b1c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:45:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:45:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:45:58 GMT
ADD file:d8e0c2340f91ec5973c8459c1a917be69f6530fe7f88da02eb5b4dd562c31730 in / 
# Wed, 01 Mar 2023 04:45:59 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:38:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:38:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5909c79a6169dfa05f978dbe7f8dfeadbb92a0d4a3a4d792314b3afe271dd793`  
		Last Modified: Wed, 01 Mar 2023 08:59:31 GMT  
		Size: 27.0 MB (27024489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e834b31ec46c994de883b1d8fd540229984065b7116dc8dab706aa6969bd5bff`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.5 MB (3539420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2617d031bbc0245044288b2afe503e376a8d9b8ded256246d64c969d12c85e7c`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.7 MB (3713780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:38af74bfc05f15a56d777c62d1184b40ec93ce4d4c5d7d2fe990ed9b898cfb5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35685491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6749e86ca4413cec2f058d6100e25f4dc008d155670d61e528de5f43d1dcd5e0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:21:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ecb6dff9238e75e6877b0624e8c0054bcb5d51c97f5f178a8a699de3e06572`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.8 MB (3760955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb16d0d18eaee62625a39492bf99dabbc71b2e3d6278c10a2080894ebe562b`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.5 MB (3536614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ec09f10603891c397a34727e768f3669e5f99ddd77f3e82242399bb18f778d89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44208684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c1fea401154387820e29c3d48abd9cd1a45519ae1df49fffce659c7057defe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:09:57 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:09:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:01 GMT
ADD file:e4d45fbda8cf3ca1613a11d2b929670e0e12b43c66818636afa9ebcbf6b48b59 in / 
# Wed, 01 Mar 2023 05:10:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:28:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:062a5dd6f1a8faa2ffa6ca3db2cdb7e930e5f49f52c8647b30709399b759b1cb`  
		Last Modified: Thu, 02 Mar 2023 03:35:30 GMT  
		Size: 35.7 MB (35711589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387fa66f2465a45a4bf52efe7a70d02b4b563ea79f4a05b59a132253b6fd192c`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.3 MB (4262192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3313c961eddc996b17782dfb540ee65ee6801254d9ee09d82691b5a9f66f7431`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.2 MB (4234903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d3dbf3f2437dac5abae4e64090c5389d96c98ea170f5cdca2e3fef799054f757
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35913408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad46ce92dd1a41929e464c3d4f34611b73f1494aef4327fce99ab635e5976d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:10:39 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:10:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:41 GMT
ADD file:db14dc9a9d330115a6699be3c4a344f5fe366ec17e7d3649c4ecb2711605e52b in / 
# Wed, 01 Mar 2023 05:10:41 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:09:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:10:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:905ef75a23211c85ea45c3aa7f7e77bc95a94ff8c250e03412ef8c50b5fb9f49`  
		Last Modified: Thu, 02 Mar 2023 02:23:13 GMT  
		Size: 28.6 MB (28647596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f21104d1d70c25a181a183058f1061378e9d8c535e59e4c939c4231cbc970c`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.8 MB (3792871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8e321da5315972e394da4ba438abe2fd4085876b6ea43578a0324a68aeb100`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.5 MB (3472941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:309fa57d4ff4c368763213a7e066d1b87cc15fe0949c124f3a7ed8430c4bcd1c
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
$ docker pull buildpack-deps@sha256:3483a701ce591a55e4782a4fb689bd1e0385394d2485d7785a88b9887508be2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77133371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bfb7a7ac339b586fd2b8395f35c7994ba14c08eaf2062e13ef0dfa8eeb378b5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b17938a1a752564000a3a0aeed04eafc6958f178a7fcc09094daa31ec80767`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.8 MB (3788644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51ade0caaff8e59d92682e80d534ad83b8bc2d760bbe60eb56dc0363c60b4d6`  
		Last Modified: Thu, 02 Mar 2023 03:43:57 GMT  
		Size: 3.6 MB (3561585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b8264f0fdf1f57cc3ac8b5b09faac810a388350812478b3dc2ab19727db68`  
		Last Modified: Thu, 02 Mar 2023 03:44:15 GMT  
		Size: 39.4 MB (39353140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:62d7932743dea29053da8801145b2aeae07aa06c8644a0b1ae37169877a25931
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76185370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3983d506885a6b142e0303d98015fc347be1fd11dcad071209eac93543f226a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:45:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:45:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:45:58 GMT
ADD file:d8e0c2340f91ec5973c8459c1a917be69f6530fe7f88da02eb5b4dd562c31730 in / 
# Wed, 01 Mar 2023 04:45:59 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:38:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:38:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:39:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5909c79a6169dfa05f978dbe7f8dfeadbb92a0d4a3a4d792314b3afe271dd793`  
		Last Modified: Wed, 01 Mar 2023 08:59:31 GMT  
		Size: 27.0 MB (27024489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e834b31ec46c994de883b1d8fd540229984065b7116dc8dab706aa6969bd5bff`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.5 MB (3539420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2617d031bbc0245044288b2afe503e376a8d9b8ded256246d64c969d12c85e7c`  
		Last Modified: Thu, 02 Mar 2023 11:56:21 GMT  
		Size: 3.7 MB (3713780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffb58fb6ee1096d3a9785f5fd877bff68fdae04f23374b1f8753549f2dfa0e8`  
		Last Modified: Thu, 02 Mar 2023 11:56:38 GMT  
		Size: 41.9 MB (41907681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c3524bdfa214bd2069033b2a4d4338b5d9d4d33b164980d265a64999c9ca18df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74928318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82fbeb6451e8bf8f6ebe5aaf0501691761c3562fff522fc1c688f5c76d97492`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:21:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:22:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ecb6dff9238e75e6877b0624e8c0054bcb5d51c97f5f178a8a699de3e06572`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.8 MB (3760955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb16d0d18eaee62625a39492bf99dabbc71b2e3d6278c10a2080894ebe562b`  
		Last Modified: Thu, 02 Mar 2023 02:37:18 GMT  
		Size: 3.5 MB (3536614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088d8f170fef46d01bbb6cd7b616c91b38f4fcad2ab1b42e1d93e9d86a7febe9`  
		Last Modified: Thu, 02 Mar 2023 02:37:34 GMT  
		Size: 39.2 MB (39242827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:de685636ac1d95144c9e8a8c6e6a46b21dc77204fffc1f53622024051a964e0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87977130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab13bb48e1dc22e897444373d0821d94c43a5d25afb1701dbaf505970e8637e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:09:57 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:09:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:01 GMT
ADD file:e4d45fbda8cf3ca1613a11d2b929670e0e12b43c66818636afa9ebcbf6b48b59 in / 
# Wed, 01 Mar 2023 05:10:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:28:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:062a5dd6f1a8faa2ffa6ca3db2cdb7e930e5f49f52c8647b30709399b759b1cb`  
		Last Modified: Thu, 02 Mar 2023 03:35:30 GMT  
		Size: 35.7 MB (35711589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387fa66f2465a45a4bf52efe7a70d02b4b563ea79f4a05b59a132253b6fd192c`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.3 MB (4262192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3313c961eddc996b17782dfb540ee65ee6801254d9ee09d82691b5a9f66f7431`  
		Last Modified: Thu, 02 Mar 2023 03:57:35 GMT  
		Size: 4.2 MB (4234903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ba7916137f91162c1002b749a8a79118a1565f3a770f8d4d9415bd64e78b8b`  
		Last Modified: Thu, 02 Mar 2023 03:58:05 GMT  
		Size: 43.8 MB (43768446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b9176765891a17832f7daca48b461c8953219e5f2188240da03d66f1191bcfdf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75196893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b4d8150feeab5b80dcb010823460e54fcfd72b565b3e8820923c650ef60d391`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:10:39 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:10:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:41 GMT
ADD file:db14dc9a9d330115a6699be3c4a344f5fe366ec17e7d3649c4ecb2711605e52b in / 
# Wed, 01 Mar 2023 05:10:41 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:09:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:10:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:10:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:905ef75a23211c85ea45c3aa7f7e77bc95a94ff8c250e03412ef8c50b5fb9f49`  
		Last Modified: Thu, 02 Mar 2023 02:23:13 GMT  
		Size: 28.6 MB (28647596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f21104d1d70c25a181a183058f1061378e9d8c535e59e4c939c4231cbc970c`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.8 MB (3792871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8e321da5315972e394da4ba438abe2fd4085876b6ea43578a0324a68aeb100`  
		Last Modified: Thu, 02 Mar 2023 02:23:09 GMT  
		Size: 3.5 MB (3472941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67223d18224c8c78226be471d16442159e0754a6cda26186d8d1c072820e289`  
		Last Modified: Thu, 02 Mar 2023 02:23:25 GMT  
		Size: 39.3 MB (39283485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:3de898d7deb52f63ea659a9406465b2011f5e5d9c42bdbd02c3986a636fdfc85
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
$ docker pull buildpack-deps@sha256:495e9e8ec9026b48115b0d3f8d00ec6f5bf85d394a2b182f021ac0e53b031832
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.7 MB (258747951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba0b089f69567a45c75ccfcde23ba31fa81898eb602bd9a598942df1988a767`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:43:07 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:43:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:43:09 GMT
ADD file:18f562911635a03a9bf9e5fc22863fc2a78a64f7d35c7daa59f2d609b7ca055a in / 
# Mon, 20 Feb 2023 11:43:10 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:33:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:34:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:34:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a10df61efde6b7f0cf3fbf848a5bed1c943a54e13566f30ef6a0cc6f259a2f33`  
		Last Modified: Thu, 02 Mar 2023 03:44:58 GMT  
		Size: 27.5 MB (27479398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9f9f71b0155b4b832dcb9bfbf542389507996cd93239b78300535c9421961`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 6.8 MB (6770219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710e0dcd6284a414a9f90e76d5555002980ba77c51b01d6a812e56d2c2d94d2e`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 3.6 MB (3635116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c20cf6be4d508b2c166988b50c5ae18cead28e74cf5a620d56202faabfe64a`  
		Last Modified: Thu, 02 Mar 2023 03:45:14 GMT  
		Size: 39.7 MB (39740010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050e88152487e2ad34afbd56fbc9c0f572f844c942044c6340d15392d91a0952`  
		Last Modified: Thu, 02 Mar 2023 03:45:47 GMT  
		Size: 181.1 MB (181123208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f636fdcf52a029e7d45340728ba354563227e08d26f89e19c7ab7d6b0021388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221869394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26553e21166cc99d3951d5842347777794fc253327acdb39b126f177bdd39e0f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 12:11:32 GMT
ARG RELEASE
# Mon, 20 Feb 2023 12:11:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 12:11:42 GMT
ADD file:f77393d0d614b99f7ca8de09afc58a2e98d9d25c84c5ff69b50e94e7f191f7bb in / 
# Mon, 20 Feb 2023 12:11:43 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:43:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:43:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:44:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:47:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e07337a9bc2a6220f565efbaf0abbba7718bb8478f0af5b255df655e98cacc06`  
		Last Modified: Thu, 02 Mar 2023 11:57:20 GMT  
		Size: 25.9 MB (25893079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84854174ca4e4c0ad5221cd0bface3a62279cc1659c26e61319a54c79f28a32`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 5.9 MB (5941095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcf439bd51bffc866ae5a81a2764cc54c7f76949d34e14d2ef5666243a5c9e6`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 3.8 MB (3801108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f989583c8ba595c2fb646ad093cc454bdb75e54ffe38ddcab4b7dc16bdb7e049`  
		Last Modified: Thu, 02 Mar 2023 11:57:37 GMT  
		Size: 42.6 MB (42607751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295db91297f7f8abb0622ff7a5f4c016e6ac8ee683a7b68eb6cd5b3acc813cfe`  
		Last Modified: Thu, 02 Mar 2023 11:58:07 GMT  
		Size: 143.6 MB (143626361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c58b5202654dafd061c9cea886f8415d96e7944c8edcf5c8080c0a0891595872
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.7 MB (246708749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d03b850f658d961584bce6f1511e1c4d58e7334d4dba0ab3ab1ad8d1f9bce2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:58:05 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:58:13 GMT
ADD file:7e756337f8554849df664b30203a26f6c39dc303e277292de31fd784b9ff471b in / 
# Mon, 20 Feb 2023 11:58:13 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:26:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:27:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:30:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30762c7e5d854e6efb956328165eb8c43cbcf6c0be6766a45d3a13fc1e1f56d3`  
		Last Modified: Thu, 02 Mar 2023 02:38:12 GMT  
		Size: 26.7 MB (26699035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a3333370dc8d23b791b4a6098f7f5a10c7edf844266e90f4027f4e85981b72`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 6.6 MB (6598072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f663586508fee1a498937d0779dfdbae3bcdd16334d54ee9295ca50aae552925`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 3.6 MB (3601892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce67b0569d875d7056824c4c9c02ac70786fa3b8901c3ba0c6a858c857ce0bd`  
		Last Modified: Thu, 02 Mar 2023 02:38:26 GMT  
		Size: 39.5 MB (39513912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0db24a7a1ff9ccf851045d646cb819453ab387ed800c01a3a0f234fa8c71c3`  
		Last Modified: Thu, 02 Mar 2023 02:38:52 GMT  
		Size: 170.3 MB (170295838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:da85a6b734638362d2f993972e3b8ec68846eb431f3f2fdeedf687d8ac682289
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281316326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f776e0dbfe7e0b9c9603f7c9158b78045c957cc54cef4b5ea1b4a69a99d04fb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:56:23 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:56:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:56:27 GMT
ADD file:541d2da8938972bd21842a8a4c8d2074a201f6f70eec4400110f90f1bc28f0e1 in / 
# Mon, 20 Feb 2023 11:56:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:39:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:afd8565abf9be19b25020425f0eef75bc6822497a915ac2ad7e299221258381b`  
		Last Modified: Thu, 02 Mar 2023 03:59:19 GMT  
		Size: 32.1 MB (32109672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c606979686591e3e15c259fedc8c72d14b5f5cb30789d4ac4fc1e7b2344079`  
		Last Modified: Thu, 02 Mar 2023 03:59:13 GMT  
		Size: 7.7 MB (7747700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30e23fe35619983be2169d8e199c937a090ab1f2c783261d342664a3574b67`  
		Last Modified: Thu, 02 Mar 2023 03:59:12 GMT  
		Size: 4.4 MB (4362546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738d753846623f2bf928d9c5ee5e40f7f523f14dd1df06fa8cb96528ab78ea3d`  
		Last Modified: Thu, 02 Mar 2023 03:59:42 GMT  
		Size: 44.1 MB (44141551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4808e644763bc63b9e5a0012ee36f28595205b8ba752baa09653edc02b649d9`  
		Last Modified: Thu, 02 Mar 2023 04:00:40 GMT  
		Size: 193.0 MB (192954857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8f715a88742ef8c20c9effa99fd07f25badf877ba6c4b81a7dbcca330da9f3a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228623596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4de103be19308a9f31f03e0d9527d2b7acda4dcae2f487b70ae0d2fe2d3ac6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:44:03 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:44:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:44:05 GMT
ADD file:9d71356e3a29a835345254e233ddbd3a67941764476c2c7a5a2d0f8a61a84115 in / 
# Mon, 20 Feb 2023 11:44:05 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:13:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:13:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:15:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bcfec0e313701229d74107ece843bd247955551cd676760c2ab56d6fbf1b157`  
		Last Modified: Thu, 02 Mar 2023 02:24:05 GMT  
		Size: 26.0 MB (26029678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741bf338192206d205e17575928e1ec37123b068da0fbfb2c33ff60198620f61`  
		Last Modified: Thu, 02 Mar 2023 02:23:59 GMT  
		Size: 6.5 MB (6461557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19aa30c75a1427834711cd28f44ba117f910f7b5c4e50f923f34ea300cd0cd`  
		Last Modified: Thu, 02 Mar 2023 02:23:58 GMT  
		Size: 3.6 MB (3625033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810d2ec3d82d4c030df6fc52d887b2bb1e9a1c9f01e957fe9dfcdea137a33d2`  
		Last Modified: Thu, 02 Mar 2023 02:24:19 GMT  
		Size: 39.6 MB (39555093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550cbac5a853fefec1b90b7e5a36dd208f74c615aaa79029f1a99c6fc499c3e2`  
		Last Modified: Thu, 02 Mar 2023 02:24:46 GMT  
		Size: 153.0 MB (152952235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:90955da3a53928299fa7a945b4072d569c0739bcce57a8472b481888082d4e99
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
$ docker pull buildpack-deps@sha256:c1bef77a747c1b0d0e2e1943063d242d97b14090c6fa5a4396872c2e5e86cd7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37884733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f070e17b881f324f200c61c5d2fbd431ae10cc95570becf16c69abab64af58b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:43:07 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:43:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:43:09 GMT
ADD file:18f562911635a03a9bf9e5fc22863fc2a78a64f7d35c7daa59f2d609b7ca055a in / 
# Mon, 20 Feb 2023 11:43:10 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:33:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:34:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a10df61efde6b7f0cf3fbf848a5bed1c943a54e13566f30ef6a0cc6f259a2f33`  
		Last Modified: Thu, 02 Mar 2023 03:44:58 GMT  
		Size: 27.5 MB (27479398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9f9f71b0155b4b832dcb9bfbf542389507996cd93239b78300535c9421961`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 6.8 MB (6770219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710e0dcd6284a414a9f90e76d5555002980ba77c51b01d6a812e56d2c2d94d2e`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 3.6 MB (3635116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b87d2b37a07f2b3373c8b775d1355e3139b302bd1713c89dcdbe11519b218229
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35635282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d205c4c1777db2634384c44cf05affec171465def20dbcbf581b53881c97c8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 12:11:32 GMT
ARG RELEASE
# Mon, 20 Feb 2023 12:11:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 12:11:42 GMT
ADD file:f77393d0d614b99f7ca8de09afc58a2e98d9d25c84c5ff69b50e94e7f191f7bb in / 
# Mon, 20 Feb 2023 12:11:43 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:43:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:43:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e07337a9bc2a6220f565efbaf0abbba7718bb8478f0af5b255df655e98cacc06`  
		Last Modified: Thu, 02 Mar 2023 11:57:20 GMT  
		Size: 25.9 MB (25893079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84854174ca4e4c0ad5221cd0bface3a62279cc1659c26e61319a54c79f28a32`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 5.9 MB (5941095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcf439bd51bffc866ae5a81a2764cc54c7f76949d34e14d2ef5666243a5c9e6`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 3.8 MB (3801108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3c113e07442a77b7e938f4bc9ef5b846f44b9cbbdc3cfc058ba264eb8738928d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36898999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caca0113519d729a4a7c61672a55b06acb176ea63c6920446e280ef75b4dca74`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:58:05 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:58:13 GMT
ADD file:7e756337f8554849df664b30203a26f6c39dc303e277292de31fd784b9ff471b in / 
# Mon, 20 Feb 2023 11:58:13 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:26:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:30762c7e5d854e6efb956328165eb8c43cbcf6c0be6766a45d3a13fc1e1f56d3`  
		Last Modified: Thu, 02 Mar 2023 02:38:12 GMT  
		Size: 26.7 MB (26699035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a3333370dc8d23b791b4a6098f7f5a10c7edf844266e90f4027f4e85981b72`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 6.6 MB (6598072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f663586508fee1a498937d0779dfdbae3bcdd16334d54ee9295ca50aae552925`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 3.6 MB (3601892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:28895716799511a352dbc3b87633877569c448c91716b07fafceed861075e0ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44219918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb34ae855f68523ba0fb2c64a0473de1fc81baf2afdac185774fc659174ca56f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:56:23 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:56:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:56:27 GMT
ADD file:541d2da8938972bd21842a8a4c8d2074a201f6f70eec4400110f90f1bc28f0e1 in / 
# Mon, 20 Feb 2023 11:56:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:afd8565abf9be19b25020425f0eef75bc6822497a915ac2ad7e299221258381b`  
		Last Modified: Thu, 02 Mar 2023 03:59:19 GMT  
		Size: 32.1 MB (32109672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c606979686591e3e15c259fedc8c72d14b5f5cb30789d4ac4fc1e7b2344079`  
		Last Modified: Thu, 02 Mar 2023 03:59:13 GMT  
		Size: 7.7 MB (7747700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30e23fe35619983be2169d8e199c937a090ab1f2c783261d342664a3574b67`  
		Last Modified: Thu, 02 Mar 2023 03:59:12 GMT  
		Size: 4.4 MB (4362546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b0150ef7049140aa70bbf29415a11063465c948a00c24d38fa2fbb671f63a581
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36116268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:493a98847f6a760a3d453b6d316eb112b0f292f9513022c75fa6a97376df7fe4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:44:03 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:44:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:44:05 GMT
ADD file:9d71356e3a29a835345254e233ddbd3a67941764476c2c7a5a2d0f8a61a84115 in / 
# Mon, 20 Feb 2023 11:44:05 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:13:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:13:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8bcfec0e313701229d74107ece843bd247955551cd676760c2ab56d6fbf1b157`  
		Last Modified: Thu, 02 Mar 2023 02:24:05 GMT  
		Size: 26.0 MB (26029678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741bf338192206d205e17575928e1ec37123b068da0fbfb2c33ff60198620f61`  
		Last Modified: Thu, 02 Mar 2023 02:23:59 GMT  
		Size: 6.5 MB (6461557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19aa30c75a1427834711cd28f44ba117f910f7b5c4e50f923f34ea300cd0cd`  
		Last Modified: Thu, 02 Mar 2023 02:23:58 GMT  
		Size: 3.6 MB (3625033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:b0e53314b314ebf0ffb12bb21dd7d20a6a45fca68be9c9775074c8769779be87
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
$ docker pull buildpack-deps@sha256:047a981c3c4d581bea16d7a0cd289b348dfa07629f24b6cc7f6add1dcc94d1aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77624743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc182bbb00ba8809b6ffb1c35841b67fd97eba00c6901a88c09dde29acd761f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:43:07 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:43:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:43:09 GMT
ADD file:18f562911635a03a9bf9e5fc22863fc2a78a64f7d35c7daa59f2d609b7ca055a in / 
# Mon, 20 Feb 2023 11:43:10 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:33:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:34:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:34:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a10df61efde6b7f0cf3fbf848a5bed1c943a54e13566f30ef6a0cc6f259a2f33`  
		Last Modified: Thu, 02 Mar 2023 03:44:58 GMT  
		Size: 27.5 MB (27479398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9f9f71b0155b4b832dcb9bfbf542389507996cd93239b78300535c9421961`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 6.8 MB (6770219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710e0dcd6284a414a9f90e76d5555002980ba77c51b01d6a812e56d2c2d94d2e`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 3.6 MB (3635116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c20cf6be4d508b2c166988b50c5ae18cead28e74cf5a620d56202faabfe64a`  
		Last Modified: Thu, 02 Mar 2023 03:45:14 GMT  
		Size: 39.7 MB (39740010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:40dd970891c5342e622abad06cef1abb7a1028fba4ea2e2cac5ba2e86654970d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78243033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b55dc8cebae19b3759058aa86d016dbd0c5b250a29ad01f961ea9507b3a27e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 12:11:32 GMT
ARG RELEASE
# Mon, 20 Feb 2023 12:11:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 12:11:42 GMT
ADD file:f77393d0d614b99f7ca8de09afc58a2e98d9d25c84c5ff69b50e94e7f191f7bb in / 
# Mon, 20 Feb 2023 12:11:43 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:43:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:43:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:44:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e07337a9bc2a6220f565efbaf0abbba7718bb8478f0af5b255df655e98cacc06`  
		Last Modified: Thu, 02 Mar 2023 11:57:20 GMT  
		Size: 25.9 MB (25893079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84854174ca4e4c0ad5221cd0bface3a62279cc1659c26e61319a54c79f28a32`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 5.9 MB (5941095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcf439bd51bffc866ae5a81a2764cc54c7f76949d34e14d2ef5666243a5c9e6`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 3.8 MB (3801108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f989583c8ba595c2fb646ad093cc454bdb75e54ffe38ddcab4b7dc16bdb7e049`  
		Last Modified: Thu, 02 Mar 2023 11:57:37 GMT  
		Size: 42.6 MB (42607751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:88e78a3e652b4b1af808021cb0b7be8e51482011249ba472e8c57ca4c852bdce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76412911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b558fd4728f4339d55d53189136d2d8d5681ab84008e295f189ebb8e86b603e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:58:05 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:58:13 GMT
ADD file:7e756337f8554849df664b30203a26f6c39dc303e277292de31fd784b9ff471b in / 
# Mon, 20 Feb 2023 11:58:13 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:26:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:27:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30762c7e5d854e6efb956328165eb8c43cbcf6c0be6766a45d3a13fc1e1f56d3`  
		Last Modified: Thu, 02 Mar 2023 02:38:12 GMT  
		Size: 26.7 MB (26699035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a3333370dc8d23b791b4a6098f7f5a10c7edf844266e90f4027f4e85981b72`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 6.6 MB (6598072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f663586508fee1a498937d0779dfdbae3bcdd16334d54ee9295ca50aae552925`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 3.6 MB (3601892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce67b0569d875d7056824c4c9c02ac70786fa3b8901c3ba0c6a858c857ce0bd`  
		Last Modified: Thu, 02 Mar 2023 02:38:26 GMT  
		Size: 39.5 MB (39513912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:88398a25e6df8710f62c22d86345a8fa3f84e0713a6ac0c996896c2bcac959ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88361469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1049a1bbcae803adb4a16ecc2adb582978810a7ddfb5ea9ec24da206f4be1ce1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:56:23 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:56:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:56:27 GMT
ADD file:541d2da8938972bd21842a8a4c8d2074a201f6f70eec4400110f90f1bc28f0e1 in / 
# Mon, 20 Feb 2023 11:56:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:39:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:afd8565abf9be19b25020425f0eef75bc6822497a915ac2ad7e299221258381b`  
		Last Modified: Thu, 02 Mar 2023 03:59:19 GMT  
		Size: 32.1 MB (32109672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c606979686591e3e15c259fedc8c72d14b5f5cb30789d4ac4fc1e7b2344079`  
		Last Modified: Thu, 02 Mar 2023 03:59:13 GMT  
		Size: 7.7 MB (7747700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30e23fe35619983be2169d8e199c937a090ab1f2c783261d342664a3574b67`  
		Last Modified: Thu, 02 Mar 2023 03:59:12 GMT  
		Size: 4.4 MB (4362546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738d753846623f2bf928d9c5ee5e40f7f523f14dd1df06fa8cb96528ab78ea3d`  
		Last Modified: Thu, 02 Mar 2023 03:59:42 GMT  
		Size: 44.1 MB (44141551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fb2be6a90e849d0cee6c46ce77e713c60d83023e6b19401fffbdaf695bc333a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75671361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecf79aedb1597b523736958d2e35a21cb919903f602fc38c3a7ac2730bd0d59`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:44:03 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:44:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:44:05 GMT
ADD file:9d71356e3a29a835345254e233ddbd3a67941764476c2c7a5a2d0f8a61a84115 in / 
# Mon, 20 Feb 2023 11:44:05 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:13:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:13:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bcfec0e313701229d74107ece843bd247955551cd676760c2ab56d6fbf1b157`  
		Last Modified: Thu, 02 Mar 2023 02:24:05 GMT  
		Size: 26.0 MB (26029678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741bf338192206d205e17575928e1ec37123b068da0fbfb2c33ff60198620f61`  
		Last Modified: Thu, 02 Mar 2023 02:23:59 GMT  
		Size: 6.5 MB (6461557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19aa30c75a1427834711cd28f44ba117f910f7b5c4e50f923f34ea300cd0cd`  
		Last Modified: Thu, 02 Mar 2023 02:23:58 GMT  
		Size: 3.6 MB (3625033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810d2ec3d82d4c030df6fc52d887b2bb1e9a1c9f01e957fe9dfcdea137a33d2`  
		Last Modified: Thu, 02 Mar 2023 02:24:19 GMT  
		Size: 39.6 MB (39555093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:6f2703639d3d17f70288d4ba212d55e159b682a990c20fc2a6562b098f01a1e7
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
$ docker pull buildpack-deps@sha256:478bf93abb60da60c1188a076991f4dc9638195df95ba30b3377b06e7196d247
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301085570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23f7a118464453742cb6c2f3bd831c8193e5f35cc52d2f9c0f6b179d3309f2a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:23:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef506d17f8897590ad73117349f3d5a00bf1d49e9df07123ad9e5f62bdc1b9c`  
		Last Modified: Wed, 01 Mar 2023 14:35:52 GMT  
		Size: 4.9 MB (4922204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcd4f409b03d9914948b724b57835b18c4640aab6bc493cc80b3a874ffcc31`  
		Last Modified: Wed, 01 Mar 2023 14:35:54 GMT  
		Size: 10.7 MB (10662168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df25173951f289c64515ba71fb87f8b90d9d1951e7287d8fc1a6b5f12c5c567`  
		Last Modified: Wed, 01 Mar 2023 14:36:41 GMT  
		Size: 53.3 MB (53307045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaeb72ebe84fa1592a617e85865bdf44882a111fe77d3709017d0944f7666f9`  
		Last Modified: Wed, 01 Mar 2023 14:38:36 GMT  
		Size: 178.9 MB (178928978 bytes)  
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
$ docker pull buildpack-deps@sha256:8c345dca9c9fc0c22ebf88e7b956b00b5e91fcc28bb20ed50f22942cfccb0b9e
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
$ docker pull buildpack-deps@sha256:dd059c3bad41c1793f0bda5fc655d3f11e84347d773ad26d8f8f9e33c667ff84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.4 MB (279400819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1152e1ec96916d1e0da389234ee993c5d6910729d6c68faaefec28f6ffb24d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:14 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:16 GMT
ADD file:a99f804e480d9a1b56aff6406b4da5a3dea89f11f968e5e02cd4ba5a25e9a7bc in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:38:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:41:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6347900c239eb6451b578d272779198ff2efe221eb716c1ee35bb33b3d36c805`  
		Last Modified: Thu, 02 Mar 2023 03:45:59 GMT  
		Size: 27.5 MB (27450641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fc9b499f00984f063653ce41c5bcd7a2101d4709bde16211c9cd61cf53c97`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 6.6 MB (6637316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583126b5de1692321379f3ac3c479e60776c2630177157537ce16c3b5310534c`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 3.7 MB (3690222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4e53abb79424a77d128c854eb7fbd2dc2baf538b9618ecdc1377d5c513a4d`  
		Last Modified: Thu, 02 Mar 2023 03:46:14 GMT  
		Size: 44.5 MB (44515661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a67102021c513567e5ad98778b40b5627ec23a5472f9c98da44bd4a7a1529`  
		Last Modified: Thu, 02 Mar 2023 03:46:53 GMT  
		Size: 197.1 MB (197106979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4b44c93e90c08a0c8ebe34455d42edaee9ca6bbc11842ce669bb625fc4076c8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.4 MB (230379620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca6c0fae7a4451d14049e9b225c0e7940914f5ca0a2808b4cf73cd9f97e1462`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:43 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:44 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:53 GMT
ADD file:e4ec0e899927e1fe0388f3524f3382183df8c74bcf9de0e35e1c8120acbc2b7a in / 
# Wed, 01 Mar 2023 05:41:53 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:48:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:48:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:49:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:51:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3149fccce04237916ad21629e6497df2edac53a12b13cf63470e4ee5833f8e4`  
		Last Modified: Thu, 02 Mar 2023 11:58:22 GMT  
		Size: 26.2 MB (26236811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1c91da9e0e927655ec912d3e65425143bf9d0dc2bde931112305247aa3dca7`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 5.8 MB (5809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee07824f253241f1cd1a7d308e85f8d6bfdb3649f0d1db1d5c49d1b1ff337a`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 3.9 MB (3852238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307ab9ceb5b6a487ea64bb9ab76e4c75483c4dd388afefcc036953ad0170c750`  
		Last Modified: Thu, 02 Mar 2023 11:58:40 GMT  
		Size: 48.6 MB (48604125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d587719a598d516477984ca010b771e6121e70f384a8612c804c4cbac316a`  
		Last Modified: Thu, 02 Mar 2023 11:59:09 GMT  
		Size: 145.9 MB (145877278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d8524c1c281222c12d123a4dc95c47e7b344cba0f7b944e9db5a7b76901c8e91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269571646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d507b30adaf2193c1c4e65e7384e76f5769f09ecb89a38418b845784e49b1599`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:57:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:57:22 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 04:57:30 GMT
ADD file:54e98f6282fdf165c9986b859ed60d05e28d3f9575c1c4915537cba24c6ec95c in / 
# Wed, 01 Mar 2023 04:57:31 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:30:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:31:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:34:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6700b5ef6bf750ef532062fc9dec24b7d9247840b877f26af1f339df77db5ba1`  
		Last Modified: Thu, 02 Mar 2023 02:39:03 GMT  
		Size: 26.9 MB (26899339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01eb5985b1759d7a00fafb6eaa0426c9ba33b24bab18656ae5ed19b74869bd3`  
		Last Modified: Thu, 02 Mar 2023 02:39:02 GMT  
		Size: 6.5 MB (6468687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136aa3449032f883f29b10908230ca4a5c79c1a4fcf12f1c28fa763b07ac0db`  
		Last Modified: Thu, 02 Mar 2023 02:39:01 GMT  
		Size: 3.6 MB (3649336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99899628512ddfc061595eb4f812d31ea2842eb378a4f491eb3ab8c133270a51`  
		Last Modified: Thu, 02 Mar 2023 02:39:17 GMT  
		Size: 44.4 MB (44350881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe305ba6cd09ca5b32809bcb5cbb3c76cfb40ef0bb6c985399edbe3a38611745`  
		Last Modified: Thu, 02 Mar 2023 02:39:45 GMT  
		Size: 188.2 MB (188203403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2c247cf6ae7ab7790b2e6ef7b6f22e062c03be67c2e6ec746c9e3028d4d9fdac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.6 MB (304625782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e1e8fb8f901f6cc5bea34fb55d0d589b98d798b4d46f5efa69fa124e3f78e10`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:58 GMT
ADD file:dd48763269678622cf7a1219a8b87a1222a24048b5cc1ab133a42cbb854c7f78 in / 
# Wed, 01 Mar 2023 05:00:58 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:52:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434ae6294eb01eccffad6e8e39b3f373d83e33cfedaa3f3cb70962a1122776f0`  
		Last Modified: Thu, 02 Mar 2023 04:01:02 GMT  
		Size: 31.9 MB (31897489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316ed6bd69a08f1739325fc66aebcc6c5bf34087b52b0f3a2e4bfca0c109e76d`  
		Last Modified: Thu, 02 Mar 2023 04:00:56 GMT  
		Size: 7.6 MB (7606587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba7fe918b6d86615ad6aaad9cb8d4e29030952575a61624dbb8f5e15f5ca8f9`  
		Last Modified: Thu, 02 Mar 2023 04:00:55 GMT  
		Size: 4.4 MB (4409088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0e010afca98d127a9b0d8607ac999fc79b19e8d612c6fc6e3a9e1ee1a1de76`  
		Last Modified: Thu, 02 Mar 2023 04:01:28 GMT  
		Size: 49.3 MB (49321485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf0a080521e887133fd7499f1530a995a4cd125cee300dc695cb79d843c68bb`  
		Last Modified: Thu, 02 Mar 2023 04:02:28 GMT  
		Size: 211.4 MB (211391133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e7e0da949a243441e9689733560d210e4400951613c1d2b5d97c7bb40587fa65
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.8 MB (250781790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a2a2bae085525070f7daabc96186ad663394847a35d43f5afe2d72617c073b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:55 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:57 GMT
ADD file:88bec1acfbc8ba8a59354ff2c1f510d9e301748628aa39527cca86d8150209e8 in / 
# Wed, 01 Mar 2023 05:00:57 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:16:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:17:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:19:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e8382b8ddc15579f4e533ad8581d16988174176dacd958bc0572d8e6417518f`  
		Last Modified: Thu, 02 Mar 2023 02:24:57 GMT  
		Size: 26.1 MB (26072339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2428ddac9d5ad4baa24cd9a8735e4aa63591aa90c5e18869189f772ac106cd2`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 6.3 MB (6319521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b57b8f1cbfb3971975200f23660e4e6bb616038be4ec693552ebd91f202ed1`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 3.7 MB (3674671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f1225557f2081b054aaa9ce9fa92db7eaf86f05602bd00bb497082952dd77c`  
		Last Modified: Thu, 02 Mar 2023 02:25:13 GMT  
		Size: 44.3 MB (44337360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787d7f0ffdc1c3dc79e056d7f534a0f5485a77be47f876d2965e7e4b1303ed1`  
		Last Modified: Thu, 02 Mar 2023 02:25:42 GMT  
		Size: 170.4 MB (170377899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-curl`

```console
$ docker pull buildpack-deps@sha256:ea0932754db65dc7cdd16c157b662925e1812053f5bd5bc536549998bdf2a2fd
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
$ docker pull buildpack-deps@sha256:4e65f9beff33426d8e782c4e765e86c5b79c6ff355c07b850a10a11557439a93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37778179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e37d1b86e663a732896bf3d39af7f0224e89bee8471e9c1bba9e4e100eaf04a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:14 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:16 GMT
ADD file:a99f804e480d9a1b56aff6406b4da5a3dea89f11f968e5e02cd4ba5a25e9a7bc in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6347900c239eb6451b578d272779198ff2efe221eb716c1ee35bb33b3d36c805`  
		Last Modified: Thu, 02 Mar 2023 03:45:59 GMT  
		Size: 27.5 MB (27450641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fc9b499f00984f063653ce41c5bcd7a2101d4709bde16211c9cd61cf53c97`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 6.6 MB (6637316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583126b5de1692321379f3ac3c479e60776c2630177157537ce16c3b5310534c`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 3.7 MB (3690222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a94b128e1356b799bc1441e88a775175a23a1ab09e255182bdf025735ab65a24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35898217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:393d2f7b0cbdfaba72c5950beec03aac8c5c421b400119d520b1541476804dc9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:43 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:44 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:53 GMT
ADD file:e4ec0e899927e1fe0388f3524f3382183df8c74bcf9de0e35e1c8120acbc2b7a in / 
# Wed, 01 Mar 2023 05:41:53 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:48:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:48:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f3149fccce04237916ad21629e6497df2edac53a12b13cf63470e4ee5833f8e4`  
		Last Modified: Thu, 02 Mar 2023 11:58:22 GMT  
		Size: 26.2 MB (26236811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1c91da9e0e927655ec912d3e65425143bf9d0dc2bde931112305247aa3dca7`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 5.8 MB (5809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee07824f253241f1cd1a7d308e85f8d6bfdb3649f0d1db1d5c49d1b1ff337a`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 3.9 MB (3852238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:29528af07c334f5ec5040c5656f9ff1b25e6a8fd192b3f2a05a2cb91c8ba94ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (37017362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b36694a82191fe66369b4b4b6a2d3d01d64ae1342857f637441504de865ca45a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:57:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:57:22 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 04:57:30 GMT
ADD file:54e98f6282fdf165c9986b859ed60d05e28d3f9575c1c4915537cba24c6ec95c in / 
# Wed, 01 Mar 2023 04:57:31 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:30:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6700b5ef6bf750ef532062fc9dec24b7d9247840b877f26af1f339df77db5ba1`  
		Last Modified: Thu, 02 Mar 2023 02:39:03 GMT  
		Size: 26.9 MB (26899339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01eb5985b1759d7a00fafb6eaa0426c9ba33b24bab18656ae5ed19b74869bd3`  
		Last Modified: Thu, 02 Mar 2023 02:39:02 GMT  
		Size: 6.5 MB (6468687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136aa3449032f883f29b10908230ca4a5c79c1a4fcf12f1c28fa763b07ac0db`  
		Last Modified: Thu, 02 Mar 2023 02:39:01 GMT  
		Size: 3.6 MB (3649336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:969acb495b97e4865f3a4be732f30166c4c8d498c36c2aa550561dbb09811de0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43913164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff2d43f367892255637542904d83ecd5cd4f07e36220da96cd5ec7e64cf1e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:58 GMT
ADD file:dd48763269678622cf7a1219a8b87a1222a24048b5cc1ab133a42cbb854c7f78 in / 
# Wed, 01 Mar 2023 05:00:58 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:434ae6294eb01eccffad6e8e39b3f373d83e33cfedaa3f3cb70962a1122776f0`  
		Last Modified: Thu, 02 Mar 2023 04:01:02 GMT  
		Size: 31.9 MB (31897489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316ed6bd69a08f1739325fc66aebcc6c5bf34087b52b0f3a2e4bfca0c109e76d`  
		Last Modified: Thu, 02 Mar 2023 04:00:56 GMT  
		Size: 7.6 MB (7606587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba7fe918b6d86615ad6aaad9cb8d4e29030952575a61624dbb8f5e15f5ca8f9`  
		Last Modified: Thu, 02 Mar 2023 04:00:55 GMT  
		Size: 4.4 MB (4409088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f899ac870d7e9fddcf8aa13caff6163265029ce5ce54986e8b09b54e73c198e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36066531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c53d3d23aef5fdf01fc69c9886733334a4d214bdfb2827d16fcc812fa5857d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:55 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:57 GMT
ADD file:88bec1acfbc8ba8a59354ff2c1f510d9e301748628aa39527cca86d8150209e8 in / 
# Wed, 01 Mar 2023 05:00:57 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:16:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9e8382b8ddc15579f4e533ad8581d16988174176dacd958bc0572d8e6417518f`  
		Last Modified: Thu, 02 Mar 2023 02:24:57 GMT  
		Size: 26.1 MB (26072339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2428ddac9d5ad4baa24cd9a8735e4aa63591aa90c5e18869189f772ac106cd2`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 6.3 MB (6319521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b57b8f1cbfb3971975200f23660e4e6bb616038be4ec693552ebd91f202ed1`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 3.7 MB (3674671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:e2ce24a28c5ffa329922d8a7fd842b4f01e5dedae68529b743195ef776b5bdd2
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
$ docker pull buildpack-deps@sha256:dfca8dc06d26d3a6045ceef176d672df2185198782833ce82c81f3417487b7e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82293840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11db010a0e4873cf66ebbbaeb58004ef354ea6507c99ebed518c311dd06e6fe4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:14 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:14 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:16 GMT
ADD file:a99f804e480d9a1b56aff6406b4da5a3dea89f11f968e5e02cd4ba5a25e9a7bc in / 
# Wed, 01 Mar 2023 05:41:17 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:38:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6347900c239eb6451b578d272779198ff2efe221eb716c1ee35bb33b3d36c805`  
		Last Modified: Thu, 02 Mar 2023 03:45:59 GMT  
		Size: 27.5 MB (27450641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635fc9b499f00984f063653ce41c5bcd7a2101d4709bde16211c9cd61cf53c97`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 6.6 MB (6637316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583126b5de1692321379f3ac3c479e60776c2630177157537ce16c3b5310534c`  
		Last Modified: Thu, 02 Mar 2023 03:45:56 GMT  
		Size: 3.7 MB (3690222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4e53abb79424a77d128c854eb7fbd2dc2baf538b9618ecdc1377d5c513a4d`  
		Last Modified: Thu, 02 Mar 2023 03:46:14 GMT  
		Size: 44.5 MB (44515661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:13ccc3def0daf769539fd0ca304f2a28da88d5bb794c46c1f93916f458251517
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84502342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a304d21e8dd95ea8eeb55ef412cc1ac9bbd4acf5075c01142941f14b6f9005ce`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:43 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:44 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:41:53 GMT
ADD file:e4ec0e899927e1fe0388f3524f3382183df8c74bcf9de0e35e1c8120acbc2b7a in / 
# Wed, 01 Mar 2023 05:41:53 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:48:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:48:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 11:49:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3149fccce04237916ad21629e6497df2edac53a12b13cf63470e4ee5833f8e4`  
		Last Modified: Thu, 02 Mar 2023 11:58:22 GMT  
		Size: 26.2 MB (26236811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1c91da9e0e927655ec912d3e65425143bf9d0dc2bde931112305247aa3dca7`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 5.8 MB (5809168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee07824f253241f1cd1a7d308e85f8d6bfdb3649f0d1db1d5c49d1b1ff337a`  
		Last Modified: Thu, 02 Mar 2023 11:58:18 GMT  
		Size: 3.9 MB (3852238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307ab9ceb5b6a487ea64bb9ab76e4c75483c4dd388afefcc036953ad0170c750`  
		Last Modified: Thu, 02 Mar 2023 11:58:40 GMT  
		Size: 48.6 MB (48604125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4d2316040e83fb85fcf5553a00d9884e58bc4ae0ac45f809513198b31164f7a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81368243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78899799edcb9bb2076bbcfe6bcfb75f1dffa05836b5c21617593bc97cd03734`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:57:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:57:22 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:57:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 04:57:30 GMT
ADD file:54e98f6282fdf165c9986b859ed60d05e28d3f9575c1c4915537cba24c6ec95c in / 
# Wed, 01 Mar 2023 04:57:31 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:30:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:31:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6700b5ef6bf750ef532062fc9dec24b7d9247840b877f26af1f339df77db5ba1`  
		Last Modified: Thu, 02 Mar 2023 02:39:03 GMT  
		Size: 26.9 MB (26899339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01eb5985b1759d7a00fafb6eaa0426c9ba33b24bab18656ae5ed19b74869bd3`  
		Last Modified: Thu, 02 Mar 2023 02:39:02 GMT  
		Size: 6.5 MB (6468687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136aa3449032f883f29b10908230ca4a5c79c1a4fcf12f1c28fa763b07ac0db`  
		Last Modified: Thu, 02 Mar 2023 02:39:01 GMT  
		Size: 3.6 MB (3649336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99899628512ddfc061595eb4f812d31ea2842eb378a4f491eb3ab8c133270a51`  
		Last Modified: Thu, 02 Mar 2023 02:39:17 GMT  
		Size: 44.4 MB (44350881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:39d5d1468937ce1cd50fdd52cb7dfc5d713f2a7494ac3925626f12ee6e417278
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93234649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7fbab15a93c2f95048c838e9d8a6e32252fb4b63ec05dd2b4fec7ba3acaf270`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:58 GMT
ADD file:dd48763269678622cf7a1219a8b87a1222a24048b5cc1ab133a42cbb854c7f78 in / 
# Wed, 01 Mar 2023 05:00:58 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 03:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434ae6294eb01eccffad6e8e39b3f373d83e33cfedaa3f3cb70962a1122776f0`  
		Last Modified: Thu, 02 Mar 2023 04:01:02 GMT  
		Size: 31.9 MB (31897489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316ed6bd69a08f1739325fc66aebcc6c5bf34087b52b0f3a2e4bfca0c109e76d`  
		Last Modified: Thu, 02 Mar 2023 04:00:56 GMT  
		Size: 7.6 MB (7606587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba7fe918b6d86615ad6aaad9cb8d4e29030952575a61624dbb8f5e15f5ca8f9`  
		Last Modified: Thu, 02 Mar 2023 04:00:55 GMT  
		Size: 4.4 MB (4409088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0e010afca98d127a9b0d8607ac999fc79b19e8d612c6fc6e3a9e1ee1a1de76`  
		Last Modified: Thu, 02 Mar 2023 04:01:28 GMT  
		Size: 49.3 MB (49321485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d2881270036984bf5335b8711121ff83ff86c5a2728ced037c770bedde7b192b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80403891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a23c0ce9ee9418f0b679ceeecc5514d7858bc439fcffeb582fb2d84c7f6a80c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:00:55 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:00:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:00:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 01 Mar 2023 05:00:57 GMT
ADD file:88bec1acfbc8ba8a59354ff2c1f510d9e301748628aa39527cca86d8150209e8 in / 
# Wed, 01 Mar 2023 05:00:57 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:16:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:16:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:17:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e8382b8ddc15579f4e533ad8581d16988174176dacd958bc0572d8e6417518f`  
		Last Modified: Thu, 02 Mar 2023 02:24:57 GMT  
		Size: 26.1 MB (26072339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2428ddac9d5ad4baa24cd9a8735e4aa63591aa90c5e18869189f772ac106cd2`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 6.3 MB (6319521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b57b8f1cbfb3971975200f23660e4e6bb616038be4ec693552ebd91f202ed1`  
		Last Modified: Thu, 02 Mar 2023 02:24:55 GMT  
		Size: 3.7 MB (3674671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f1225557f2081b054aaa9ce9fa92db7eaf86f05602bd00bb497082952dd77c`  
		Last Modified: Thu, 02 Mar 2023 02:25:13 GMT  
		Size: 44.3 MB (44337360 bytes)  
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
$ docker pull buildpack-deps@sha256:ca9b375648e50b4c26007c99cb7dca68626fc42863c01841d7232f41e166130e
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
$ docker pull buildpack-deps@sha256:a342b7a73b4c0cabe77fc12a63c608a8114dd750b757d720688dd114ddca8f98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122156592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f29263ab5584d0b1394d255686d09c9b9acec2b70d35751fc7e2b81f63e3202`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef506d17f8897590ad73117349f3d5a00bf1d49e9df07123ad9e5f62bdc1b9c`  
		Last Modified: Wed, 01 Mar 2023 14:35:52 GMT  
		Size: 4.9 MB (4922204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcd4f409b03d9914948b724b57835b18c4640aab6bc493cc80b3a874ffcc31`  
		Last Modified: Wed, 01 Mar 2023 14:35:54 GMT  
		Size: 10.7 MB (10662168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df25173951f289c64515ba71fb87f8b90d9d1951e7287d8fc1a6b5f12c5c567`  
		Last Modified: Wed, 01 Mar 2023 14:36:41 GMT  
		Size: 53.3 MB (53307045 bytes)  
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
$ docker pull buildpack-deps@sha256:3665f214cc7a833c3bbd719b8cb29ccfe77232df1a05c7018f1cdd7fa0a79597
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
$ docker pull buildpack-deps@sha256:47dc0fbb2a082ab8902bdd131ee988a5f0e00dcefd372fb7bfeea467c0c1ace6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.4 MB (321371150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51fb9a05e6abe2c06e4797caa146e7499b646b00ed39cde466eff314a31d0ee7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:11:29 GMT
ADD file:0cba93ebf4cf24adc0d2ab76ca2285ed3e4c1d07e2498a55a964f61a47d0f560 in / 
# Wed, 01 Mar 2023 02:11:34 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:25:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:27:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:32:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6fa2f96bfa02eb0ced41b1f356f7b6aa1c6dcd2de446f0e6931fb513751316f`  
		Last Modified: Wed, 01 Mar 2023 02:19:32 GMT  
		Size: 49.3 MB (49270629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d065d7ea1126da8c947e70a82de46ea4f5654122ed4491abeca140ff6e5c5865`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 8.4 MB (8431807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee9fdc617c60ef3cb7ebd08a285a7f5620969f1115a7d36b712df4a1d6a5a21`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 11.2 MB (11153650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aa7dc7af7fb2bbb1d9ee43b715bd2063af972d33a79974539ff4b29aa3ad89`  
		Last Modified: Wed, 01 Mar 2023 14:39:42 GMT  
		Size: 63.0 MB (62993873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96576f9b714a0a396d90707c7026ab68f17a79237d0fca82751b6c6ff8f9c9ae`  
		Last Modified: Wed, 01 Mar 2023 14:41:44 GMT  
		Size: 189.5 MB (189521191 bytes)  
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
$ docker pull buildpack-deps@sha256:ee4d912a0ada15896576fb69ce8da356854eb12fdba498e31214fb0b9fc5689b
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
$ docker pull buildpack-deps@sha256:2554f9cf67dc27292de873a393ce0d758d73a78d5eb3d20edd417f7c2ca2c199
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68856086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:710aca4721d36199d2da95c21696054d4433794324cb9b451e24ba3e5ecb99ed`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:11:29 GMT
ADD file:0cba93ebf4cf24adc0d2ab76ca2285ed3e4c1d07e2498a55a964f61a47d0f560 in / 
# Wed, 01 Mar 2023 02:11:34 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:25:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f6fa2f96bfa02eb0ced41b1f356f7b6aa1c6dcd2de446f0e6931fb513751316f`  
		Last Modified: Wed, 01 Mar 2023 02:19:32 GMT  
		Size: 49.3 MB (49270629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d065d7ea1126da8c947e70a82de46ea4f5654122ed4491abeca140ff6e5c5865`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 8.4 MB (8431807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee9fdc617c60ef3cb7ebd08a285a7f5620969f1115a7d36b712df4a1d6a5a21`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 11.2 MB (11153650 bytes)  
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
$ docker pull buildpack-deps@sha256:1a8c68907c58a2cb19020509ee7cd91bc363c6d0dc7baada92f5917d877574fc
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
$ docker pull buildpack-deps@sha256:0482d45883838e5543ea9770e77901ebaa4dc56c528bd6fad1fafe421f25df94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131849959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf77dcd74f170edd0ff9bf5e8d84d9ca2156a4d23eb5ccd126584f94082ab3f6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:11:29 GMT
ADD file:0cba93ebf4cf24adc0d2ab76ca2285ed3e4c1d07e2498a55a964f61a47d0f560 in / 
# Wed, 01 Mar 2023 02:11:34 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:25:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:27:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6fa2f96bfa02eb0ced41b1f356f7b6aa1c6dcd2de446f0e6931fb513751316f`  
		Last Modified: Wed, 01 Mar 2023 02:19:32 GMT  
		Size: 49.3 MB (49270629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d065d7ea1126da8c947e70a82de46ea4f5654122ed4491abeca140ff6e5c5865`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 8.4 MB (8431807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee9fdc617c60ef3cb7ebd08a285a7f5620969f1115a7d36b712df4a1d6a5a21`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 11.2 MB (11153650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aa7dc7af7fb2bbb1d9ee43b715bd2063af972d33a79974539ff4b29aa3ad89`  
		Last Modified: Wed, 01 Mar 2023 14:39:42 GMT  
		Size: 63.0 MB (62993873 bytes)  
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
$ docker pull buildpack-deps@sha256:6f2703639d3d17f70288d4ba212d55e159b682a990c20fc2a6562b098f01a1e7
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
$ docker pull buildpack-deps@sha256:478bf93abb60da60c1188a076991f4dc9638195df95ba30b3377b06e7196d247
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301085570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23f7a118464453742cb6c2f3bd831c8193e5f35cc52d2f9c0f6b179d3309f2a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:23:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef506d17f8897590ad73117349f3d5a00bf1d49e9df07123ad9e5f62bdc1b9c`  
		Last Modified: Wed, 01 Mar 2023 14:35:52 GMT  
		Size: 4.9 MB (4922204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcd4f409b03d9914948b724b57835b18c4640aab6bc493cc80b3a874ffcc31`  
		Last Modified: Wed, 01 Mar 2023 14:35:54 GMT  
		Size: 10.7 MB (10662168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df25173951f289c64515ba71fb87f8b90d9d1951e7287d8fc1a6b5f12c5c567`  
		Last Modified: Wed, 01 Mar 2023 14:36:41 GMT  
		Size: 53.3 MB (53307045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaeb72ebe84fa1592a617e85865bdf44882a111fe77d3709017d0944f7666f9`  
		Last Modified: Wed, 01 Mar 2023 14:38:36 GMT  
		Size: 178.9 MB (178928978 bytes)  
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
$ docker pull buildpack-deps@sha256:1b0af9f90719ef87bfec766349df533e0b9051282d2cf845c6584fbc4412b70d
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
$ docker pull buildpack-deps@sha256:a6f2a19a68aa123aad96add6fc1b3303e711608e3f67ef461202424893602731
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68849547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335938bead68388bf68af487c365a97a41376b45ccc2f2d17893aab6ba39a233`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef506d17f8897590ad73117349f3d5a00bf1d49e9df07123ad9e5f62bdc1b9c`  
		Last Modified: Wed, 01 Mar 2023 14:35:52 GMT  
		Size: 4.9 MB (4922204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcd4f409b03d9914948b724b57835b18c4640aab6bc493cc80b3a874ffcc31`  
		Last Modified: Wed, 01 Mar 2023 14:35:54 GMT  
		Size: 10.7 MB (10662168 bytes)  
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
$ docker pull buildpack-deps@sha256:ca9b375648e50b4c26007c99cb7dca68626fc42863c01841d7232f41e166130e
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
$ docker pull buildpack-deps@sha256:a342b7a73b4c0cabe77fc12a63c608a8114dd750b757d720688dd114ddca8f98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122156592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f29263ab5584d0b1394d255686d09c9b9acec2b70d35751fc7e2b81f63e3202`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef506d17f8897590ad73117349f3d5a00bf1d49e9df07123ad9e5f62bdc1b9c`  
		Last Modified: Wed, 01 Mar 2023 14:35:52 GMT  
		Size: 4.9 MB (4922204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcd4f409b03d9914948b724b57835b18c4640aab6bc493cc80b3a874ffcc31`  
		Last Modified: Wed, 01 Mar 2023 14:35:54 GMT  
		Size: 10.7 MB (10662168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df25173951f289c64515ba71fb87f8b90d9d1951e7287d8fc1a6b5f12c5c567`  
		Last Modified: Wed, 01 Mar 2023 14:36:41 GMT  
		Size: 53.3 MB (53307045 bytes)  
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
$ docker pull buildpack-deps@sha256:9212e46cdbd63c438f51632df2951c70ccd898648a5ba90e82adf0fc03a6786c
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
$ docker pull buildpack-deps@sha256:26ae81f0d87b16da338ff5e9aaa7d9401fd2e69444797c89e96130cf4042b3c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321235599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:131ecc0b55080b3773d14fd12cb1b4d190b56336d637a82e5348fac7737471f0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:09:05 GMT
ADD file:77abd413b6799ae4f1f24f3bcc389dd12515fc4f732e81239d8c25475bc37fac in / 
# Wed, 01 Mar 2023 02:09:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:07:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:07:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:09:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:15:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65f9863fa983221d5b14b7a7e06e92e49a04fbced0e7af12bdafbdfcbc7a2deb`  
		Last Modified: Wed, 01 Mar 2023 02:16:56 GMT  
		Size: 49.2 MB (49245473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bcf13485e3ee0cadac8054427f8f6f3a08a8542574c273072b5a938746e826`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 8.4 MB (8414213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56e46e1c6aaa24d965fe76a54803920eb56ce4ab2092a6993067da3dd253f8`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 11.2 MB (11153696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e391ddfe06a9169f7cea164ba5cd6836dce99ef8ba4fc6f3cb9b0b3b79f63f`  
		Last Modified: Wed, 01 Mar 2023 14:33:39 GMT  
		Size: 62.9 MB (62920983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee394f8b54a43ab6674140143e254f3b40806874e56d6b59eca1035e6308e7b2`  
		Last Modified: Wed, 01 Mar 2023 14:35:40 GMT  
		Size: 189.5 MB (189501234 bytes)  
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
$ docker pull buildpack-deps@sha256:4a5f77cacf83c9f3c521015d89b61490036eab8481ac4d91e454f207fc666512
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
$ docker pull buildpack-deps@sha256:3a972cbb1aa6f0bf3842a0b059977a9d854135a4f95bfda1e4aac50feea75fb9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68813382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84bc6ab63e76ee0ebb37779fc3faacb153b7561e4475d7901826171b7a28e86`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:09:05 GMT
ADD file:77abd413b6799ae4f1f24f3bcc389dd12515fc4f732e81239d8c25475bc37fac in / 
# Wed, 01 Mar 2023 02:09:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:07:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:07:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:65f9863fa983221d5b14b7a7e06e92e49a04fbced0e7af12bdafbdfcbc7a2deb`  
		Last Modified: Wed, 01 Mar 2023 02:16:56 GMT  
		Size: 49.2 MB (49245473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bcf13485e3ee0cadac8054427f8f6f3a08a8542574c273072b5a938746e826`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 8.4 MB (8414213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56e46e1c6aaa24d965fe76a54803920eb56ce4ab2092a6993067da3dd253f8`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 11.2 MB (11153696 bytes)  
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
$ docker pull buildpack-deps@sha256:f9571020b467313c668d9cfbe8ebaa011f376e998adf9c90d32071626d0a07fa
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
$ docker pull buildpack-deps@sha256:7160ec99476b0a2468b9e7a2eb492fcc969b360833f5ccd8ef15e62729232c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131734365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2ccbb6f9934bc8cabfebd1553a774f9b2b06bb6a6162921a03743859ff60482`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:09:05 GMT
ADD file:77abd413b6799ae4f1f24f3bcc389dd12515fc4f732e81239d8c25475bc37fac in / 
# Wed, 01 Mar 2023 02:09:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:07:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:07:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:09:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65f9863fa983221d5b14b7a7e06e92e49a04fbced0e7af12bdafbdfcbc7a2deb`  
		Last Modified: Wed, 01 Mar 2023 02:16:56 GMT  
		Size: 49.2 MB (49245473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bcf13485e3ee0cadac8054427f8f6f3a08a8542574c273072b5a938746e826`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 8.4 MB (8414213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56e46e1c6aaa24d965fe76a54803920eb56ce4ab2092a6993067da3dd253f8`  
		Last Modified: Wed, 01 Mar 2023 14:32:49 GMT  
		Size: 11.2 MB (11153696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e391ddfe06a9169f7cea164ba5cd6836dce99ef8ba4fc6f3cb9b0b3b79f63f`  
		Last Modified: Wed, 01 Mar 2023 14:33:39 GMT  
		Size: 62.9 MB (62920983 bytes)  
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
$ docker pull buildpack-deps@sha256:3665f214cc7a833c3bbd719b8cb29ccfe77232df1a05c7018f1cdd7fa0a79597
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
$ docker pull buildpack-deps@sha256:47dc0fbb2a082ab8902bdd131ee988a5f0e00dcefd372fb7bfeea467c0c1ace6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.4 MB (321371150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51fb9a05e6abe2c06e4797caa146e7499b646b00ed39cde466eff314a31d0ee7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:11:29 GMT
ADD file:0cba93ebf4cf24adc0d2ab76ca2285ed3e4c1d07e2498a55a964f61a47d0f560 in / 
# Wed, 01 Mar 2023 02:11:34 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:25:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:27:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:32:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6fa2f96bfa02eb0ced41b1f356f7b6aa1c6dcd2de446f0e6931fb513751316f`  
		Last Modified: Wed, 01 Mar 2023 02:19:32 GMT  
		Size: 49.3 MB (49270629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d065d7ea1126da8c947e70a82de46ea4f5654122ed4491abeca140ff6e5c5865`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 8.4 MB (8431807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee9fdc617c60ef3cb7ebd08a285a7f5620969f1115a7d36b712df4a1d6a5a21`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 11.2 MB (11153650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aa7dc7af7fb2bbb1d9ee43b715bd2063af972d33a79974539ff4b29aa3ad89`  
		Last Modified: Wed, 01 Mar 2023 14:39:42 GMT  
		Size: 63.0 MB (62993873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96576f9b714a0a396d90707c7026ab68f17a79237d0fca82751b6c6ff8f9c9ae`  
		Last Modified: Wed, 01 Mar 2023 14:41:44 GMT  
		Size: 189.5 MB (189521191 bytes)  
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
$ docker pull buildpack-deps@sha256:ee4d912a0ada15896576fb69ce8da356854eb12fdba498e31214fb0b9fc5689b
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
$ docker pull buildpack-deps@sha256:2554f9cf67dc27292de873a393ce0d758d73a78d5eb3d20edd417f7c2ca2c199
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68856086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:710aca4721d36199d2da95c21696054d4433794324cb9b451e24ba3e5ecb99ed`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:11:29 GMT
ADD file:0cba93ebf4cf24adc0d2ab76ca2285ed3e4c1d07e2498a55a964f61a47d0f560 in / 
# Wed, 01 Mar 2023 02:11:34 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:25:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f6fa2f96bfa02eb0ced41b1f356f7b6aa1c6dcd2de446f0e6931fb513751316f`  
		Last Modified: Wed, 01 Mar 2023 02:19:32 GMT  
		Size: 49.3 MB (49270629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d065d7ea1126da8c947e70a82de46ea4f5654122ed4491abeca140ff6e5c5865`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 8.4 MB (8431807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee9fdc617c60ef3cb7ebd08a285a7f5620969f1115a7d36b712df4a1d6a5a21`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 11.2 MB (11153650 bytes)  
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
$ docker pull buildpack-deps@sha256:1a8c68907c58a2cb19020509ee7cd91bc363c6d0dc7baada92f5917d877574fc
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
$ docker pull buildpack-deps@sha256:0482d45883838e5543ea9770e77901ebaa4dc56c528bd6fad1fafe421f25df94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131849959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf77dcd74f170edd0ff9bf5e8d84d9ca2156a4d23eb5ccd126584f94082ab3f6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:11:29 GMT
ADD file:0cba93ebf4cf24adc0d2ab76ca2285ed3e4c1d07e2498a55a964f61a47d0f560 in / 
# Wed, 01 Mar 2023 02:11:34 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:25:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 14:27:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6fa2f96bfa02eb0ced41b1f356f7b6aa1c6dcd2de446f0e6931fb513751316f`  
		Last Modified: Wed, 01 Mar 2023 02:19:32 GMT  
		Size: 49.3 MB (49270629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d065d7ea1126da8c947e70a82de46ea4f5654122ed4491abeca140ff6e5c5865`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 8.4 MB (8431807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee9fdc617c60ef3cb7ebd08a285a7f5620969f1115a7d36b712df4a1d6a5a21`  
		Last Modified: Wed, 01 Mar 2023 14:38:52 GMT  
		Size: 11.2 MB (11153650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aa7dc7af7fb2bbb1d9ee43b715bd2063af972d33a79974539ff4b29aa3ad89`  
		Last Modified: Wed, 01 Mar 2023 14:39:42 GMT  
		Size: 63.0 MB (62993873 bytes)  
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
