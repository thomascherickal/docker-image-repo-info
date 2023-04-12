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
$ docker pull buildpack-deps@sha256:fb154449c96034e2ac28a113cfbc31b7da0e4a21387c397dec6b1deec6d89d73
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
$ docker pull buildpack-deps@sha256:b1da6a5f500b67fa28bbae2b90a8e9da4def283d1fb918b1d4db0c9cd86ec183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221417037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeecfa359fe257650879cc03de2c96ee1ab252d40eaf9467a855893ac7df28f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:21:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:21:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:24:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c78e6dac9cec3c01ca7687f8e0a53a4b5e9b04f4910729279be4204ce5360e`  
		Last Modified: Thu, 16 Mar 2023 05:41:29 GMT  
		Size: 6.6 MB (6617364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b18b892afad36455b3ae75f0ab2c1bc45822e03069f2667faa4bede3825be5`  
		Last Modified: Thu, 16 Mar 2023 05:41:28 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c57462ca1fd8565d56aa476a7fa497011a11c6f761194b368d2c722e146b20`  
		Last Modified: Thu, 16 Mar 2023 05:41:43 GMT  
		Size: 45.5 MB (45514749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f391d58903094b86c56fd169ec96c398321c3ccab4f8893113f4de938d003a`  
		Last Modified: Thu, 16 Mar 2023 05:42:10 GMT  
		Size: 139.5 MB (139548050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f740f07a329775404244fd36ca65500a61ecd79c38851ee6ce6408443fa9779
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189581013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb26767826b27bb17bc813102a23903c31d4ea475f341486310a77dd6e54d766`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:44:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:45:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:47:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2b71966fc2f22e1375423fb61221ed137cf5e7e8d202bfa403292ba600daab`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 5.7 MB (5681012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf04b4bbda07472ffbb83ab11cb71b6ff2c6bef9749979a8a3981f285c0f53`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 2.6 MB (2586979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3058bdcdd1b82bda414133ce433d46f98b5f56911e44f00ff6bd1de1c0a6caba`  
		Last Modified: Thu, 16 Mar 2023 04:08:04 GMT  
		Size: 40.7 MB (40713543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d88abc5604e52bcee192566d8fae426f1031f855abd4229bd8c43feeb2648d`  
		Last Modified: Thu, 16 Mar 2023 04:08:30 GMT  
		Size: 118.3 MB (118294105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2c9e464ea859a1b832272828463904e3f9c04bdebf0e7aa9cdc4c6c48481c85e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (206011203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b97289739597eaf439933630ebefa90822ac12cd90c8157a55e7b3f32763f4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:58:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:59:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc06fc1cf8ad0140062ec53dbc631cea853ddb72d7c0b353edd743b1dca4ceb`  
		Last Modified: Thu, 16 Mar 2023 04:21:50 GMT  
		Size: 6.1 MB (6057809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d0b4e623a1829e474acf7b4d21109a9f27c7d8c8bf12f163ffe645eed93ec`  
		Last Modified: Thu, 16 Mar 2023 04:21:49 GMT  
		Size: 2.8 MB (2790695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37de71f159d52bbc91be8b71a2d8862f89e2c137ac5d4e17c923aaa4fa5aa30`  
		Last Modified: Thu, 16 Mar 2023 04:22:03 GMT  
		Size: 43.3 MB (43311869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc13acad8ae8946317f508f7e0eda6de200ca13831f7433e58942f2466c21473`  
		Last Modified: Thu, 16 Mar 2023 04:22:25 GMT  
		Size: 130.1 MB (130116124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d189ba12fe145c64ea06852f5de7d0ab170ab04daca4c5effd4a4705cabb888e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218710648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc3d7329f212c3056b20a7f0084491a4e3d07e63c6848a789189f5137e2d75d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:19 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:21 GMT
ADD file:6cf3e34995c6c44762ed692b86a0442d981e9a69fa4288960047e505d75c0223 in / 
# Wed, 08 Mar 2023 03:13:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:57:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:00:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58af8b772f2ca9c63db81d620e48946c13c027ecd7ab2d9062d010ca2ed11f3`  
		Last Modified: Thu, 16 Mar 2023 01:54:42 GMT  
		Size: 27.2 MB (27164610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df9a7dbeea70a625098ba195b5c6a6046e010992d4b2616b74e5efca85ff0`  
		Last Modified: Thu, 16 Mar 2023 02:02:18 GMT  
		Size: 6.9 MB (6907798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9c7488bcb45de5faeb1bc3f4a19015817de4a09d3c762c619d48aa2855322e`  
		Last Modified: Thu, 16 Mar 2023 02:02:17 GMT  
		Size: 3.3 MB (3255693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54663dad9d7f237e7f0a0a533af683ae66d66098cdd57ea8f90fde4dd8897ffb`  
		Last Modified: Thu, 16 Mar 2023 02:02:38 GMT  
		Size: 47.1 MB (47095486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5e9e49852091a0f82ca614c93efb7802ff6bbabc0da2e14b9606920c072cb6`  
		Last Modified: Thu, 16 Mar 2023 02:03:15 GMT  
		Size: 134.3 MB (134287061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:093d533487c60b2c92363199f07f041884638f879f09c20c9aa303e056b1267c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246441203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcd83e221d1f7aaec4fdcb03d7776c2eadf8d9cf89c85eaba5ab7f7793f25ed`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:07:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:08:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:14:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e5cf4c1f014d5508f129bb3d2e36a3448b5d92b400a35d3051160723af42b4`  
		Last Modified: Thu, 16 Mar 2023 03:47:41 GMT  
		Size: 7.0 MB (7036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a259ed8117f57e3f76e8e31ddb857f6d36e8f1ac8131d38a456833aa7e0c20`  
		Last Modified: Thu, 16 Mar 2023 03:47:40 GMT  
		Size: 3.7 MB (3740612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409f528497ffaa0bc9ae78b8139359ddd38315caf439a39a670aaed487c6c06d`  
		Last Modified: Thu, 16 Mar 2023 03:48:07 GMT  
		Size: 53.7 MB (53736792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22095eabcbee3060dd218f09d76cf296a873b1a36d1d4f86794d105fe7e5ec5f`  
		Last Modified: Thu, 16 Mar 2023 03:48:53 GMT  
		Size: 151.5 MB (151484912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0c8e0a8e8c0a624863dcfee0278ed624183fd34de9612945d2db9d6842c229d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205782934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8557c42f5d0087a913e9c89b40998da81a7d55355bad38d52f6b3f7699f2681b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:23:29 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:23:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:23:31 GMT
ADD file:a6309e462d28398152cb726a11615118d79858da963b8c614772b87d87465967 in / 
# Wed, 08 Mar 2023 03:23:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:43:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:44:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:46:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3a2279f06ab19f0d57823e69b999f54a344e28bd9f955b4db9a5875c0caa543a`  
		Last Modified: Thu, 16 Mar 2023 02:01:03 GMT  
		Size: 25.4 MB (25370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37be097f66ed2ca5a62bf5e79eee23cbae99ae37fa4214bd021813206a4896`  
		Last Modified: Thu, 16 Mar 2023 02:01:00 GMT  
		Size: 6.3 MB (6310585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffee9aa0246535c2e55658c3cb0a6996668f7a403a4b960a9fdbcd4d42847f3`  
		Last Modified: Thu, 16 Mar 2023 02:00:59 GMT  
		Size: 3.0 MB (2976589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc2dd868684ceaf83a27108c1b52ca7a6e8f3b0168ad780911abc88235bfb03`  
		Last Modified: Thu, 16 Mar 2023 02:01:18 GMT  
		Size: 45.0 MB (45040946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df620083a573baec7672a8d7b904f0c02ababd741e0ace4108dda4b119901ee2`  
		Last Modified: Thu, 16 Mar 2023 02:01:42 GMT  
		Size: 126.1 MB (126083821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-curl`

```console
$ docker pull buildpack-deps@sha256:3fd8a96d4a8804a8424ff1593c4b2858231aa0c710e83e5c826fab6724f4037f
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
$ docker pull buildpack-deps@sha256:edc4ef3195e1d82ba936e48a088384a87de4ef1e079743cf63a8590eb9a20bfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36354238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36747240a25171490608a4897f503021ceb197cb460e20444ca7089a2453ea7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:21:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:21:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c78e6dac9cec3c01ca7687f8e0a53a4b5e9b04f4910729279be4204ce5360e`  
		Last Modified: Thu, 16 Mar 2023 05:41:29 GMT  
		Size: 6.6 MB (6617364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b18b892afad36455b3ae75f0ab2c1bc45822e03069f2667faa4bede3825be5`  
		Last Modified: Thu, 16 Mar 2023 05:41:28 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:37305f1fffd9b6e8b98b050b702e595498870f5d0cf8cbc4d2e30cdcc7b2177a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30573365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45de6bc525f3e1c8327e7663ff847e537821bb211ca5fe282aa4fe66f79c36f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:44:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:45:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2b71966fc2f22e1375423fb61221ed137cf5e7e8d202bfa403292ba600daab`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 5.7 MB (5681012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf04b4bbda07472ffbb83ab11cb71b6ff2c6bef9749979a8a3981f285c0f53`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 2.6 MB (2586979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bbaa8d87e02533fb9f0e332551bec711913649f23f663cb20c4c47c5323680f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32583210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3656a9cc190e6da3224283797ac375e158b4a022d1d5a3d2bb49d9dac0b85124`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:58:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc06fc1cf8ad0140062ec53dbc631cea853ddb72d7c0b353edd743b1dca4ceb`  
		Last Modified: Thu, 16 Mar 2023 04:21:50 GMT  
		Size: 6.1 MB (6057809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d0b4e623a1829e474acf7b4d21109a9f27c7d8c8bf12f163ffe645eed93ec`  
		Last Modified: Thu, 16 Mar 2023 04:21:49 GMT  
		Size: 2.8 MB (2790695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c88613067a38450529dace018781fd35548bed5b209c241a5262b458b0e48a52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37328101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e48e7492b46c775c749e6d5febf5731b1aeface4bf187ab7edb99482a1e0f64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:19 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:21 GMT
ADD file:6cf3e34995c6c44762ed692b86a0442d981e9a69fa4288960047e505d75c0223 in / 
# Wed, 08 Mar 2023 03:13:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c58af8b772f2ca9c63db81d620e48946c13c027ecd7ab2d9062d010ca2ed11f3`  
		Last Modified: Thu, 16 Mar 2023 01:54:42 GMT  
		Size: 27.2 MB (27164610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df9a7dbeea70a625098ba195b5c6a6046e010992d4b2616b74e5efca85ff0`  
		Last Modified: Thu, 16 Mar 2023 02:02:18 GMT  
		Size: 6.9 MB (6907798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9c7488bcb45de5faeb1bc3f4a19015817de4a09d3c762c619d48aa2855322e`  
		Last Modified: Thu, 16 Mar 2023 02:02:17 GMT  
		Size: 3.3 MB (3255693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:93af7cd2c9b2348c3885ca9fad668d06a219296d9c2032725a0d3de25878e908
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41219499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1588570491594531960cec00e2bb87f2fb1b48f878dc4d6bd888024f30e1de`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:07:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e5cf4c1f014d5508f129bb3d2e36a3448b5d92b400a35d3051160723af42b4`  
		Last Modified: Thu, 16 Mar 2023 03:47:41 GMT  
		Size: 7.0 MB (7036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a259ed8117f57e3f76e8e31ddb857f6d36e8f1ac8131d38a456833aa7e0c20`  
		Last Modified: Thu, 16 Mar 2023 03:47:40 GMT  
		Size: 3.7 MB (3740612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:20ebcda199381e882997d1cb49046a4a86cf2a4d85ec17a0d4cf03c2342dee11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34658167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f626e5ed1171f12e2d4e06623f35558e748ecc2010eb93c132ab27524b2b55b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:23:29 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:23:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:23:31 GMT
ADD file:a6309e462d28398152cb726a11615118d79858da963b8c614772b87d87465967 in / 
# Wed, 08 Mar 2023 03:23:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:43:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3a2279f06ab19f0d57823e69b999f54a344e28bd9f955b4db9a5875c0caa543a`  
		Last Modified: Thu, 16 Mar 2023 02:01:03 GMT  
		Size: 25.4 MB (25370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37be097f66ed2ca5a62bf5e79eee23cbae99ae37fa4214bd021813206a4896`  
		Last Modified: Thu, 16 Mar 2023 02:01:00 GMT  
		Size: 6.3 MB (6310585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffee9aa0246535c2e55658c3cb0a6996668f7a403a4b960a9fdbcd4d42847f3`  
		Last Modified: Thu, 16 Mar 2023 02:00:59 GMT  
		Size: 3.0 MB (2976589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:18.04-scm`

```console
$ docker pull buildpack-deps@sha256:341aade2e27224f02ffa8406356d222ae812b4b877d9cae398a6f1c9c8aa1fb3
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
$ docker pull buildpack-deps@sha256:c5ed4186cca291cb15e4a3ec07c8f72214eecb664ab6000d21de81b4ef3c22eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81868987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee72242d4f5e40206fc21b1eda028beb28d7d73857bfdba0cc421a166b05b081`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:21:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:21:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c78e6dac9cec3c01ca7687f8e0a53a4b5e9b04f4910729279be4204ce5360e`  
		Last Modified: Thu, 16 Mar 2023 05:41:29 GMT  
		Size: 6.6 MB (6617364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b18b892afad36455b3ae75f0ab2c1bc45822e03069f2667faa4bede3825be5`  
		Last Modified: Thu, 16 Mar 2023 05:41:28 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c57462ca1fd8565d56aa476a7fa497011a11c6f761194b368d2c722e146b20`  
		Last Modified: Thu, 16 Mar 2023 05:41:43 GMT  
		Size: 45.5 MB (45514749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f9d5b0d3c5fb26bbcb17109b65208ac2a36d7a6a4253289e090c1e39fbe1744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71286908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf91a3d86cf7e62586cfa021d5d042c3f8ad4473ddc03742ce5fe9199395303a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:44:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:45:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2b71966fc2f22e1375423fb61221ed137cf5e7e8d202bfa403292ba600daab`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 5.7 MB (5681012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf04b4bbda07472ffbb83ab11cb71b6ff2c6bef9749979a8a3981f285c0f53`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 2.6 MB (2586979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3058bdcdd1b82bda414133ce433d46f98b5f56911e44f00ff6bd1de1c0a6caba`  
		Last Modified: Thu, 16 Mar 2023 04:08:04 GMT  
		Size: 40.7 MB (40713543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:127e2166fb2409edd8d8b5261a115a0e2aec1641f2bc70769b51e60924fda8eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75895079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c55e4c16477e8e6ec9875fa4a0fc1eb3184b34403fb222976e5a361d5ab3466`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:58:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:59:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc06fc1cf8ad0140062ec53dbc631cea853ddb72d7c0b353edd743b1dca4ceb`  
		Last Modified: Thu, 16 Mar 2023 04:21:50 GMT  
		Size: 6.1 MB (6057809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d0b4e623a1829e474acf7b4d21109a9f27c7d8c8bf12f163ffe645eed93ec`  
		Last Modified: Thu, 16 Mar 2023 04:21:49 GMT  
		Size: 2.8 MB (2790695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37de71f159d52bbc91be8b71a2d8862f89e2c137ac5d4e17c923aaa4fa5aa30`  
		Last Modified: Thu, 16 Mar 2023 04:22:03 GMT  
		Size: 43.3 MB (43311869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:06347734d5e392a96f4432d6290610b9761773fe58a4467957bb5ac5c104e085
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84423587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea41bed709b37c2011e131b1f224971e01f761e9a8b0c487987ca43d939e5062`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:19 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:21 GMT
ADD file:6cf3e34995c6c44762ed692b86a0442d981e9a69fa4288960047e505d75c0223 in / 
# Wed, 08 Mar 2023 03:13:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:57:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58af8b772f2ca9c63db81d620e48946c13c027ecd7ab2d9062d010ca2ed11f3`  
		Last Modified: Thu, 16 Mar 2023 01:54:42 GMT  
		Size: 27.2 MB (27164610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df9a7dbeea70a625098ba195b5c6a6046e010992d4b2616b74e5efca85ff0`  
		Last Modified: Thu, 16 Mar 2023 02:02:18 GMT  
		Size: 6.9 MB (6907798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9c7488bcb45de5faeb1bc3f4a19015817de4a09d3c762c619d48aa2855322e`  
		Last Modified: Thu, 16 Mar 2023 02:02:17 GMT  
		Size: 3.3 MB (3255693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54663dad9d7f237e7f0a0a533af683ae66d66098cdd57ea8f90fde4dd8897ffb`  
		Last Modified: Thu, 16 Mar 2023 02:02:38 GMT  
		Size: 47.1 MB (47095486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:47ffaea8984e18680bf34023dc84dbbc005a5c50b47cb92e9221be8e55ce28a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94956291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e8cb730f01b5b2426648fed56c18477b531abea23c6d47db1eacc88079b2ab4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:07:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:08:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e5cf4c1f014d5508f129bb3d2e36a3448b5d92b400a35d3051160723af42b4`  
		Last Modified: Thu, 16 Mar 2023 03:47:41 GMT  
		Size: 7.0 MB (7036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a259ed8117f57e3f76e8e31ddb857f6d36e8f1ac8131d38a456833aa7e0c20`  
		Last Modified: Thu, 16 Mar 2023 03:47:40 GMT  
		Size: 3.7 MB (3740612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409f528497ffaa0bc9ae78b8139359ddd38315caf439a39a670aaed487c6c06d`  
		Last Modified: Thu, 16 Mar 2023 03:48:07 GMT  
		Size: 53.7 MB (53736792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:18.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3e5c483b07d9d0b5a4f4dbb989320ab32f2ccc83e8b565759f680a7659b1961c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79699113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d8b61386e03e4309345be55e3dd943e007820aadcbcc64fb24e1524fea86052`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:23:29 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:23:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:23:31 GMT
ADD file:a6309e462d28398152cb726a11615118d79858da963b8c614772b87d87465967 in / 
# Wed, 08 Mar 2023 03:23:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:43:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:44:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3a2279f06ab19f0d57823e69b999f54a344e28bd9f955b4db9a5875c0caa543a`  
		Last Modified: Thu, 16 Mar 2023 02:01:03 GMT  
		Size: 25.4 MB (25370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37be097f66ed2ca5a62bf5e79eee23cbae99ae37fa4214bd021813206a4896`  
		Last Modified: Thu, 16 Mar 2023 02:01:00 GMT  
		Size: 6.3 MB (6310585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffee9aa0246535c2e55658c3cb0a6996668f7a403a4b960a9fdbcd4d42847f3`  
		Last Modified: Thu, 16 Mar 2023 02:00:59 GMT  
		Size: 3.0 MB (2976589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc2dd868684ceaf83a27108c1b52ca7a6e8f3b0168ad780911abc88235bfb03`  
		Last Modified: Thu, 16 Mar 2023 02:01:18 GMT  
		Size: 45.0 MB (45040946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04`

```console
$ docker pull buildpack-deps@sha256:19c0f7f64b8335561e884c84493a4a3480f90912af313ce1584b55dac0410045
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
$ docker pull buildpack-deps@sha256:a499d7cf331a38e4daf02148cf1f4b908048eab65947d337c4954bf635d37592
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245775730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7906168918fbe41e4eacbec9b2252ee5a4c8d9ab004d3ba2719b59d4a9719c3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:25:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:25:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:26:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:28:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bc9af4214222561c992590ace8ae277238c112e32760c1ff3ef6caf8ca4f6`  
		Last Modified: Thu, 16 Mar 2023 05:42:20 GMT  
		Size: 7.7 MB (7739206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155d64edd9d618f19a8fecb84dfbc4cf87eff8210625c22cc9634721fba93a7f`  
		Last Modified: Thu, 16 Mar 2023 05:42:19 GMT  
		Size: 3.6 MB (3627138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231a0ed819686e9daf3eef08ba444c6b7ebd1f65cdb1fe72aef57a0f6bb50b44`  
		Last Modified: Thu, 16 Mar 2023 05:42:37 GMT  
		Size: 60.7 MB (60741678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd7ee9669c83df2d803ace7367f27ea8d15d3ef24e11274c8810ecfb106739c`  
		Last Modified: Thu, 16 Mar 2023 05:43:05 GMT  
		Size: 145.1 MB (145089640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7328be0f102351eef287e2517d6ee5c2bbe3f4148f3a5ea2cfe48671892d56ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211775407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dddfdd3085f4ab0f9a8671e25b13cea8ae4112cca857278022e03057c9cada`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:48:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:48:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:49:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:50:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47332fc42b573d4baf56c0357c8403f43cd7e32995cd91e98f1b63904c165edc`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 6.7 MB (6726111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7608366f198edf1178000bf5d347ad633c37686847555ad129799eb689113`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 3.1 MB (3104510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53730f672819fbb90234967569a7b902545c30edae9b2a899cbd60f6d11c64d1`  
		Last Modified: Thu, 16 Mar 2023 04:09:01 GMT  
		Size: 55.4 MB (55433480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053c5c89030c8bd301889d79a2fc68e023925bd9527dc1fc7cab71f8a4bae26f`  
		Last Modified: Thu, 16 Mar 2023 04:09:28 GMT  
		Size: 121.9 MB (121924824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ff57e910e4f7e1d0490a538306c2bc5f7d3c3be91bc6b6d4949901ec3f2a24a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235999544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83ed8c452dfe38712e7bd28165dece30e24886b5d4095feddafa309b723f28c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:03:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:04:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:07:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada92025b6d5b0737643d0b1828f2344b2cdb92c860a121d471b8f0c87875d0c`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 7.6 MB (7602314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d3bbdc78821c82e7efb7e6b25412a925801281a52d89ff278c1440c1682f2`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 3.6 MB (3617260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f381dea6869d6e20db1531b80e454b1082f1678f0397903199ce41446330364`  
		Last Modified: Thu, 16 Mar 2023 04:22:52 GMT  
		Size: 60.8 MB (60817533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0abeae2a014e811b1cd94b6bf883f31eeea92a20e0e001d1142493ed5a2c9e`  
		Last Modified: Thu, 16 Mar 2023 04:23:14 GMT  
		Size: 136.8 MB (136766276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3e9e963156b739e06ca605543ef30f47c13d2f94fa896e98194fbbffdf0948d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269621988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:554288919fbda3305223d05afd514cd056b314df8de2d1ed100be57b04e2fdac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:15:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:17:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:22:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35c7876eb976fb68d0f3bf24f227b6220a73f879e77ad564d913af35104da2eb`  
		Last Modified: Thu, 16 Mar 2023 01:58:06 GMT  
		Size: 33.3 MB (33300378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6346be203b914f77b544d394d2d63c301d06a7b8926cd30449cdb5a3046edc`  
		Last Modified: Thu, 16 Mar 2023 03:49:06 GMT  
		Size: 8.7 MB (8692841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabdc66fc416ff468476139eca7bc89d467220b030d725d5715d0f79364e4c8`  
		Last Modified: Thu, 16 Mar 2023 03:49:04 GMT  
		Size: 4.5 MB (4486834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a7f4b71be518565ac628205f8fc97a71ee63e098c11a5602ff80ad69427db1`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 69.6 MB (69553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87bf022fbd7e81163adf826c15b5acbc213f43f5ea50267acaa3fb720dbf501`  
		Last Modified: Thu, 16 Mar 2023 03:50:23 GMT  
		Size: 153.6 MB (153588308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1d9d8256bc33bab81422b7a398094681d9648a8c654df7a6c1eeebdd004a1e38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226375246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00868f7fb08f67a580a9e48f17f152318ef7cd6afe9d8b40e94cbf0615c43b56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:46:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:47:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:49:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:422c367cdac1ee2f6bd9ea546c8e5a643af0847a822d04ba202af409973273ad`  
		Last Modified: Thu, 16 Mar 2023 01:40:19 GMT  
		Size: 27.0 MB (27016120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a483453055472ff48de1fd6d705ef6ead7ebb9e0846c4954ba91b6fb7660d5`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 7.4 MB (7379309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348a385bccd245fea6b55ab45b16d2bd72f5a321f2339d63941b14ea5af141e`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 3.5 MB (3542074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75aaa62969cac1411806a644c6dfa90c4b1cdbb89ee7952acb34e84da5caa83`  
		Last Modified: Thu, 16 Mar 2023 02:02:05 GMT  
		Size: 60.0 MB (60015921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae1a1a48eef579da3815ca10377b205802a368ab7293d343e8f40d7fed0be9c`  
		Last Modified: Thu, 16 Mar 2023 02:02:29 GMT  
		Size: 128.4 MB (128421822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:603fe1ece48d066ae790ee69b12733fa30d45465034083519f2bfba9c81e5875
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
$ docker pull buildpack-deps@sha256:244b89a7f94d393b379d796cf11687de045affc0a8ec223b9c140cf08cd1d583
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39944412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:502631fc74e69f270fc93f0d999f3c9fd1757effb421af66951f8fde5428f4d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:25:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:25:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bc9af4214222561c992590ace8ae277238c112e32760c1ff3ef6caf8ca4f6`  
		Last Modified: Thu, 16 Mar 2023 05:42:20 GMT  
		Size: 7.7 MB (7739206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155d64edd9d618f19a8fecb84dfbc4cf87eff8210625c22cc9634721fba93a7f`  
		Last Modified: Thu, 16 Mar 2023 05:42:19 GMT  
		Size: 3.6 MB (3627138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1e8bc526fbffc69c9d0e626081bc81793a560032e1e3c4d3a449f5a60672d96f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34417103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c33bbc0c141172ce22bf7cf86bda316933123e335366e1ea9deba8bd6b964d00`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:48:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:48:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47332fc42b573d4baf56c0357c8403f43cd7e32995cd91e98f1b63904c165edc`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 6.7 MB (6726111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7608366f198edf1178000bf5d347ad633c37686847555ad129799eb689113`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 3.1 MB (3104510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ffc84a0fcbb9d176e50ebb0222e5eeb290a58fb42bf38dc74b182632e8e2e222
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38415735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce8c193e0e6515f7fb45285ce5e80b324f558869d3e85d6ccb9c186b56de169b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:03:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada92025b6d5b0737643d0b1828f2344b2cdb92c860a121d471b8f0c87875d0c`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 7.6 MB (7602314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d3bbdc78821c82e7efb7e6b25412a925801281a52d89ff278c1440c1682f2`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 3.6 MB (3617260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6bcb7bbe9e71ec3bf79e404b8dca4821d0a8a8d3e0ba52087d4db6b77cfa2e2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46480053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2030d035639fd89c4173ce60293f8f470778669b33f7cb717d29c96ea46f603`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:15:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:35c7876eb976fb68d0f3bf24f227b6220a73f879e77ad564d913af35104da2eb`  
		Last Modified: Thu, 16 Mar 2023 01:58:06 GMT  
		Size: 33.3 MB (33300378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6346be203b914f77b544d394d2d63c301d06a7b8926cd30449cdb5a3046edc`  
		Last Modified: Thu, 16 Mar 2023 03:49:06 GMT  
		Size: 8.7 MB (8692841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabdc66fc416ff468476139eca7bc89d467220b030d725d5715d0f79364e4c8`  
		Last Modified: Thu, 16 Mar 2023 03:49:04 GMT  
		Size: 4.5 MB (4486834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1c1099e10a2fe4905babce95ad918aafac037e6865e1dd2de6bebf8c1b1b282f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37937503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e125599525fdd8c0449dd97ad937ff4d8e51359718898ac7bf028fcc1e0ef9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:46:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:422c367cdac1ee2f6bd9ea546c8e5a643af0847a822d04ba202af409973273ad`  
		Last Modified: Thu, 16 Mar 2023 01:40:19 GMT  
		Size: 27.0 MB (27016120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a483453055472ff48de1fd6d705ef6ead7ebb9e0846c4954ba91b6fb7660d5`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 7.4 MB (7379309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348a385bccd245fea6b55ab45b16d2bd72f5a321f2339d63941b14ea5af141e`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 3.5 MB (3542074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:9103aa62d5027f1fb05a5d84099d7267fbe850182634fd6e3c294d06663c8a95
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
$ docker pull buildpack-deps@sha256:f50962aa19f626f477ccc1d83a5c7a2c58f82d9ed60236522a10c4283117c4c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100686090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db3508b90f202b776567efc3d8a59364ad1cf351a3a715e39aa46e5fbc8c68b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:25:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:25:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:26:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bc9af4214222561c992590ace8ae277238c112e32760c1ff3ef6caf8ca4f6`  
		Last Modified: Thu, 16 Mar 2023 05:42:20 GMT  
		Size: 7.7 MB (7739206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155d64edd9d618f19a8fecb84dfbc4cf87eff8210625c22cc9634721fba93a7f`  
		Last Modified: Thu, 16 Mar 2023 05:42:19 GMT  
		Size: 3.6 MB (3627138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231a0ed819686e9daf3eef08ba444c6b7ebd1f65cdb1fe72aef57a0f6bb50b44`  
		Last Modified: Thu, 16 Mar 2023 05:42:37 GMT  
		Size: 60.7 MB (60741678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:58f3602ee4c39695c30963274b5faeb2d2167ace201af9f3f4c6eacbf8649880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89850583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77759cced7d3cf207131d1c31211cac9b8d4c861cb3cedfedc5392380534046e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:48:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:48:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:49:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47332fc42b573d4baf56c0357c8403f43cd7e32995cd91e98f1b63904c165edc`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 6.7 MB (6726111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7608366f198edf1178000bf5d347ad633c37686847555ad129799eb689113`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 3.1 MB (3104510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53730f672819fbb90234967569a7b902545c30edae9b2a899cbd60f6d11c64d1`  
		Last Modified: Thu, 16 Mar 2023 04:09:01 GMT  
		Size: 55.4 MB (55433480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cd02558f0a6dfba6c29fb4fd3b69d47d7ed610742c110ad3d48dd3665b3969c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99233268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385e737702d65ec663825da56324f18677ab4add5cb2c78ea43971cfa1d0310d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:03:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:04:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada92025b6d5b0737643d0b1828f2344b2cdb92c860a121d471b8f0c87875d0c`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 7.6 MB (7602314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d3bbdc78821c82e7efb7e6b25412a925801281a52d89ff278c1440c1682f2`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 3.6 MB (3617260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f381dea6869d6e20db1531b80e454b1082f1678f0397903199ce41446330364`  
		Last Modified: Thu, 16 Mar 2023 04:22:52 GMT  
		Size: 60.8 MB (60817533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:04aa4f32a7113bd9a0200497ffd5fbaeff2317498842cec9c830351405426a17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116033680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76b46c4ec83bd6f7f1c891f7e7a478529374a2b66b1958647d5603fbf251d8f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:15:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:17:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35c7876eb976fb68d0f3bf24f227b6220a73f879e77ad564d913af35104da2eb`  
		Last Modified: Thu, 16 Mar 2023 01:58:06 GMT  
		Size: 33.3 MB (33300378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6346be203b914f77b544d394d2d63c301d06a7b8926cd30449cdb5a3046edc`  
		Last Modified: Thu, 16 Mar 2023 03:49:06 GMT  
		Size: 8.7 MB (8692841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabdc66fc416ff468476139eca7bc89d467220b030d725d5715d0f79364e4c8`  
		Last Modified: Thu, 16 Mar 2023 03:49:04 GMT  
		Size: 4.5 MB (4486834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a7f4b71be518565ac628205f8fc97a71ee63e098c11a5602ff80ad69427db1`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 69.6 MB (69553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:92b7d5e1a84baf82d1937e88aa05702580caababdba82c5b27730cf1ad6a71e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (97953424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:240ac351ad3ff93ba8dfd9d10b19e92cfa3c8bcba3868e4927134e37ce7ec2e9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:46:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:47:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:422c367cdac1ee2f6bd9ea546c8e5a643af0847a822d04ba202af409973273ad`  
		Last Modified: Thu, 16 Mar 2023 01:40:19 GMT  
		Size: 27.0 MB (27016120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a483453055472ff48de1fd6d705ef6ead7ebb9e0846c4954ba91b6fb7660d5`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 7.4 MB (7379309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348a385bccd245fea6b55ab45b16d2bd72f5a321f2339d63941b14ea5af141e`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 3.5 MB (3542074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75aaa62969cac1411806a644c6dfa90c4b1cdbb89ee7952acb34e84da5caa83`  
		Last Modified: Thu, 16 Mar 2023 02:02:05 GMT  
		Size: 60.0 MB (60015921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04`

```console
$ docker pull buildpack-deps@sha256:fe20c1a1fa7749ce93af04e56c2a46297e6b236eeddbdb8fd780ec58784c121a
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
$ docker pull buildpack-deps@sha256:c7af89fe20e8b370fa3d84c23f5dbb048e01cfd38fbc12c1e02232c1a84af80f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (250022556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375da4bb35d8bd52aa3070617888fd8aea7a8aec9a99774cdd1df6a8a87cd5ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:29:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:29:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:29:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:32:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7490ba7e16ba382ca21015280e2ee6dad31879a1f043029e350a8e429770f36`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.8 MB (3788671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeb23ea57c359eecf9e21c40ddb69f738e9121008fd4956d733ba66d3b7eb38`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.6 MB (3561600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c00a0ea05e6a2089233e7238bbed0ffbf7b2655f03195967e2083ee623899`  
		Last Modified: Thu, 16 Mar 2023 05:43:30 GMT  
		Size: 39.4 MB (39352910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa902bb14f17725bbd311e77e44da0ef803e68e0965c5f95635eb83f288b5d4`  
		Last Modified: Thu, 16 Mar 2023 05:44:00 GMT  
		Size: 172.9 MB (172889412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:548a747004a966f5fe24d920b0b67a7e2f63d2f84ee8a998d73573f3534d291c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216673703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2805f8c5309daa5cfffe1813e3cf819142f1ed5ef4f8e6be329cbcad71c2d30`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:51:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:51:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:52:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:55:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d54aa809ca004a01d3a10bf7017a1fb216f185fd9d0f210f1bc9512298c1`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.5 MB (3540124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caec72904127d7cb95dfd39a3f311865b026d929e1440427ec21122be6e15db3`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.7 MB (3714418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b259dc20995aa828e48008def151ea3da6891615621976f66dc6b63fdbda38a`  
		Last Modified: Thu, 16 Mar 2023 04:09:57 GMT  
		Size: 41.9 MB (41908320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d21e83a1a0d8dfe0c0f53e1f8d51356e226e68eb9de5b136253db03ceac4e7`  
		Last Modified: Thu, 16 Mar 2023 04:10:26 GMT  
		Size: 140.5 MB (140485444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bc8bb348a53f7d9f3e309b375c7fd76b56a0c48f89c849a9c6ade599cdc8180a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241329007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffb8e18683ff48d54f07c675683997a40a1555dde02c54147d8d9d48aa756df`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:08:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:08:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aef66b301cbfe4ff1bb09357ccf381140239a236438d27a992d076491a3a066`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.8 MB (3760501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693278d975de74bdcb529fd46771b1335b9501b8f479a3c8128b69375f7945a8`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.5 MB (3536190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfc2e7bfd914b57fdeae1d187ca7a12534443f9e2a6142287dab73c0296ade8`  
		Last Modified: Thu, 16 Mar 2023 04:23:36 GMT  
		Size: 39.2 MB (39243621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2292b558961f2b5d5b6555b004730bdf51c7012b78b0a9474df76b1674aaa26`  
		Last Modified: Thu, 16 Mar 2023 04:24:01 GMT  
		Size: 166.4 MB (166401141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d098228e71918993c4063a767b2eef4e86f48651116a36ecd3b3faa15276d498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271846871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55eaa1527dc94604178ceeb1d0dd71d0ef94cf7213d605391668aa27d2fb142e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:24:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:29:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda6a81b65d142865ef5dbb2df2e98c084dc995272e55f804a36f283c6f9cc0a`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.3 MB (4262063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ead6720a64b98a3aff60731463b608c0b67ecd6e1da5fdea16027f2602fed35`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.2 MB (4234751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d902f277ddd72c79a705e87198d386aa6f00888bd94535ac236140f709bbdce`  
		Last Modified: Thu, 16 Mar 2023 03:50:57 GMT  
		Size: 43.8 MB (43768451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e52f20a783e0f77850e23839602213aca9d779491820b6b87d582377010ff1`  
		Last Modified: Thu, 16 Mar 2023 03:51:51 GMT  
		Size: 183.9 MB (183869878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d8f68fa9506203d2ae62c96ff52ca734da392b0abdf6fb87d0b095d32da75234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223696064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:027fabc11727fa0a1d019f1c51338d85905a5113cdc2c03b8c1fbb1f2a852c17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:49:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:50:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:52:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfb18fcfcf98f525d6770606600d80d5413262ce3575995b49064988c1bd147`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.8 MB (3792844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072af6d5dacbd70c88a5e91a5627fe4a95af544c4db1b250a263452128dc9cab`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.5 MB (3472886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b80aecb29fcddae2ca64d4c31faa682b41b3206400c727d5eec25c7d83c8630`  
		Last Modified: Thu, 16 Mar 2023 02:02:54 GMT  
		Size: 39.3 MB (39284857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277c8fbd8d44bf1475a44df6398ba9159c13423417cffb98f23824dca61b4a1d`  
		Last Modified: Thu, 16 Mar 2023 02:03:19 GMT  
		Size: 148.5 MB (148497878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-curl`

```console
$ docker pull buildpack-deps@sha256:1950ad34a10c685de875a9d2f586a239612590e033635f7ca3b07cd333c35d88
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
$ docker pull buildpack-deps@sha256:e1f00c6daf4cd328bbef9c52e6c60f18a47e5b716ef5a5d78542c90635025d20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37780234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb7e40d800141c3758097d639c8f71da7d755a34a9ce59dabba14aac2a540ee`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:29:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:29:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7490ba7e16ba382ca21015280e2ee6dad31879a1f043029e350a8e429770f36`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.8 MB (3788671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeb23ea57c359eecf9e21c40ddb69f738e9121008fd4956d733ba66d3b7eb38`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.6 MB (3561600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d14e02d71154d77fa15e8fe99c09399a29cf9cd6a168b06bf6cfdc6cbdd98960
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34279939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:831a4c6176514fb8d4452ddac355efa1a3da26e98087da273d6c3bcc34ba38e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:51:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:51:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d54aa809ca004a01d3a10bf7017a1fb216f185fd9d0f210f1bc9512298c1`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.5 MB (3540124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caec72904127d7cb95dfd39a3f311865b026d929e1440427ec21122be6e15db3`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.7 MB (3714418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fa825f78772b21eb6d058d2d80e48ded564c870a66ec077b8219225d6f515c2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35684245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd233dec7831ce72a921837b590af2d1f8f8d87f1b119fae78edba2ea730316`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:08:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aef66b301cbfe4ff1bb09357ccf381140239a236438d27a992d076491a3a066`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.8 MB (3760501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693278d975de74bdcb529fd46771b1335b9501b8f479a3c8128b69375f7945a8`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.5 MB (3536190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:057ed8d3115324cc3a7cbde4dad9bc42768a3cfeeb98aa5a2342d57a704ea2b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44208542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d825634c6ab1942263dbe9f71d6b27d39b833fb4013c32ad433760b35351762d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda6a81b65d142865ef5dbb2df2e98c084dc995272e55f804a36f283c6f9cc0a`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.3 MB (4262063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ead6720a64b98a3aff60731463b608c0b67ecd6e1da5fdea16027f2602fed35`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.2 MB (4234751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b22525cdcb82e2ef5355054b43872f265a7e983b5de76a9606921cde9d74b610
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35913329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a514140debee8dd2b4218d8d1975fc7b1e4623707f2083cffa6cdbd3f7e11228`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:49:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfb18fcfcf98f525d6770606600d80d5413262ce3575995b49064988c1bd147`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.8 MB (3792844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072af6d5dacbd70c88a5e91a5627fe4a95af544c4db1b250a263452128dc9cab`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.5 MB (3472886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-scm`

```console
$ docker pull buildpack-deps@sha256:79b0f9319ebb640493eaf8539641f9fc67a08f10ec5fc2f8a7d9a447fd786055
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
$ docker pull buildpack-deps@sha256:f34fd3d1a17609e88da35bc2a959ddd09a4cff838e251132a6a4551b7f710a8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77133144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e9805e59e9e583a30a563cbac116296ba8acf152f10fabcbecc2d3f99f8b6ab`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:29:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:29:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:29:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7490ba7e16ba382ca21015280e2ee6dad31879a1f043029e350a8e429770f36`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.8 MB (3788671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeb23ea57c359eecf9e21c40ddb69f738e9121008fd4956d733ba66d3b7eb38`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.6 MB (3561600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c00a0ea05e6a2089233e7238bbed0ffbf7b2655f03195967e2083ee623899`  
		Last Modified: Thu, 16 Mar 2023 05:43:30 GMT  
		Size: 39.4 MB (39352910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8249c9a5f7475ad02f242ade08a27052609481d8cd35ae4089fa7ecb14295c45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76188259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b7c6edcb5acd77a3e2b70af5afcda9bef5dcb2ee9c21e24297ee96426322b6e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:51:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:51:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:52:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d54aa809ca004a01d3a10bf7017a1fb216f185fd9d0f210f1bc9512298c1`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.5 MB (3540124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caec72904127d7cb95dfd39a3f311865b026d929e1440427ec21122be6e15db3`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.7 MB (3714418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b259dc20995aa828e48008def151ea3da6891615621976f66dc6b63fdbda38a`  
		Last Modified: Thu, 16 Mar 2023 04:09:57 GMT  
		Size: 41.9 MB (41908320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6857aefe9fc47abf0d2d28e21e046b63e6be875de53f2b1fd49dea88192e4560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74927866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9591d5aa5d0b25f21dfa798fa26b330206f083d8ca36701124b4a875b6c2c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:08:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:08:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aef66b301cbfe4ff1bb09357ccf381140239a236438d27a992d076491a3a066`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.8 MB (3760501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693278d975de74bdcb529fd46771b1335b9501b8f479a3c8128b69375f7945a8`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.5 MB (3536190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfc2e7bfd914b57fdeae1d187ca7a12534443f9e2a6142287dab73c0296ade8`  
		Last Modified: Thu, 16 Mar 2023 04:23:36 GMT  
		Size: 39.2 MB (39243621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d8da9e38d3c74aa25f5da85d9e692795099198656dfb38ba3058d5cc1c3284d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87976993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a899652169ee26f65829047e0799b9409330896911f49369b3b425b1315c02b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:24:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda6a81b65d142865ef5dbb2df2e98c084dc995272e55f804a36f283c6f9cc0a`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.3 MB (4262063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ead6720a64b98a3aff60731463b608c0b67ecd6e1da5fdea16027f2602fed35`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.2 MB (4234751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d902f277ddd72c79a705e87198d386aa6f00888bd94535ac236140f709bbdce`  
		Last Modified: Thu, 16 Mar 2023 03:50:57 GMT  
		Size: 43.8 MB (43768451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9b906aa81cc60290a664f0ff6bcb0f491cac7dd31f6cc7fbb73f4f2823d84ca0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75198186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:accf40ea7a4019526a1b76f2c48458f738926fa6bb6f285ca24c9c03b98771ed`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:49:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:50:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfb18fcfcf98f525d6770606600d80d5413262ce3575995b49064988c1bd147`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.8 MB (3792844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072af6d5dacbd70c88a5e91a5627fe4a95af544c4db1b250a263452128dc9cab`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.5 MB (3472886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b80aecb29fcddae2ca64d4c31faa682b41b3206400c727d5eec25c7d83c8630`  
		Last Modified: Thu, 16 Mar 2023 02:02:54 GMT  
		Size: 39.3 MB (39284857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10`

```console
$ docker pull buildpack-deps@sha256:175fb2896f655cccf6e13731e9e6d786c9c69630240717433c43d615958e67a3
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
$ docker pull buildpack-deps@sha256:6e3f3abbace0fcfb2e2393b134bb14479e39d5f78d9cfb25875150cbdcee2887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.8 MB (258751145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab725b6129919899348d2631b8bccdf236f9217de9abad4c65d0db0e544d4cd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:05 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:07 GMT
ADD file:3492508b382c909e968c4d8467b9acbd5f61ed6ca69c8a47241f930d90de7158 in / 
# Wed, 08 Mar 2023 05:58:07 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:33:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:33:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:34:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:36:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17a407a0ba4a4df07961f83dc5f45a6167aef7c4f6ca31fb67cb40abd601132d`  
		Last Modified: Thu, 16 Mar 2023 05:44:13 GMT  
		Size: 27.5 MB (27482092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3ce1e417f7729d7a549758b735166f99e55a7991459164e9a2cdee45bf49a4`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 6.8 MB (6770607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7f86ef9e483dabe62f207ba172ab1901264fcb5d62bd81ef5221c8ce9d67b3`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 3.6 MB (3635351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c5edfb2bc00433326244b5dd4da0315012e82e1b065c452afd8f40148f3180`  
		Last Modified: Thu, 16 Mar 2023 05:44:28 GMT  
		Size: 39.7 MB (39740353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6dbdd9f6c26e43b8b352fa3493515965ff36d7b264eb1458b635d095f086e`  
		Last Modified: Thu, 16 Mar 2023 05:45:00 GMT  
		Size: 181.1 MB (181122742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:962f9fa1a90ddfb86df762aa441ae2acbadf5a937ad2d29897e0eecae5e45c79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221867223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c52237c7765716061da64dd0c0e9e6c1a561f72d56a75d92470700609eb300b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:55:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:55:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:55:49 GMT
ADD file:827330b6c59e67c5d2edd3ceb3492b97865b15f9246f14710f478d12e94d2048 in / 
# Wed, 08 Mar 2023 05:55:49 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:56:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:57:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6408fcff70bde57e1c23e7502a9476939cc569e2eff3e9e9adca350cb5b4dac1`  
		Last Modified: Thu, 16 Mar 2023 04:10:41 GMT  
		Size: 25.9 MB (25890803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467248c617f5da80617561605e184647a03bc6ee0731094ea5fa1a10a9d97d12`  
		Last Modified: Thu, 16 Mar 2023 04:10:38 GMT  
		Size: 5.9 MB (5941308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084ed064758ff6efc72c5bfa16404dd5e5a7196c6704c9bfce54fffbe511f026`  
		Last Modified: Thu, 16 Mar 2023 04:10:37 GMT  
		Size: 3.8 MB (3801366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4d5295b37133c15e99cf4caa18ed1036eb41e583b687ff4e31eeb39287307d`  
		Last Modified: Thu, 16 Mar 2023 04:10:58 GMT  
		Size: 42.6 MB (42608451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b2ee1d700f51191bf1f9fda529c4cc2b75e353b7a936061fd2fe96c9f78678`  
		Last Modified: Thu, 16 Mar 2023 04:11:28 GMT  
		Size: 143.6 MB (143625295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:146ce1a60825f205a892808cd7a290d6b1a6e5898ad0d9210c66123d35dfe859
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.7 MB (246723891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2280a8119a9d7647830181ac7ce5e7c0e62f3a61d806d7003efd469a9f943063`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:57:57 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:57:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:57:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:57:58 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:57:59 GMT
ADD file:884e00dc91bf6d392fa3d117913cc2534177128322d89137bfb8b2734bc38579 in / 
# Wed, 08 Mar 2023 05:58:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:12:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:16:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:254a784e837e29e485a63351d1a7aba22a34cad2c55e16264bd25ec0add89463`  
		Last Modified: Thu, 16 Mar 2023 04:24:12 GMT  
		Size: 26.7 MB (26703428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5262eba6308f5bd6759d8fe45a1d30f1c39e36af3ffc10b11c84e335e3cf5`  
		Last Modified: Thu, 16 Mar 2023 04:24:10 GMT  
		Size: 6.6 MB (6600337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d93a07df4f2da69d3c85f944e8fa42f4e401cfb09edbff605d5863469a8c37`  
		Last Modified: Thu, 16 Mar 2023 04:24:09 GMT  
		Size: 3.6 MB (3604205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c46f9dfcefdff9c3932f840ec8ab4bf6808e7f4ade97eaf2a7ff68143dc8ac6`  
		Last Modified: Thu, 16 Mar 2023 04:24:25 GMT  
		Size: 39.5 MB (39516410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84953c5033e8f35541798119d0992d31f9b11c41d8790751581f9da4f03c7ff9`  
		Last Modified: Thu, 16 Mar 2023 04:24:51 GMT  
		Size: 170.3 MB (170299511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:06669921677d024d21c8b5bf374e4c76980db68187ef23ed12b774f09cc2e817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281308399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d473e407ad7791542b97cc0a0c2d858cd32beea41851e3dd56e8bdba1362ef37`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:03 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:06 GMT
ADD file:583061e8201c03de4747860e734200b6c35b449443a1382ad8e8efc6f7e9ea13 in / 
# Wed, 08 Mar 2023 05:58:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:30:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:31:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:36:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ec1f8fff860753bb5de879722c39643b2fecee25466efe51120479c4cd7647f`  
		Last Modified: Thu, 16 Mar 2023 03:52:17 GMT  
		Size: 32.1 MB (32098861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00fc14ce944c08bb40e1940367da097dd6113e4621903eedbeb83cf9caea6cc`  
		Last Modified: Thu, 16 Mar 2023 03:52:08 GMT  
		Size: 7.7 MB (7748081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75e7525a0f6794b3368a8aecf0b1c8c88ab38a7de79a51f2cc03b69581df2f`  
		Last Modified: Thu, 16 Mar 2023 03:52:07 GMT  
		Size: 4.4 MB (4362802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181a3a7eb1466bfe41561019eef321a775ae9583da803da64216210ccba3f91d`  
		Last Modified: Thu, 16 Mar 2023 03:52:39 GMT  
		Size: 44.1 MB (44142002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c199734d8e3b9bc7a3c36814098b8d531785794c938276dc46411ec36cdb0d`  
		Last Modified: Thu, 16 Mar 2023 03:53:36 GMT  
		Size: 193.0 MB (192956653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5b34f6d4e61a65640b7b2c4ebfea0b28a3aa10a05e87019ea523c5d3597d47a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228629856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597b8cfc1db04a45533b44e8f28ad50b5fc7e01b8423c09757ed1daeb251d21c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 06:11:04 GMT
ARG RELEASE
# Wed, 08 Mar 2023 06:11:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 06:11:06 GMT
ADD file:974d67ca1d5bcaacbc707820609d36af0d7ed3ff7179a702a4aa56dcc43f79f3 in / 
# Wed, 08 Mar 2023 06:11:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:53:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:53:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:55:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e94c7036e7dc9a2d6666b2f4fc00019c0540bd3edd16e54289a9d6b7134b349`  
		Last Modified: Thu, 16 Mar 2023 02:03:35 GMT  
		Size: 26.0 MB (26029370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc60d216fdfa5dd36e7941c80e0ea9d1b8c692a8c067ad512585b6ae40bd6e99`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 6.5 MB (6461878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c257c035538e42c9fb24b73041a70d92b99378d720c80bc418d8ed7900e2d15c`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 3.6 MB (3625230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2543f565e0a12ed697a188c8d0c2e00c8788a6dee791dbf852c2b335985834`  
		Last Modified: Thu, 16 Mar 2023 02:03:48 GMT  
		Size: 39.6 MB (39559711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a414ee64d952ecb156be9cb912b41983739a5bd309bf9db2c7cc6cba5ffdc2`  
		Last Modified: Thu, 16 Mar 2023 02:04:16 GMT  
		Size: 153.0 MB (152953667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-curl`

```console
$ docker pull buildpack-deps@sha256:82f90458af310619116662064c4a1bfd08da721e3ac46a1452047c268517fde0
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
$ docker pull buildpack-deps@sha256:4a0ea70e27ab3ee9d260740e1e11ef06f009589299eaa372b3313a5d617480bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37888050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83a06332258b828506b4757d4fa816eb9f29440d4e56282a9a38e120f33cd5c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:05 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:07 GMT
ADD file:3492508b382c909e968c4d8467b9acbd5f61ed6ca69c8a47241f930d90de7158 in / 
# Wed, 08 Mar 2023 05:58:07 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:33:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:33:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:17a407a0ba4a4df07961f83dc5f45a6167aef7c4f6ca31fb67cb40abd601132d`  
		Last Modified: Thu, 16 Mar 2023 05:44:13 GMT  
		Size: 27.5 MB (27482092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3ce1e417f7729d7a549758b735166f99e55a7991459164e9a2cdee45bf49a4`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 6.8 MB (6770607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7f86ef9e483dabe62f207ba172ab1901264fcb5d62bd81ef5221c8ce9d67b3`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 3.6 MB (3635351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4af883c5eab3c2380a46236ca3ca95f3048243965b2e897814c48e8260dfa2c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35633477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094d55cec9f8dc3d95b8ee21b11560284d162a4571f93b0b44109e9fe8e3d0cc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:55:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:55:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:55:49 GMT
ADD file:827330b6c59e67c5d2edd3ceb3492b97865b15f9246f14710f478d12e94d2048 in / 
# Wed, 08 Mar 2023 05:55:49 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:56:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6408fcff70bde57e1c23e7502a9476939cc569e2eff3e9e9adca350cb5b4dac1`  
		Last Modified: Thu, 16 Mar 2023 04:10:41 GMT  
		Size: 25.9 MB (25890803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467248c617f5da80617561605e184647a03bc6ee0731094ea5fa1a10a9d97d12`  
		Last Modified: Thu, 16 Mar 2023 04:10:38 GMT  
		Size: 5.9 MB (5941308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084ed064758ff6efc72c5bfa16404dd5e5a7196c6704c9bfce54fffbe511f026`  
		Last Modified: Thu, 16 Mar 2023 04:10:37 GMT  
		Size: 3.8 MB (3801366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f7410e86839d94189da0421368263daad23e4532602532ebebb243959a6589bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36907970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11201af935ca582771cd9c1d5a25562f6956d2d83b5561f776ff20235996f3a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:57:57 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:57:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:57:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:57:58 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:57:59 GMT
ADD file:884e00dc91bf6d392fa3d117913cc2534177128322d89137bfb8b2734bc38579 in / 
# Wed, 08 Mar 2023 05:58:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:12:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:254a784e837e29e485a63351d1a7aba22a34cad2c55e16264bd25ec0add89463`  
		Last Modified: Thu, 16 Mar 2023 04:24:12 GMT  
		Size: 26.7 MB (26703428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5262eba6308f5bd6759d8fe45a1d30f1c39e36af3ffc10b11c84e335e3cf5`  
		Last Modified: Thu, 16 Mar 2023 04:24:10 GMT  
		Size: 6.6 MB (6600337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d93a07df4f2da69d3c85f944e8fa42f4e401cfb09edbff605d5863469a8c37`  
		Last Modified: Thu, 16 Mar 2023 04:24:09 GMT  
		Size: 3.6 MB (3604205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6760f29c9bdcdc308fcf3afb3ca98c719d1c0c3e8c5a5bea33cc33c3db2550d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44209744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14fbb219e4d625d407f193f60f7c075595d470a92f731343a064f26b3a6c72a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:03 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:06 GMT
ADD file:583061e8201c03de4747860e734200b6c35b449443a1382ad8e8efc6f7e9ea13 in / 
# Wed, 08 Mar 2023 05:58:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:30:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6ec1f8fff860753bb5de879722c39643b2fecee25466efe51120479c4cd7647f`  
		Last Modified: Thu, 16 Mar 2023 03:52:17 GMT  
		Size: 32.1 MB (32098861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00fc14ce944c08bb40e1940367da097dd6113e4621903eedbeb83cf9caea6cc`  
		Last Modified: Thu, 16 Mar 2023 03:52:08 GMT  
		Size: 7.7 MB (7748081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75e7525a0f6794b3368a8aecf0b1c8c88ab38a7de79a51f2cc03b69581df2f`  
		Last Modified: Thu, 16 Mar 2023 03:52:07 GMT  
		Size: 4.4 MB (4362802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d2366f9c8542e47115c50c026f6cf9ccda7aaf6b859307b5ca9f1f1c0cf8a50b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36116478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ee7ee58323c7f6349967f769687f47de069565561ee8264351d32a8d0ecd22e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 06:11:04 GMT
ARG RELEASE
# Wed, 08 Mar 2023 06:11:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 06:11:06 GMT
ADD file:974d67ca1d5bcaacbc707820609d36af0d7ed3ff7179a702a4aa56dcc43f79f3 in / 
# Wed, 08 Mar 2023 06:11:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:53:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3e94c7036e7dc9a2d6666b2f4fc00019c0540bd3edd16e54289a9d6b7134b349`  
		Last Modified: Thu, 16 Mar 2023 02:03:35 GMT  
		Size: 26.0 MB (26029370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc60d216fdfa5dd36e7941c80e0ea9d1b8c692a8c067ad512585b6ae40bd6e99`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 6.5 MB (6461878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c257c035538e42c9fb24b73041a70d92b99378d720c80bc418d8ed7900e2d15c`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 3.6 MB (3625230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-scm`

```console
$ docker pull buildpack-deps@sha256:aa76817af3e5497173c1e3d3e67c0365b99897e5b1e315ac4910b2920c424f95
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
$ docker pull buildpack-deps@sha256:e6378630b29880479224ed0c4d5c760022695b18656bb1a04f7ee4c840c365fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77628403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4098822eb5aa2de33de31a2e39c977e7c97b73cb3d43bf8ad263135afdc338a7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:05 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:07 GMT
ADD file:3492508b382c909e968c4d8467b9acbd5f61ed6ca69c8a47241f930d90de7158 in / 
# Wed, 08 Mar 2023 05:58:07 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:33:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:33:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:34:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17a407a0ba4a4df07961f83dc5f45a6167aef7c4f6ca31fb67cb40abd601132d`  
		Last Modified: Thu, 16 Mar 2023 05:44:13 GMT  
		Size: 27.5 MB (27482092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3ce1e417f7729d7a549758b735166f99e55a7991459164e9a2cdee45bf49a4`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 6.8 MB (6770607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7f86ef9e483dabe62f207ba172ab1901264fcb5d62bd81ef5221c8ce9d67b3`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 3.6 MB (3635351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c5edfb2bc00433326244b5dd4da0315012e82e1b065c452afd8f40148f3180`  
		Last Modified: Thu, 16 Mar 2023 05:44:28 GMT  
		Size: 39.7 MB (39740353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:90515c216502433efbdc090e03b1210bf49d905412b2c6c1d721854daf004502
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78241928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de12f85f2fcdabf5af043eb805c6ed21fdfbdfac456a33d4e17ae057800a5a0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:55:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:55:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:55:49 GMT
ADD file:827330b6c59e67c5d2edd3ceb3492b97865b15f9246f14710f478d12e94d2048 in / 
# Wed, 08 Mar 2023 05:55:49 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:56:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:57:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6408fcff70bde57e1c23e7502a9476939cc569e2eff3e9e9adca350cb5b4dac1`  
		Last Modified: Thu, 16 Mar 2023 04:10:41 GMT  
		Size: 25.9 MB (25890803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467248c617f5da80617561605e184647a03bc6ee0731094ea5fa1a10a9d97d12`  
		Last Modified: Thu, 16 Mar 2023 04:10:38 GMT  
		Size: 5.9 MB (5941308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084ed064758ff6efc72c5bfa16404dd5e5a7196c6704c9bfce54fffbe511f026`  
		Last Modified: Thu, 16 Mar 2023 04:10:37 GMT  
		Size: 3.8 MB (3801366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4d5295b37133c15e99cf4caa18ed1036eb41e583b687ff4e31eeb39287307d`  
		Last Modified: Thu, 16 Mar 2023 04:10:58 GMT  
		Size: 42.6 MB (42608451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7ea350ea72f5dc34447ad0ad32230ca304a8954c691d5e2219aeb1c3d33dd977
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76424380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc47c377e953ab11b6623e2d24bbe50bdb550a956e97f3bf19941a13663ae09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:57:57 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:57:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:57:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:57:58 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:57:59 GMT
ADD file:884e00dc91bf6d392fa3d117913cc2534177128322d89137bfb8b2734bc38579 in / 
# Wed, 08 Mar 2023 05:58:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:12:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:254a784e837e29e485a63351d1a7aba22a34cad2c55e16264bd25ec0add89463`  
		Last Modified: Thu, 16 Mar 2023 04:24:12 GMT  
		Size: 26.7 MB (26703428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5262eba6308f5bd6759d8fe45a1d30f1c39e36af3ffc10b11c84e335e3cf5`  
		Last Modified: Thu, 16 Mar 2023 04:24:10 GMT  
		Size: 6.6 MB (6600337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d93a07df4f2da69d3c85f944e8fa42f4e401cfb09edbff605d5863469a8c37`  
		Last Modified: Thu, 16 Mar 2023 04:24:09 GMT  
		Size: 3.6 MB (3604205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c46f9dfcefdff9c3932f840ec8ab4bf6808e7f4ade97eaf2a7ff68143dc8ac6`  
		Last Modified: Thu, 16 Mar 2023 04:24:25 GMT  
		Size: 39.5 MB (39516410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:47814ff7d3d0680f98234b1b77e52c20623de4ea381d7d64b45058c0420e3b98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88351746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6520324913b2522ab60f497720b420e064788b9c36489fc9db9df6e7ccd90d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:03 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:06 GMT
ADD file:583061e8201c03de4747860e734200b6c35b449443a1382ad8e8efc6f7e9ea13 in / 
# Wed, 08 Mar 2023 05:58:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:30:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:31:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ec1f8fff860753bb5de879722c39643b2fecee25466efe51120479c4cd7647f`  
		Last Modified: Thu, 16 Mar 2023 03:52:17 GMT  
		Size: 32.1 MB (32098861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00fc14ce944c08bb40e1940367da097dd6113e4621903eedbeb83cf9caea6cc`  
		Last Modified: Thu, 16 Mar 2023 03:52:08 GMT  
		Size: 7.7 MB (7748081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75e7525a0f6794b3368a8aecf0b1c8c88ab38a7de79a51f2cc03b69581df2f`  
		Last Modified: Thu, 16 Mar 2023 03:52:07 GMT  
		Size: 4.4 MB (4362802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181a3a7eb1466bfe41561019eef321a775ae9583da803da64216210ccba3f91d`  
		Last Modified: Thu, 16 Mar 2023 03:52:39 GMT  
		Size: 44.1 MB (44142002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9bbf357cfc90c5b3effb70b70ec060ca6b1b3e1a6867604c88d94fbbbe77399d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75676189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e90e10986384324d54a15fec854faff368bcba346fce3c6b1ff80c08f0998a0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 06:11:04 GMT
ARG RELEASE
# Wed, 08 Mar 2023 06:11:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 06:11:06 GMT
ADD file:974d67ca1d5bcaacbc707820609d36af0d7ed3ff7179a702a4aa56dcc43f79f3 in / 
# Wed, 08 Mar 2023 06:11:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:53:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:53:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e94c7036e7dc9a2d6666b2f4fc00019c0540bd3edd16e54289a9d6b7134b349`  
		Last Modified: Thu, 16 Mar 2023 02:03:35 GMT  
		Size: 26.0 MB (26029370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc60d216fdfa5dd36e7941c80e0ea9d1b8c692a8c067ad512585b6ae40bd6e99`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 6.5 MB (6461878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c257c035538e42c9fb24b73041a70d92b99378d720c80bc418d8ed7900e2d15c`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 3.6 MB (3625230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2543f565e0a12ed697a188c8d0c2e00c8788a6dee791dbf852c2b335985834`  
		Last Modified: Thu, 16 Mar 2023 02:03:48 GMT  
		Size: 39.6 MB (39559711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04`

```console
$ docker pull buildpack-deps@sha256:560e0088301609081b9f373dec446d2e62c1a2d6649abeb3fcc344e1e47bf596
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
$ docker pull buildpack-deps@sha256:287222a734407093da8bd5d1aa36fbb68ec0bedd34f5d3d6c953369ee20930b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.8 MB (265813027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81d6e1c88be1ef8bc7e4711555c9bc2801e4ae6d1ba36047cc5ccfc957d722a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:37:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:37:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:40:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbd9104be902889dc21019a0f5023f798f3d4659871b7eff4e60ea6f1496df08`  
		Last Modified: Thu, 16 Mar 2023 05:45:13 GMT  
		Size: 27.5 MB (27533123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926546ac77ef389dea10f2f48a9435499b9fd85ce007f054787873fba3ba820`  
		Last Modified: Thu, 16 Mar 2023 05:45:10 GMT  
		Size: 6.7 MB (6653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e02fdac0efdc0f5d71c45d6ab71b8cf2421156adfbe3dd6673c198b60f5e696`  
		Last Modified: Thu, 16 Mar 2023 05:45:09 GMT  
		Size: 3.7 MB (3689653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57775961ac4b5f4df9ba21c9a454eec60eced52106a9c3c6480abe04fd31e975`  
		Last Modified: Thu, 16 Mar 2023 05:45:29 GMT  
		Size: 44.3 MB (44251085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d411862c594e5099f7d047ca155efc294f71792fc959ab9aa3e07e449b5f29ae`  
		Last Modified: Thu, 16 Mar 2023 05:46:00 GMT  
		Size: 183.7 MB (183685294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:155908323c4e07137e4866c58870f6590c6de3ca0b3cbd687cd8ec6672e62b57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.4 MB (230430758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86991c1a884508bddd7bad77896595630d8d44bf3cfe5080600a260675f86e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:01:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:04:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2e2ff6a76c080ab34fadea2f47efdf4e1606b1482ed2e4597e51810a467b28a`  
		Last Modified: Thu, 16 Mar 2023 04:11:42 GMT  
		Size: 25.4 MB (25359548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003fc5922aae3f4274356fca42181568c983c95440b266598d0a8b3307f981b3`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 5.8 MB (5819049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f573392ff6ba3d538b9dd78eaac78c3a48a8719f2c3a366e5031c24433553af7`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 3.9 MB (3850947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e5edf4553807d09a5e079189ad8abe94fa20ac8d3b91a1fdee74ffbbfc465a`  
		Last Modified: Thu, 16 Mar 2023 04:12:00 GMT  
		Size: 48.3 MB (48335132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4f27e394d3d3e059ce90e3503f32ac8d096f2652745ce86e56fa4bb4b25ab5`  
		Last Modified: Thu, 16 Mar 2023 04:12:30 GMT  
		Size: 147.1 MB (147066082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e9b21ae0c7c9575c3bdbcc4e38e37afc2bf155d4304484b260fc63b65decc3d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.0 MB (255963478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c30df20c0e7ce6c6b1e087b68175313ed2ed3632a7707c2078dd03a949b607b9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:17:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:20:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bd94ab779df0c538759342d8eef230b315e98979bcac4604e94fb874397461b`  
		Last Modified: Thu, 16 Mar 2023 04:25:04 GMT  
		Size: 26.9 MB (26945660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df8402fa00c99b6f8233d0c6452e59cfe2742b9b2c9f44a504aaa45a0516cd3`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 6.5 MB (6484575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa45039d5b2736a9624493cbbbf9200c134de7ddb8696ce87c68dad417e12f4`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 3.6 MB (3648517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5195e2054b68f924f77b2db71706b518fdc87c9c6f3d900adad8e6eec601fb`  
		Last Modified: Thu, 16 Mar 2023 04:25:18 GMT  
		Size: 44.1 MB (44054619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afa7d18844d07a4d0a59be44ee5dfea5fae8e0ed488bf7cd0a5c87e6b4ab3cc`  
		Last Modified: Thu, 16 Mar 2023 04:25:44 GMT  
		Size: 174.8 MB (174830107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3f87acc02cf05e895c5cdca40f10af0846f6beef7f7d0d413e64336ebe514f6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.1 MB (290142434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e375ebe6881fcb8e14ab34fd4f73359da22f443ac83cbcc5448356866acd3d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:38:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:45:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c13086b2cdc797d6ae8ae49964c3990abf6b026e7f643db84a65b7f084366f08`  
		Last Modified: Thu, 16 Mar 2023 03:53:59 GMT  
		Size: 32.0 MB (31970021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb512502a00877ef190b1815b85439c23acfccd37a17990ec798b2bea4e21069`  
		Last Modified: Thu, 16 Mar 2023 03:53:49 GMT  
		Size: 7.6 MB (7632987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c926d392a0489ac95be096f121aa71205ac931a151fc7c4564fc57444078c1fd`  
		Last Modified: Thu, 16 Mar 2023 03:53:48 GMT  
		Size: 4.4 MB (4408510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2857f7a011d6755514a89958db979d33059396ce8ea89c6552489bef9035282b`  
		Last Modified: Thu, 16 Mar 2023 03:54:23 GMT  
		Size: 48.9 MB (48926165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0775c8324947137c1777a6bb6e389e8f1ae322fbca889c73a00a2c57a91e8a1b`  
		Last Modified: Thu, 16 Mar 2023 03:55:20 GMT  
		Size: 197.2 MB (197204751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:45e836f4bee45e343d3d20e203bbab10f5eaad7b0934027e11c1be55ebca27a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.1 MB (237149064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1505c6374943ba67de8bcae872902c1bc61e99bc98f23769939466c5ae877c8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:56:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:58:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:413472b726c3207e3bafacfb65a3db7c0c8692445502e7d2ad70b1585e534841`  
		Last Modified: Thu, 16 Mar 2023 02:04:26 GMT  
		Size: 26.2 MB (26162786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef961f5d29313e42026cc5111865e26af7782293f64f5eca11172750d63f804`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 6.3 MB (6335431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b09797bd3d78e6694a4d023216c32e3665a913d5dcd639c47a00674aa9bd5f`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 3.7 MB (3674242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ac168459f3e70bf00dbc80bd6a3cca0005c0e36d3ecf7fd0ae2395921677c5`  
		Last Modified: Thu, 16 Mar 2023 02:04:40 GMT  
		Size: 44.1 MB (44081685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4a0858837f3c6eeaa709f1bf472664e892f57a6f75cf799ebf86f41ac8b732`  
		Last Modified: Thu, 16 Mar 2023 02:05:08 GMT  
		Size: 156.9 MB (156894920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-curl`

```console
$ docker pull buildpack-deps@sha256:3c92603c3c4cfdf54434d189f6ea4b878e2f864e9756808938df4b7b261813e9
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
$ docker pull buildpack-deps@sha256:88cc8d8450e2140b02c76ab91eb047c03405b2b54809c53dd5850a6b766b84cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37876648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9541ffb4362b8ed33942bce7957eb33fc7b9063e91e93e93d47fecd801deb76d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:37:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dbd9104be902889dc21019a0f5023f798f3d4659871b7eff4e60ea6f1496df08`  
		Last Modified: Thu, 16 Mar 2023 05:45:13 GMT  
		Size: 27.5 MB (27533123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926546ac77ef389dea10f2f48a9435499b9fd85ce007f054787873fba3ba820`  
		Last Modified: Thu, 16 Mar 2023 05:45:10 GMT  
		Size: 6.7 MB (6653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e02fdac0efdc0f5d71c45d6ab71b8cf2421156adfbe3dd6673c198b60f5e696`  
		Last Modified: Thu, 16 Mar 2023 05:45:09 GMT  
		Size: 3.7 MB (3689653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:614fca6a30bbfe066856c014a147fa326ec793122ed0e9624732cb670ce2e85f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35029544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24b29040dc3a4ce8a013430cf3b9e64653cb7a9d0e2b07e0b725dc6c71041281`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:01:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f2e2ff6a76c080ab34fadea2f47efdf4e1606b1482ed2e4597e51810a467b28a`  
		Last Modified: Thu, 16 Mar 2023 04:11:42 GMT  
		Size: 25.4 MB (25359548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003fc5922aae3f4274356fca42181568c983c95440b266598d0a8b3307f981b3`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 5.8 MB (5819049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f573392ff6ba3d538b9dd78eaac78c3a48a8719f2c3a366e5031c24433553af7`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 3.9 MB (3850947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9bfb20d764824394d6318a1e3ea3ca8dc572a7fc5d2174fe2057b50bb244e9e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37078752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629f7f7e4b34d738f867a79f3b2bb90546a32a19fe6bb8ad427d42c1d6153cc7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:17:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5bd94ab779df0c538759342d8eef230b315e98979bcac4604e94fb874397461b`  
		Last Modified: Thu, 16 Mar 2023 04:25:04 GMT  
		Size: 26.9 MB (26945660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df8402fa00c99b6f8233d0c6452e59cfe2742b9b2c9f44a504aaa45a0516cd3`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 6.5 MB (6484575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa45039d5b2736a9624493cbbbf9200c134de7ddb8696ce87c68dad417e12f4`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 3.6 MB (3648517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a5df0b199035bf5963b942dadf1b32fc61120f2d0605e2a9fad2cabc1839a7b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44011518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1611814033075adc80702cce1f81c5df91554f4e75044921f9b25158d1cbe296`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:38:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c13086b2cdc797d6ae8ae49964c3990abf6b026e7f643db84a65b7f084366f08`  
		Last Modified: Thu, 16 Mar 2023 03:53:59 GMT  
		Size: 32.0 MB (31970021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb512502a00877ef190b1815b85439c23acfccd37a17990ec798b2bea4e21069`  
		Last Modified: Thu, 16 Mar 2023 03:53:49 GMT  
		Size: 7.6 MB (7632987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c926d392a0489ac95be096f121aa71205ac931a151fc7c4564fc57444078c1fd`  
		Last Modified: Thu, 16 Mar 2023 03:53:48 GMT  
		Size: 4.4 MB (4408510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7d87ab98ab8a33299dd743e4394ecfd4148bae746acec49a6fffefb7e01b57ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36172459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8450951ba16b57ce51376ee52be443e0ef4c01e6ab2e5b0789a6a004768c0358`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:413472b726c3207e3bafacfb65a3db7c0c8692445502e7d2ad70b1585e534841`  
		Last Modified: Thu, 16 Mar 2023 02:04:26 GMT  
		Size: 26.2 MB (26162786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef961f5d29313e42026cc5111865e26af7782293f64f5eca11172750d63f804`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 6.3 MB (6335431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b09797bd3d78e6694a4d023216c32e3665a913d5dcd639c47a00674aa9bd5f`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 3.7 MB (3674242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-scm`

```console
$ docker pull buildpack-deps@sha256:4e0401bf1ba398dfbd820acc7da7a7b48bebe090d46f525f29b42f1e54334bf7
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
$ docker pull buildpack-deps@sha256:8c474a27635a29ce1f6daffda32528a0aa48b6f589ecf88490b158f33a571f15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82127733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46a0d94344b399c5d7604309d08fcd4a61f68a8911fd92690bd5f4a46d9c8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:37:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:37:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbd9104be902889dc21019a0f5023f798f3d4659871b7eff4e60ea6f1496df08`  
		Last Modified: Thu, 16 Mar 2023 05:45:13 GMT  
		Size: 27.5 MB (27533123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926546ac77ef389dea10f2f48a9435499b9fd85ce007f054787873fba3ba820`  
		Last Modified: Thu, 16 Mar 2023 05:45:10 GMT  
		Size: 6.7 MB (6653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e02fdac0efdc0f5d71c45d6ab71b8cf2421156adfbe3dd6673c198b60f5e696`  
		Last Modified: Thu, 16 Mar 2023 05:45:09 GMT  
		Size: 3.7 MB (3689653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57775961ac4b5f4df9ba21c9a454eec60eced52106a9c3c6480abe04fd31e975`  
		Last Modified: Thu, 16 Mar 2023 05:45:29 GMT  
		Size: 44.3 MB (44251085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6b08244e2bc4db9fd4a22095b42d9044de738c27f0c4f78a9fd1303fb5e9459e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83364676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad34d38cd21a977e6a4b1485518ff8873988b314b13cb4796e11b2ed4ec4d693`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:01:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2e2ff6a76c080ab34fadea2f47efdf4e1606b1482ed2e4597e51810a467b28a`  
		Last Modified: Thu, 16 Mar 2023 04:11:42 GMT  
		Size: 25.4 MB (25359548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003fc5922aae3f4274356fca42181568c983c95440b266598d0a8b3307f981b3`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 5.8 MB (5819049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f573392ff6ba3d538b9dd78eaac78c3a48a8719f2c3a366e5031c24433553af7`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 3.9 MB (3850947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e5edf4553807d09a5e079189ad8abe94fa20ac8d3b91a1fdee74ffbbfc465a`  
		Last Modified: Thu, 16 Mar 2023 04:12:00 GMT  
		Size: 48.3 MB (48335132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7718090c669d397351860cb0345fd87226c3f44bfc63156d13b88ee8b6bb13c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81133371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:794f72335c8bb0cbfaa191b6c8873dca8c9aeca030e74c1f1e6e88e9df6cfe91`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:17:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bd94ab779df0c538759342d8eef230b315e98979bcac4604e94fb874397461b`  
		Last Modified: Thu, 16 Mar 2023 04:25:04 GMT  
		Size: 26.9 MB (26945660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df8402fa00c99b6f8233d0c6452e59cfe2742b9b2c9f44a504aaa45a0516cd3`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 6.5 MB (6484575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa45039d5b2736a9624493cbbbf9200c134de7ddb8696ce87c68dad417e12f4`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 3.6 MB (3648517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5195e2054b68f924f77b2db71706b518fdc87c9c6f3d900adad8e6eec601fb`  
		Last Modified: Thu, 16 Mar 2023 04:25:18 GMT  
		Size: 44.1 MB (44054619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:80776e57275eac4ab14959cc2eb0aa5c39dfbc1eac936218d2bd4714c32b6d34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92937683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86884dca514275133e923ec8f78e2785269d5ed21433f44077b1e44c33e5751b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:38:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c13086b2cdc797d6ae8ae49964c3990abf6b026e7f643db84a65b7f084366f08`  
		Last Modified: Thu, 16 Mar 2023 03:53:59 GMT  
		Size: 32.0 MB (31970021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb512502a00877ef190b1815b85439c23acfccd37a17990ec798b2bea4e21069`  
		Last Modified: Thu, 16 Mar 2023 03:53:49 GMT  
		Size: 7.6 MB (7632987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c926d392a0489ac95be096f121aa71205ac931a151fc7c4564fc57444078c1fd`  
		Last Modified: Thu, 16 Mar 2023 03:53:48 GMT  
		Size: 4.4 MB (4408510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2857f7a011d6755514a89958db979d33059396ce8ea89c6552489bef9035282b`  
		Last Modified: Thu, 16 Mar 2023 03:54:23 GMT  
		Size: 48.9 MB (48926165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:be8e1571ea2945b768f155c85a9fc4d617a62103e27b12291a1b9e88c5ae2f53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80254144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad371214c349f4a458439e817f999971228fed0bcf6aceaccbb08508cf9c8a0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:56:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:413472b726c3207e3bafacfb65a3db7c0c8692445502e7d2ad70b1585e534841`  
		Last Modified: Thu, 16 Mar 2023 02:04:26 GMT  
		Size: 26.2 MB (26162786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef961f5d29313e42026cc5111865e26af7782293f64f5eca11172750d63f804`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 6.3 MB (6335431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b09797bd3d78e6694a4d023216c32e3665a913d5dcd639c47a00674aa9bd5f`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 3.7 MB (3674242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ac168459f3e70bf00dbc80bd6a3cca0005c0e36d3ecf7fd0ae2395921677c5`  
		Last Modified: Thu, 16 Mar 2023 02:04:40 GMT  
		Size: 44.1 MB (44081685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:fb154449c96034e2ac28a113cfbc31b7da0e4a21387c397dec6b1deec6d89d73
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
$ docker pull buildpack-deps@sha256:b1da6a5f500b67fa28bbae2b90a8e9da4def283d1fb918b1d4db0c9cd86ec183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221417037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeecfa359fe257650879cc03de2c96ee1ab252d40eaf9467a855893ac7df28f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:21:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:21:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:24:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c78e6dac9cec3c01ca7687f8e0a53a4b5e9b04f4910729279be4204ce5360e`  
		Last Modified: Thu, 16 Mar 2023 05:41:29 GMT  
		Size: 6.6 MB (6617364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b18b892afad36455b3ae75f0ab2c1bc45822e03069f2667faa4bede3825be5`  
		Last Modified: Thu, 16 Mar 2023 05:41:28 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c57462ca1fd8565d56aa476a7fa497011a11c6f761194b368d2c722e146b20`  
		Last Modified: Thu, 16 Mar 2023 05:41:43 GMT  
		Size: 45.5 MB (45514749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f391d58903094b86c56fd169ec96c398321c3ccab4f8893113f4de938d003a`  
		Last Modified: Thu, 16 Mar 2023 05:42:10 GMT  
		Size: 139.5 MB (139548050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f740f07a329775404244fd36ca65500a61ecd79c38851ee6ce6408443fa9779
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189581013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb26767826b27bb17bc813102a23903c31d4ea475f341486310a77dd6e54d766`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:44:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:45:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:47:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2b71966fc2f22e1375423fb61221ed137cf5e7e8d202bfa403292ba600daab`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 5.7 MB (5681012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf04b4bbda07472ffbb83ab11cb71b6ff2c6bef9749979a8a3981f285c0f53`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 2.6 MB (2586979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3058bdcdd1b82bda414133ce433d46f98b5f56911e44f00ff6bd1de1c0a6caba`  
		Last Modified: Thu, 16 Mar 2023 04:08:04 GMT  
		Size: 40.7 MB (40713543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d88abc5604e52bcee192566d8fae426f1031f855abd4229bd8c43feeb2648d`  
		Last Modified: Thu, 16 Mar 2023 04:08:30 GMT  
		Size: 118.3 MB (118294105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2c9e464ea859a1b832272828463904e3f9c04bdebf0e7aa9cdc4c6c48481c85e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (206011203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b97289739597eaf439933630ebefa90822ac12cd90c8157a55e7b3f32763f4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:58:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:59:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:02:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc06fc1cf8ad0140062ec53dbc631cea853ddb72d7c0b353edd743b1dca4ceb`  
		Last Modified: Thu, 16 Mar 2023 04:21:50 GMT  
		Size: 6.1 MB (6057809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d0b4e623a1829e474acf7b4d21109a9f27c7d8c8bf12f163ffe645eed93ec`  
		Last Modified: Thu, 16 Mar 2023 04:21:49 GMT  
		Size: 2.8 MB (2790695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37de71f159d52bbc91be8b71a2d8862f89e2c137ac5d4e17c923aaa4fa5aa30`  
		Last Modified: Thu, 16 Mar 2023 04:22:03 GMT  
		Size: 43.3 MB (43311869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc13acad8ae8946317f508f7e0eda6de200ca13831f7433e58942f2466c21473`  
		Last Modified: Thu, 16 Mar 2023 04:22:25 GMT  
		Size: 130.1 MB (130116124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d189ba12fe145c64ea06852f5de7d0ab170ab04daca4c5effd4a4705cabb888e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218710648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc3d7329f212c3056b20a7f0084491a4e3d07e63c6848a789189f5137e2d75d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:19 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:21 GMT
ADD file:6cf3e34995c6c44762ed692b86a0442d981e9a69fa4288960047e505d75c0223 in / 
# Wed, 08 Mar 2023 03:13:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:57:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:00:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58af8b772f2ca9c63db81d620e48946c13c027ecd7ab2d9062d010ca2ed11f3`  
		Last Modified: Thu, 16 Mar 2023 01:54:42 GMT  
		Size: 27.2 MB (27164610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df9a7dbeea70a625098ba195b5c6a6046e010992d4b2616b74e5efca85ff0`  
		Last Modified: Thu, 16 Mar 2023 02:02:18 GMT  
		Size: 6.9 MB (6907798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9c7488bcb45de5faeb1bc3f4a19015817de4a09d3c762c619d48aa2855322e`  
		Last Modified: Thu, 16 Mar 2023 02:02:17 GMT  
		Size: 3.3 MB (3255693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54663dad9d7f237e7f0a0a533af683ae66d66098cdd57ea8f90fde4dd8897ffb`  
		Last Modified: Thu, 16 Mar 2023 02:02:38 GMT  
		Size: 47.1 MB (47095486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5e9e49852091a0f82ca614c93efb7802ff6bbabc0da2e14b9606920c072cb6`  
		Last Modified: Thu, 16 Mar 2023 02:03:15 GMT  
		Size: 134.3 MB (134287061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:093d533487c60b2c92363199f07f041884638f879f09c20c9aa303e056b1267c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246441203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcd83e221d1f7aaec4fdcb03d7776c2eadf8d9cf89c85eaba5ab7f7793f25ed`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:07:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:08:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:14:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e5cf4c1f014d5508f129bb3d2e36a3448b5d92b400a35d3051160723af42b4`  
		Last Modified: Thu, 16 Mar 2023 03:47:41 GMT  
		Size: 7.0 MB (7036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a259ed8117f57e3f76e8e31ddb857f6d36e8f1ac8131d38a456833aa7e0c20`  
		Last Modified: Thu, 16 Mar 2023 03:47:40 GMT  
		Size: 3.7 MB (3740612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409f528497ffaa0bc9ae78b8139359ddd38315caf439a39a670aaed487c6c06d`  
		Last Modified: Thu, 16 Mar 2023 03:48:07 GMT  
		Size: 53.7 MB (53736792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22095eabcbee3060dd218f09d76cf296a873b1a36d1d4f86794d105fe7e5ec5f`  
		Last Modified: Thu, 16 Mar 2023 03:48:53 GMT  
		Size: 151.5 MB (151484912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0c8e0a8e8c0a624863dcfee0278ed624183fd34de9612945d2db9d6842c229d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205782934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8557c42f5d0087a913e9c89b40998da81a7d55355bad38d52f6b3f7699f2681b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:23:29 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:23:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:23:31 GMT
ADD file:a6309e462d28398152cb726a11615118d79858da963b8c614772b87d87465967 in / 
# Wed, 08 Mar 2023 03:23:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:43:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:44:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:46:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3a2279f06ab19f0d57823e69b999f54a344e28bd9f955b4db9a5875c0caa543a`  
		Last Modified: Thu, 16 Mar 2023 02:01:03 GMT  
		Size: 25.4 MB (25370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37be097f66ed2ca5a62bf5e79eee23cbae99ae37fa4214bd021813206a4896`  
		Last Modified: Thu, 16 Mar 2023 02:01:00 GMT  
		Size: 6.3 MB (6310585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffee9aa0246535c2e55658c3cb0a6996668f7a403a4b960a9fdbcd4d42847f3`  
		Last Modified: Thu, 16 Mar 2023 02:00:59 GMT  
		Size: 3.0 MB (2976589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc2dd868684ceaf83a27108c1b52ca7a6e8f3b0168ad780911abc88235bfb03`  
		Last Modified: Thu, 16 Mar 2023 02:01:18 GMT  
		Size: 45.0 MB (45040946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df620083a573baec7672a8d7b904f0c02ababd741e0ace4108dda4b119901ee2`  
		Last Modified: Thu, 16 Mar 2023 02:01:42 GMT  
		Size: 126.1 MB (126083821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:3fd8a96d4a8804a8424ff1593c4b2858231aa0c710e83e5c826fab6724f4037f
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
$ docker pull buildpack-deps@sha256:edc4ef3195e1d82ba936e48a088384a87de4ef1e079743cf63a8590eb9a20bfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36354238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36747240a25171490608a4897f503021ceb197cb460e20444ca7089a2453ea7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:21:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:21:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c78e6dac9cec3c01ca7687f8e0a53a4b5e9b04f4910729279be4204ce5360e`  
		Last Modified: Thu, 16 Mar 2023 05:41:29 GMT  
		Size: 6.6 MB (6617364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b18b892afad36455b3ae75f0ab2c1bc45822e03069f2667faa4bede3825be5`  
		Last Modified: Thu, 16 Mar 2023 05:41:28 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:37305f1fffd9b6e8b98b050b702e595498870f5d0cf8cbc4d2e30cdcc7b2177a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30573365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45de6bc525f3e1c8327e7663ff847e537821bb211ca5fe282aa4fe66f79c36f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:44:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:45:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2b71966fc2f22e1375423fb61221ed137cf5e7e8d202bfa403292ba600daab`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 5.7 MB (5681012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf04b4bbda07472ffbb83ab11cb71b6ff2c6bef9749979a8a3981f285c0f53`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 2.6 MB (2586979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bbaa8d87e02533fb9f0e332551bec711913649f23f663cb20c4c47c5323680f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32583210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3656a9cc190e6da3224283797ac375e158b4a022d1d5a3d2bb49d9dac0b85124`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:58:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc06fc1cf8ad0140062ec53dbc631cea853ddb72d7c0b353edd743b1dca4ceb`  
		Last Modified: Thu, 16 Mar 2023 04:21:50 GMT  
		Size: 6.1 MB (6057809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d0b4e623a1829e474acf7b4d21109a9f27c7d8c8bf12f163ffe645eed93ec`  
		Last Modified: Thu, 16 Mar 2023 04:21:49 GMT  
		Size: 2.8 MB (2790695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c88613067a38450529dace018781fd35548bed5b209c241a5262b458b0e48a52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37328101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e48e7492b46c775c749e6d5febf5731b1aeface4bf187ab7edb99482a1e0f64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:19 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:21 GMT
ADD file:6cf3e34995c6c44762ed692b86a0442d981e9a69fa4288960047e505d75c0223 in / 
# Wed, 08 Mar 2023 03:13:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c58af8b772f2ca9c63db81d620e48946c13c027ecd7ab2d9062d010ca2ed11f3`  
		Last Modified: Thu, 16 Mar 2023 01:54:42 GMT  
		Size: 27.2 MB (27164610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df9a7dbeea70a625098ba195b5c6a6046e010992d4b2616b74e5efca85ff0`  
		Last Modified: Thu, 16 Mar 2023 02:02:18 GMT  
		Size: 6.9 MB (6907798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9c7488bcb45de5faeb1bc3f4a19015817de4a09d3c762c619d48aa2855322e`  
		Last Modified: Thu, 16 Mar 2023 02:02:17 GMT  
		Size: 3.3 MB (3255693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:93af7cd2c9b2348c3885ca9fad668d06a219296d9c2032725a0d3de25878e908
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41219499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1588570491594531960cec00e2bb87f2fb1b48f878dc4d6bd888024f30e1de`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:07:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e5cf4c1f014d5508f129bb3d2e36a3448b5d92b400a35d3051160723af42b4`  
		Last Modified: Thu, 16 Mar 2023 03:47:41 GMT  
		Size: 7.0 MB (7036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a259ed8117f57e3f76e8e31ddb857f6d36e8f1ac8131d38a456833aa7e0c20`  
		Last Modified: Thu, 16 Mar 2023 03:47:40 GMT  
		Size: 3.7 MB (3740612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:20ebcda199381e882997d1cb49046a4a86cf2a4d85ec17a0d4cf03c2342dee11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34658167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f626e5ed1171f12e2d4e06623f35558e748ecc2010eb93c132ab27524b2b55b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:23:29 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:23:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:23:31 GMT
ADD file:a6309e462d28398152cb726a11615118d79858da963b8c614772b87d87465967 in / 
# Wed, 08 Mar 2023 03:23:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:43:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3a2279f06ab19f0d57823e69b999f54a344e28bd9f955b4db9a5875c0caa543a`  
		Last Modified: Thu, 16 Mar 2023 02:01:03 GMT  
		Size: 25.4 MB (25370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37be097f66ed2ca5a62bf5e79eee23cbae99ae37fa4214bd021813206a4896`  
		Last Modified: Thu, 16 Mar 2023 02:01:00 GMT  
		Size: 6.3 MB (6310585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffee9aa0246535c2e55658c3cb0a6996668f7a403a4b960a9fdbcd4d42847f3`  
		Last Modified: Thu, 16 Mar 2023 02:00:59 GMT  
		Size: 3.0 MB (2976589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:341aade2e27224f02ffa8406356d222ae812b4b877d9cae398a6f1c9c8aa1fb3
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
$ docker pull buildpack-deps@sha256:c5ed4186cca291cb15e4a3ec07c8f72214eecb664ab6000d21de81b4ef3c22eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81868987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee72242d4f5e40206fc21b1eda028beb28d7d73857bfdba0cc421a166b05b081`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:21:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:21:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c78e6dac9cec3c01ca7687f8e0a53a4b5e9b04f4910729279be4204ce5360e`  
		Last Modified: Thu, 16 Mar 2023 05:41:29 GMT  
		Size: 6.6 MB (6617364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b18b892afad36455b3ae75f0ab2c1bc45822e03069f2667faa4bede3825be5`  
		Last Modified: Thu, 16 Mar 2023 05:41:28 GMT  
		Size: 3.0 MB (3026128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c57462ca1fd8565d56aa476a7fa497011a11c6f761194b368d2c722e146b20`  
		Last Modified: Thu, 16 Mar 2023 05:41:43 GMT  
		Size: 45.5 MB (45514749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f9d5b0d3c5fb26bbcb17109b65208ac2a36d7a6a4253289e090c1e39fbe1744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71286908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf91a3d86cf7e62586cfa021d5d042c3f8ad4473ddc03742ce5fe9199395303a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:44:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:45:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2b71966fc2f22e1375423fb61221ed137cf5e7e8d202bfa403292ba600daab`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 5.7 MB (5681012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf04b4bbda07472ffbb83ab11cb71b6ff2c6bef9749979a8a3981f285c0f53`  
		Last Modified: Thu, 16 Mar 2023 04:07:46 GMT  
		Size: 2.6 MB (2586979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3058bdcdd1b82bda414133ce433d46f98b5f56911e44f00ff6bd1de1c0a6caba`  
		Last Modified: Thu, 16 Mar 2023 04:08:04 GMT  
		Size: 40.7 MB (40713543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:127e2166fb2409edd8d8b5261a115a0e2aec1641f2bc70769b51e60924fda8eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75895079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c55e4c16477e8e6ec9875fa4a0fc1eb3184b34403fb222976e5a361d5ab3466`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:58:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:59:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc06fc1cf8ad0140062ec53dbc631cea853ddb72d7c0b353edd743b1dca4ceb`  
		Last Modified: Thu, 16 Mar 2023 04:21:50 GMT  
		Size: 6.1 MB (6057809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d0b4e623a1829e474acf7b4d21109a9f27c7d8c8bf12f163ffe645eed93ec`  
		Last Modified: Thu, 16 Mar 2023 04:21:49 GMT  
		Size: 2.8 MB (2790695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37de71f159d52bbc91be8b71a2d8862f89e2c137ac5d4e17c923aaa4fa5aa30`  
		Last Modified: Thu, 16 Mar 2023 04:22:03 GMT  
		Size: 43.3 MB (43311869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:06347734d5e392a96f4432d6290610b9761773fe58a4467957bb5ac5c104e085
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84423587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea41bed709b37c2011e131b1f224971e01f761e9a8b0c487987ca43d939e5062`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:19 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:21 GMT
ADD file:6cf3e34995c6c44762ed692b86a0442d981e9a69fa4288960047e505d75c0223 in / 
# Wed, 08 Mar 2023 03:13:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:57:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58af8b772f2ca9c63db81d620e48946c13c027ecd7ab2d9062d010ca2ed11f3`  
		Last Modified: Thu, 16 Mar 2023 01:54:42 GMT  
		Size: 27.2 MB (27164610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1df9a7dbeea70a625098ba195b5c6a6046e010992d4b2616b74e5efca85ff0`  
		Last Modified: Thu, 16 Mar 2023 02:02:18 GMT  
		Size: 6.9 MB (6907798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9c7488bcb45de5faeb1bc3f4a19015817de4a09d3c762c619d48aa2855322e`  
		Last Modified: Thu, 16 Mar 2023 02:02:17 GMT  
		Size: 3.3 MB (3255693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54663dad9d7f237e7f0a0a533af683ae66d66098cdd57ea8f90fde4dd8897ffb`  
		Last Modified: Thu, 16 Mar 2023 02:02:38 GMT  
		Size: 47.1 MB (47095486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:47ffaea8984e18680bf34023dc84dbbc005a5c50b47cb92e9221be8e55ce28a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94956291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e8cb730f01b5b2426648fed56c18477b531abea23c6d47db1eacc88079b2ab4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:07:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:08:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c668e1b654ae9320eeecdef5ebc0faea219f3828f6cd3a05983984863b60058`  
		Last Modified: Thu, 16 Mar 2023 01:43:01 GMT  
		Size: 30.4 MB (30441944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e5cf4c1f014d5508f129bb3d2e36a3448b5d92b400a35d3051160723af42b4`  
		Last Modified: Thu, 16 Mar 2023 03:47:41 GMT  
		Size: 7.0 MB (7036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a259ed8117f57e3f76e8e31ddb857f6d36e8f1ac8131d38a456833aa7e0c20`  
		Last Modified: Thu, 16 Mar 2023 03:47:40 GMT  
		Size: 3.7 MB (3740612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409f528497ffaa0bc9ae78b8139359ddd38315caf439a39a670aaed487c6c06d`  
		Last Modified: Thu, 16 Mar 2023 03:48:07 GMT  
		Size: 53.7 MB (53736792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3e5c483b07d9d0b5a4f4dbb989320ab32f2ccc83e8b565759f680a7659b1961c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79699113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d8b61386e03e4309345be55e3dd943e007820aadcbcc64fb24e1524fea86052`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:23:29 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:23:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:23:31 GMT
ADD file:a6309e462d28398152cb726a11615118d79858da963b8c614772b87d87465967 in / 
# Wed, 08 Mar 2023 03:23:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:43:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:43:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:44:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3a2279f06ab19f0d57823e69b999f54a344e28bd9f955b4db9a5875c0caa543a`  
		Last Modified: Thu, 16 Mar 2023 02:01:03 GMT  
		Size: 25.4 MB (25370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37be097f66ed2ca5a62bf5e79eee23cbae99ae37fa4214bd021813206a4896`  
		Last Modified: Thu, 16 Mar 2023 02:01:00 GMT  
		Size: 6.3 MB (6310585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffee9aa0246535c2e55658c3cb0a6996668f7a403a4b960a9fdbcd4d42847f3`  
		Last Modified: Thu, 16 Mar 2023 02:00:59 GMT  
		Size: 3.0 MB (2976589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc2dd868684ceaf83a27108c1b52ca7a6e8f3b0168ad780911abc88235bfb03`  
		Last Modified: Thu, 16 Mar 2023 02:01:18 GMT  
		Size: 45.0 MB (45040946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:acbf47c1484ea66ab4481e7cd1e28e4cf13d33200ff604e572c5d59bda54a9d7
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
$ docker pull buildpack-deps@sha256:d2831f26a1be4155a536403a4091c9fa3578d932016713ad45c204a54ef9bbe0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.9 MB (345874026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8740ff589a8566528392543b04f5042041d597aebdf89a8351ad91a78b3c798`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:35 GMT
ADD file:1cb6c660a2e3ea14b2a11bb8b80f53920c3da423a0ad7004391bfab4db4d0177 in / 
# Wed, 12 Apr 2023 00:19:36 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:48:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:49:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:49:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:50:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc556c281183180fae02d57fa6fb60ed0a99d9040936278743dc4022bfb0c686`  
		Last Modified: Wed, 12 Apr 2023 00:22:48 GMT  
		Size: 49.3 MB (49292938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8022b43d7c31d74c341d297cf10031ff0c51f596473a0c1945ee83a841094638`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 9.1 MB (9083160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db75f726ec67539c4823cb16851963ebe5838a853b0e769fd662020fad918781`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 11.4 MB (11422437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8a9e299258b84de99d6d739eb84b5b1632005f9c7723f2dd9e209fb1a8aaa3`  
		Last Modified: Wed, 12 Apr 2023 07:56:46 GMT  
		Size: 64.1 MB (64097699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5269c0251f891649bf20972368b34411b22208df54ce5c4b1b9eb649793edbb`  
		Last Modified: Wed, 12 Apr 2023 07:57:20 GMT  
		Size: 212.0 MB (211977792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ca3000a5c2c81e15247951e66c081c65117913ded0f177159d6c15adf29997c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.6 MB (314581039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7816bfe042349b0c7c87b9c180f83b2294e7e688a27afa564c62ce1bbbe48fa1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:19 GMT
ADD file:df1103dce44baa95c92287ab5016f36d5cc45c6062116ebf5273f7e79a00915c in / 
# Wed, 12 Apr 2023 00:48:20 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:795c0ca2726dffdb0e5ef6ffa341d17ec672d5915011f1a93a05e8c95a4779ae`  
		Last Modified: Wed, 12 Apr 2023 00:50:12 GMT  
		Size: 48.1 MB (48110879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e70c1a23fdf0fd320a61a2506f0ca4a391a319de8403734e4af8d678a6081fc`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 8.5 MB (8523001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27111cd5fb1057675f2e0b269790dc264d344d6e4b7ad92ff941f90a496167b`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 11.1 MB (11065924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ed8d7f4b0f78246beda91a51ddbc4ab368fe6f04bb2432498c3f5a76cbc010`  
		Last Modified: Wed, 12 Apr 2023 01:20:30 GMT  
		Size: 61.5 MB (61541287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7bffea89dcea5595c3a9d4dcd9ae2c5876dacb4265050ed658554b4d6da420`  
		Last Modified: Wed, 12 Apr 2023 01:21:06 GMT  
		Size: 185.3 MB (185339948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:83c7e12691e98dd0fc20a10fe128ccd02202938fe42a4dc9b838336aed51bceb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.9 MB (298938719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aba0af1fa024bb80f3fd7118949ea96c3eb4605028f55e173a2140e1703915e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:09:37 GMT
ADD file:084e44d77ffdb8aad1f856ec10db87922bdba3a90e06f9f1cafcb6e4284c8ff7 in / 
# Thu, 23 Mar 2023 01:09:37 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:37:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b14dce67c2fdb37d2b0eacccff5119e226c45c2906f12d6ee93d8850400824b`  
		Last Modified: Thu, 23 Mar 2023 01:32:34 GMT  
		Size: 45.9 MB (45889194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395ab26b892c3659080680521b7e37b5cee24838f59696a77cfd944e93ccd158`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 8.2 MB (8168514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788f0ce3e6e5ae63843a828f2542045686f8131e60c22d54846351e88422de`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 10.7 MB (10687642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9a3318c652dc50d1377b04d3c6d10a08df4155179df516ddbb594b1e7df246`  
		Last Modified: Thu, 23 Mar 2023 12:44:21 GMT  
		Size: 59.2 MB (59244953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23277d44a430ca9622032448c2da0203a6bd89b1246d243611b93d52ed2fa502`  
		Last Modified: Thu, 23 Mar 2023 12:44:51 GMT  
		Size: 174.9 MB (174948416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:93e13c1041833e26336a9a4362a935021cb140f05c425f7cda66b1d288da141d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (337000447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4817e1bdddcea21ae977e3e5b270332950842257559a3ae2efe4a18f83f1110e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:27 GMT
ADD file:efed18ef2a003bff7e64e7049455216e51876402083581032c35085328e416f6 in / 
# Wed, 12 Apr 2023 00:39:28 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:04:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0f987ce91d920ae0a705ed6c9824f1bbbfa282defb8986614030eb8e2bc0b4e`  
		Last Modified: Wed, 12 Apr 2023 00:41:45 GMT  
		Size: 49.3 MB (49345365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6a618ee06e99ebfbb7809c1cc4902cb717d294243f3765f170fd1c8eaf94a`  
		Last Modified: Wed, 12 Apr 2023 01:12:23 GMT  
		Size: 8.9 MB (8915044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c3f19470d2fd9e1407a7ddcbac3c316a999a143865347f221db18517e0838`  
		Last Modified: Wed, 12 Apr 2023 01:12:24 GMT  
		Size: 11.4 MB (11389565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b373ae05bf678c385bace283c65197a2bbc2a334c528ed7b58a01d93131de585`  
		Last Modified: Wed, 12 Apr 2023 01:12:39 GMT  
		Size: 64.0 MB (63974624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4f590cd785a4e380e2e92cca3c7b2d82be15d89bb52da582994cc39d9bdd5`  
		Last Modified: Wed, 12 Apr 2023 01:13:07 GMT  
		Size: 203.4 MB (203375849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:34c578f8d193ff514ac530b8922a3055877b2d87cc4e289f31e765c7450ed112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.4 MB (348376060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7d23d91b6b9538e488de01d18982225f2c00d113996363a9198e3a7dc32c14`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:30 GMT
ADD file:7718865253a3489583d40f8c7a7beede0c20cebbab68bb3e97ad2e84082afcb7 in / 
# Wed, 12 Apr 2023 00:38:30 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:02:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:03:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4ce9e81f634822e5166ef3eef875a4140795ac18afe0391433d72c7865bf67b`  
		Last Modified: Wed, 12 Apr 2023 00:41:43 GMT  
		Size: 50.3 MB (50317977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e54183fe5cb0866f886a93c0d098d38e649286a2b516b64d9658dd40f5d74b`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 9.3 MB (9264042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76896a8c48193a86329dc809066c177aedc76d55811eb32ca7c80c1ab06f66f1`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 11.8 MB (11827045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba7e1ed0df9a2a8a6501d91360cea22ab988653bf057d73c44ecb41e49f6151`  
		Last Modified: Wed, 12 Apr 2023 01:13:56 GMT  
		Size: 66.0 MB (65960427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4551baecfb99d1499518d7ef04818e3c6d649ec19322e320b452af6855389592`  
		Last Modified: Wed, 12 Apr 2023 01:14:43 GMT  
		Size: 211.0 MB (211006569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b771ae6c70d63080a0d7f3fa508cba380a502afe80ab68ab34979adbb4978d2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.4 MB (321358603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:045143f5b199fa1752d0c43df4c092cd488a99e790cf8a1b02d9edb5aaaa1645`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:15:54 GMT
ADD file:454bfcbdd9d738730885002e9124aea5e8eb4920ca5d3bf13bb9f4707023bd67 in / 
# Thu, 23 Mar 2023 05:15:59 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:03:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:05:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:12:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70edc5cd98f5a2e589d309248c77122dabf95f437c0448b99513b15ef209f244`  
		Last Modified: Thu, 23 Mar 2023 05:23:55 GMT  
		Size: 49.3 MB (49291654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74250ff8fd2374ebbb2086f535377d5246a78ee51939da5984dc42e7afe6d2f5`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 8.4 MB (8439840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c3b2ae326a6eb2a81faaff9322b317ad4788f4c53f6c3b6721724ed9f3d04`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 11.2 MB (11154181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce72fc6141c1bf4e5dcee62655f6469a6796ecc6186b5f6d227dd67b147c683`  
		Last Modified: Thu, 23 Mar 2023 07:31:48 GMT  
		Size: 62.9 MB (62937602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac50d1e65b3f5c0bb45b9748fbb137f77f5b7b2c56d8e39a47c9da1d4b420d05`  
		Last Modified: Thu, 23 Mar 2023 07:33:49 GMT  
		Size: 189.5 MB (189535326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:89a99f29891a6b80a810cf53b3c770ea325643cc1b97d0a5c10df49aeb6ee70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.7 MB (358668762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6399c6b33c24a1a9ef3642ece1d0265b6a626033822f24b9225f51bc1a08be09`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:18:49 GMT
ADD file:5e17f6075630657b8465309f99ecbfc57e325d159b54f58181b974526f2314a5 in / 
# Thu, 23 Mar 2023 01:18:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:10:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:11:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:14:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60e68956630003599038e3cfe86d6dd09ee874e8c30d9ea29b8350e0d3fa8497`  
		Last Modified: Thu, 23 Mar 2023 01:23:06 GMT  
		Size: 53.3 MB (53290316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcdbd51144dbb4a208e40072c2caf491305afb997e9161481db00137eefec5e`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 9.7 MB (9661293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bed649f1a85d37347952942e0ee256bdf515769a40a1c23cf02e65c6c90e6b1`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 12.2 MB (12168496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f138294734fe3a74e7b88ac5a9a4fe51653cff8b3ad0ba829039339f82a1a99`  
		Last Modified: Thu, 23 Mar 2023 13:23:46 GMT  
		Size: 69.6 MB (69563655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a3c96c81acee7018db01424d6026016ac1a292d63251b021cf094b1565fcde`  
		Last Modified: Thu, 23 Mar 2023 13:24:44 GMT  
		Size: 214.0 MB (213985002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f3ab35ffe09db7e9be153f5725015386c28800e98cb51a46e7c57187d5a0e602
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314808227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7150ecfe845b425b67f772c301e8610bfca04fb6c670705d638bd01b5dd34bb1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:19 GMT
ADD file:5d2b35b45a0f23e2f2e93f9c311eb34a92e4591ea27979236d801e512d44cb85 in / 
# Tue, 11 Apr 2023 23:59:31 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:24:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:25:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a09cd2374da8355612e7d4c91d55107a3f089816ae52b2c91b9e08e6a895ab1`  
		Last Modified: Wed, 12 Apr 2023 00:04:39 GMT  
		Size: 47.7 MB (47670407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d047361c12b2aeb253b1923b053dcc960101b3b3348af8f15f95f7fda2b89e4`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 8.7 MB (8713846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a462d218c24c21390b32ace449f4f47a57624b858dc05a37c31cb7f6e21c41`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 11.3 MB (11288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628da1a495c0341f28b24cb228c4984d7d8a718059c95991d67739f4a4602e4b`  
		Last Modified: Wed, 12 Apr 2023 00:32:14 GMT  
		Size: 63.1 MB (63101451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e16abe3590f67fe9ba9faa6530081d422098a3dabb4fd1cb81b378a88316bf`  
		Last Modified: Wed, 12 Apr 2023 00:32:42 GMT  
		Size: 184.0 MB (184034442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:ffce4af019ca05ac6bdf932121dba95eace904dc9236d899ed8c0f8287f80bfc
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
$ docker pull buildpack-deps@sha256:6a036620bf66ab7f03f891595654eae2995b8a08bb32443b8e130fa87c26c2b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69798535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e95348693c13cd4b3237dba422f5d46f3c7b727c7c451791d70fb9f93a80800b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:35 GMT
ADD file:1cb6c660a2e3ea14b2a11bb8b80f53920c3da423a0ad7004391bfab4db4d0177 in / 
# Wed, 12 Apr 2023 00:19:36 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:48:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:49:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cc556c281183180fae02d57fa6fb60ed0a99d9040936278743dc4022bfb0c686`  
		Last Modified: Wed, 12 Apr 2023 00:22:48 GMT  
		Size: 49.3 MB (49292938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8022b43d7c31d74c341d297cf10031ff0c51f596473a0c1945ee83a841094638`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 9.1 MB (9083160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db75f726ec67539c4823cb16851963ebe5838a853b0e769fd662020fad918781`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 11.4 MB (11422437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:66ba8371e61af6282fc38b6060f0c069dfedce71185d25e520e1124503a36408
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67699804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fc6c4cd7610510c3dbf367553fdb3b3d67108a1c4f5fef96d4fccbb8635f2db`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:19 GMT
ADD file:df1103dce44baa95c92287ab5016f36d5cc45c6062116ebf5273f7e79a00915c in / 
# Wed, 12 Apr 2023 00:48:20 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:795c0ca2726dffdb0e5ef6ffa341d17ec672d5915011f1a93a05e8c95a4779ae`  
		Last Modified: Wed, 12 Apr 2023 00:50:12 GMT  
		Size: 48.1 MB (48110879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e70c1a23fdf0fd320a61a2506f0ca4a391a319de8403734e4af8d678a6081fc`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 8.5 MB (8523001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27111cd5fb1057675f2e0b269790dc264d344d6e4b7ad92ff941f90a496167b`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 11.1 MB (11065924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1a5fd5565a96a28b5697fe91cee1bfa10686530f24736891bcc6aab90718b2ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64745350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320b1096c45b1588add1358fdcf606ea86168a27bfae2aea622165c45259f995`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:09:37 GMT
ADD file:084e44d77ffdb8aad1f856ec10db87922bdba3a90e06f9f1cafcb6e4284c8ff7 in / 
# Thu, 23 Mar 2023 01:09:37 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:37:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0b14dce67c2fdb37d2b0eacccff5119e226c45c2906f12d6ee93d8850400824b`  
		Last Modified: Thu, 23 Mar 2023 01:32:34 GMT  
		Size: 45.9 MB (45889194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395ab26b892c3659080680521b7e37b5cee24838f59696a77cfd944e93ccd158`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 8.2 MB (8168514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788f0ce3e6e5ae63843a828f2542045686f8131e60c22d54846351e88422de`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 10.7 MB (10687642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:03a892b4f8141b6f3f3c1d36591ec20f5abf8e7db913d6b06bef0195f59ada5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69649974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c5127fd80af5e1e2f2405e7610f8464a9e99f288f6b5e5afce4df2eb1aa624`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:27 GMT
ADD file:efed18ef2a003bff7e64e7049455216e51876402083581032c35085328e416f6 in / 
# Wed, 12 Apr 2023 00:39:28 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:04:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b0f987ce91d920ae0a705ed6c9824f1bbbfa282defb8986614030eb8e2bc0b4e`  
		Last Modified: Wed, 12 Apr 2023 00:41:45 GMT  
		Size: 49.3 MB (49345365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6a618ee06e99ebfbb7809c1cc4902cb717d294243f3765f170fd1c8eaf94a`  
		Last Modified: Wed, 12 Apr 2023 01:12:23 GMT  
		Size: 8.9 MB (8915044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c3f19470d2fd9e1407a7ddcbac3c316a999a143865347f221db18517e0838`  
		Last Modified: Wed, 12 Apr 2023 01:12:24 GMT  
		Size: 11.4 MB (11389565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b43a148c9da49809e8efcfafdef9c412da433e7735208795c69a14047f003874
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71409064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e15fc1cc8869eaa3b3492c5ebdad339d1c464b7630edf0a5e01a6fd94f6f3be`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:30 GMT
ADD file:7718865253a3489583d40f8c7a7beede0c20cebbab68bb3e97ad2e84082afcb7 in / 
# Wed, 12 Apr 2023 00:38:30 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:02:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a4ce9e81f634822e5166ef3eef875a4140795ac18afe0391433d72c7865bf67b`  
		Last Modified: Wed, 12 Apr 2023 00:41:43 GMT  
		Size: 50.3 MB (50317977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e54183fe5cb0866f886a93c0d098d38e649286a2b516b64d9658dd40f5d74b`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 9.3 MB (9264042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76896a8c48193a86329dc809066c177aedc76d55811eb32ca7c80c1ab06f66f1`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 11.8 MB (11827045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:cadf8f4e08099c01875c361dcd8fba3645b495aeecf0d53c2fd22a569372c184
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68885675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad6eff184509b73b66c889069c907dfd84004b8c2324f62ffbe80bc0453f87a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:15:54 GMT
ADD file:454bfcbdd9d738730885002e9124aea5e8eb4920ca5d3bf13bb9f4707023bd67 in / 
# Thu, 23 Mar 2023 05:15:59 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:03:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:70edc5cd98f5a2e589d309248c77122dabf95f437c0448b99513b15ef209f244`  
		Last Modified: Thu, 23 Mar 2023 05:23:55 GMT  
		Size: 49.3 MB (49291654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74250ff8fd2374ebbb2086f535377d5246a78ee51939da5984dc42e7afe6d2f5`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 8.4 MB (8439840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c3b2ae326a6eb2a81faaff9322b317ad4788f4c53f6c3b6721724ed9f3d04`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 11.2 MB (11154181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b2e26276ba83c4b68ff602aaa743294d6f71c408e0912d7dd1a787da5bffc9c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75120105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d6cc655a5db67e5cb97de4dfb139ff43049f64913c4d3b79788825fea30a1c9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:18:49 GMT
ADD file:5e17f6075630657b8465309f99ecbfc57e325d159b54f58181b974526f2314a5 in / 
# Thu, 23 Mar 2023 01:18:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:10:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:60e68956630003599038e3cfe86d6dd09ee874e8c30d9ea29b8350e0d3fa8497`  
		Last Modified: Thu, 23 Mar 2023 01:23:06 GMT  
		Size: 53.3 MB (53290316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcdbd51144dbb4a208e40072c2caf491305afb997e9161481db00137eefec5e`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 9.7 MB (9661293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bed649f1a85d37347952942e0ee256bdf515769a40a1c23cf02e65c6c90e6b1`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 12.2 MB (12168496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:377be7d5891b37466c736b399c0beb5ac9fdccf106bbee4e802cd0c0200a985e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67672334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75da5ea476406e76c74e365fa869cd83bc1a1cbbd23ef34d20b56b9cf7624b2c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:19 GMT
ADD file:5d2b35b45a0f23e2f2e93f9c311eb34a92e4591ea27979236d801e512d44cb85 in / 
# Tue, 11 Apr 2023 23:59:31 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:24:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8a09cd2374da8355612e7d4c91d55107a3f089816ae52b2c91b9e08e6a895ab1`  
		Last Modified: Wed, 12 Apr 2023 00:04:39 GMT  
		Size: 47.7 MB (47670407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d047361c12b2aeb253b1923b053dcc960101b3b3348af8f15f95f7fda2b89e4`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 8.7 MB (8713846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a462d218c24c21390b32ace449f4f47a57624b858dc05a37c31cb7f6e21c41`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 11.3 MB (11288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:5e0efa3054c24e10273c68601b3fccaaf0a0227b1fde44194bd37d41a14b472f
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
$ docker pull buildpack-deps@sha256:9ed3be818675099491b2a9c5066bbd63d5283caa5f3b77d978ea95ecb43f2d61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133896234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba56358263d5c537ab77ee622af1e53f4ab231c655f7637aa7739d9b469a80da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:35 GMT
ADD file:1cb6c660a2e3ea14b2a11bb8b80f53920c3da423a0ad7004391bfab4db4d0177 in / 
# Wed, 12 Apr 2023 00:19:36 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:48:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:49:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:49:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc556c281183180fae02d57fa6fb60ed0a99d9040936278743dc4022bfb0c686`  
		Last Modified: Wed, 12 Apr 2023 00:22:48 GMT  
		Size: 49.3 MB (49292938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8022b43d7c31d74c341d297cf10031ff0c51f596473a0c1945ee83a841094638`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 9.1 MB (9083160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db75f726ec67539c4823cb16851963ebe5838a853b0e769fd662020fad918781`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 11.4 MB (11422437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8a9e299258b84de99d6d739eb84b5b1632005f9c7723f2dd9e209fb1a8aaa3`  
		Last Modified: Wed, 12 Apr 2023 07:56:46 GMT  
		Size: 64.1 MB (64097699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:344b53de882fcda7c2d453195595144a3c69b6e842ee71d13d6da33ab28ecc50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129241091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5754c39ab542288953f32e05c79772f7f299ee5ef462be8bd98f34a5d5ae07f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:19 GMT
ADD file:df1103dce44baa95c92287ab5016f36d5cc45c6062116ebf5273f7e79a00915c in / 
# Wed, 12 Apr 2023 00:48:20 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:795c0ca2726dffdb0e5ef6ffa341d17ec672d5915011f1a93a05e8c95a4779ae`  
		Last Modified: Wed, 12 Apr 2023 00:50:12 GMT  
		Size: 48.1 MB (48110879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e70c1a23fdf0fd320a61a2506f0ca4a391a319de8403734e4af8d678a6081fc`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 8.5 MB (8523001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27111cd5fb1057675f2e0b269790dc264d344d6e4b7ad92ff941f90a496167b`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 11.1 MB (11065924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ed8d7f4b0f78246beda91a51ddbc4ab368fe6f04bb2432498c3f5a76cbc010`  
		Last Modified: Wed, 12 Apr 2023 01:20:30 GMT  
		Size: 61.5 MB (61541287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:83bc2ff04b8e6c4dccf1eeb1c113368f19ccdf7b850ad03505d94a5dbcb1ea9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123990303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd862b11f39b556183892c170beb4f43c718d63859ec32f1056de0082737529`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:09:37 GMT
ADD file:084e44d77ffdb8aad1f856ec10db87922bdba3a90e06f9f1cafcb6e4284c8ff7 in / 
# Thu, 23 Mar 2023 01:09:37 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:37:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b14dce67c2fdb37d2b0eacccff5119e226c45c2906f12d6ee93d8850400824b`  
		Last Modified: Thu, 23 Mar 2023 01:32:34 GMT  
		Size: 45.9 MB (45889194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395ab26b892c3659080680521b7e37b5cee24838f59696a77cfd944e93ccd158`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 8.2 MB (8168514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788f0ce3e6e5ae63843a828f2542045686f8131e60c22d54846351e88422de`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 10.7 MB (10687642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9a3318c652dc50d1377b04d3c6d10a08df4155179df516ddbb594b1e7df246`  
		Last Modified: Thu, 23 Mar 2023 12:44:21 GMT  
		Size: 59.2 MB (59244953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:14fe92b486d2fa872ed5792948ef263bf382710d96156521bba91db6409d8adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133624598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13f0946fdc4f05c98259e0c4a796a7215b79fdfac56393722a52de699ef3ad2c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:27 GMT
ADD file:efed18ef2a003bff7e64e7049455216e51876402083581032c35085328e416f6 in / 
# Wed, 12 Apr 2023 00:39:28 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:04:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0f987ce91d920ae0a705ed6c9824f1bbbfa282defb8986614030eb8e2bc0b4e`  
		Last Modified: Wed, 12 Apr 2023 00:41:45 GMT  
		Size: 49.3 MB (49345365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6a618ee06e99ebfbb7809c1cc4902cb717d294243f3765f170fd1c8eaf94a`  
		Last Modified: Wed, 12 Apr 2023 01:12:23 GMT  
		Size: 8.9 MB (8915044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c3f19470d2fd9e1407a7ddcbac3c316a999a143865347f221db18517e0838`  
		Last Modified: Wed, 12 Apr 2023 01:12:24 GMT  
		Size: 11.4 MB (11389565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b373ae05bf678c385bace283c65197a2bbc2a334c528ed7b58a01d93131de585`  
		Last Modified: Wed, 12 Apr 2023 01:12:39 GMT  
		Size: 64.0 MB (63974624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1b7217dd58c62e94d4df1bd3fe5e75114d9fdb3da6a3d8338c1e2534008bffce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137369491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8865cd6ac62a089861253f45fe5c6131b992aa6d88dd85645089c3f5ada23`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:30 GMT
ADD file:7718865253a3489583d40f8c7a7beede0c20cebbab68bb3e97ad2e84082afcb7 in / 
# Wed, 12 Apr 2023 00:38:30 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:02:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:03:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4ce9e81f634822e5166ef3eef875a4140795ac18afe0391433d72c7865bf67b`  
		Last Modified: Wed, 12 Apr 2023 00:41:43 GMT  
		Size: 50.3 MB (50317977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e54183fe5cb0866f886a93c0d098d38e649286a2b516b64d9658dd40f5d74b`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 9.3 MB (9264042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76896a8c48193a86329dc809066c177aedc76d55811eb32ca7c80c1ab06f66f1`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 11.8 MB (11827045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba7e1ed0df9a2a8a6501d91360cea22ab988653bf057d73c44ecb41e49f6151`  
		Last Modified: Wed, 12 Apr 2023 01:13:56 GMT  
		Size: 66.0 MB (65960427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:febd8b1b579bb8f8c6e10e278729e85eedae1a13b46197fcaf699aee460de42a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131823277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f8ca8bc3fe142102f73eaa97cc8abc67f75fa29f8c4f921365762e6e5e75e17`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:15:54 GMT
ADD file:454bfcbdd9d738730885002e9124aea5e8eb4920ca5d3bf13bb9f4707023bd67 in / 
# Thu, 23 Mar 2023 05:15:59 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:03:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:05:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70edc5cd98f5a2e589d309248c77122dabf95f437c0448b99513b15ef209f244`  
		Last Modified: Thu, 23 Mar 2023 05:23:55 GMT  
		Size: 49.3 MB (49291654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74250ff8fd2374ebbb2086f535377d5246a78ee51939da5984dc42e7afe6d2f5`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 8.4 MB (8439840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c3b2ae326a6eb2a81faaff9322b317ad4788f4c53f6c3b6721724ed9f3d04`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 11.2 MB (11154181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce72fc6141c1bf4e5dcee62655f6469a6796ecc6186b5f6d227dd67b147c683`  
		Last Modified: Thu, 23 Mar 2023 07:31:48 GMT  
		Size: 62.9 MB (62937602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5be307306068d9b39637f16fe607ab070f354512a3b03fa1a34fa79afe382201
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144683760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503fa7c99f71ee01993b38f1cad0622c095add9381ddd3cdfa3854728a10d5e2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:18:49 GMT
ADD file:5e17f6075630657b8465309f99ecbfc57e325d159b54f58181b974526f2314a5 in / 
# Thu, 23 Mar 2023 01:18:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:10:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:11:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60e68956630003599038e3cfe86d6dd09ee874e8c30d9ea29b8350e0d3fa8497`  
		Last Modified: Thu, 23 Mar 2023 01:23:06 GMT  
		Size: 53.3 MB (53290316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcdbd51144dbb4a208e40072c2caf491305afb997e9161481db00137eefec5e`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 9.7 MB (9661293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bed649f1a85d37347952942e0ee256bdf515769a40a1c23cf02e65c6c90e6b1`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 12.2 MB (12168496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f138294734fe3a74e7b88ac5a9a4fe51653cff8b3ad0ba829039339f82a1a99`  
		Last Modified: Thu, 23 Mar 2023 13:23:46 GMT  
		Size: 69.6 MB (69563655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f1a6a91892b66c97ca28c0d4aa10b5706ce5d49d91fcfb33f33d04a191068ce7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130773785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1798d2a8c091800a97b7795b2e2f35680f165f0a95d7f44b12965f19623788f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:19 GMT
ADD file:5d2b35b45a0f23e2f2e93f9c311eb34a92e4591ea27979236d801e512d44cb85 in / 
# Tue, 11 Apr 2023 23:59:31 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:24:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:25:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a09cd2374da8355612e7d4c91d55107a3f089816ae52b2c91b9e08e6a895ab1`  
		Last Modified: Wed, 12 Apr 2023 00:04:39 GMT  
		Size: 47.7 MB (47670407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d047361c12b2aeb253b1923b053dcc960101b3b3348af8f15f95f7fda2b89e4`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 8.7 MB (8713846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a462d218c24c21390b32ace449f4f47a57624b858dc05a37c31cb7f6e21c41`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 11.3 MB (11288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628da1a495c0341f28b24cb228c4984d7d8a718059c95991d67739f4a4602e4b`  
		Last Modified: Wed, 12 Apr 2023 00:32:14 GMT  
		Size: 63.1 MB (63101451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:422b4400e1ae3a5aa208dc236e3dc05e3db66b72387ac2d7b11bee187ff87f7d
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
$ docker pull buildpack-deps@sha256:4156d4c78d3e29a9aa11a5528a08847352e66895bb0a75cec05f4d43752fb8f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322492485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09bd8b383fcae8260115c949f68a3ccbe1df72567c4e1ad6f53b72329c1c5e1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b89f3c7f7da8adf032a33a75d1b659cee33179ecb88ea0ba75e4fc58ebe63a6`  
		Last Modified: Wed, 12 Apr 2023 07:57:46 GMT  
		Size: 54.6 MB (54584801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d62772179761f8fddfaed03ed2bdf7078b103b193d18d79a9b49364830d56cf`  
		Last Modified: Wed, 12 Apr 2023 07:58:19 GMT  
		Size: 196.8 MB (196811503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:5307e4d5147eb64f430d2a521eee4a5504ed8c4a0d7d98aa81c28190c2c963d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295551904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62bc4c385631ea22e58568f3c02e7102b4f9f8f5a1ebb96d7e82bf8764dbecae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:15:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:16:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:17:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49db155cdf8645f599affcbbbc75eb928b0a9d010c4ac54afcfa9d7e4fa85e0`  
		Last Modified: Wed, 12 Apr 2023 01:21:15 GMT  
		Size: 5.1 MB (5072827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936087cbd048148575fda58348506149db80a2699e99ae2042086628c0e5a38`  
		Last Modified: Wed, 12 Apr 2023 01:21:16 GMT  
		Size: 10.6 MB (10573853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0bf11569c39ee4f3d8515112046a55f14f39e54c6f0ea26271033c090f77d2`  
		Last Modified: Wed, 12 Apr 2023 01:21:35 GMT  
		Size: 52.3 MB (52340617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622390f39404d88752f248bc2136a55baca97d5324d43689204df0157d284282`  
		Last Modified: Wed, 12 Apr 2023 01:22:13 GMT  
		Size: 175.0 MB (175009432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f9e1d777129a6edd74d7bf1c46bceacdb0494da93b4f6f30b9e3e1ddc047be34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (283008120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49b8799c6deee224d45f54f351a870631cfae0b6039cfe91ea6c3adf9a1810e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:41:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca667140ff247fc759283fc9ff4cafbe304d1777ffc70e1bd593b63151c31a`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 4.9 MB (4934357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879c254431e9965afb23e55a148faffd29450a9218269f769be95d6e9673a93`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 10.2 MB (10217859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64c4a1b9916f6da6f286835522f27f11a812694e5f878e87468d4c6b90b343e`  
		Last Modified: Thu, 23 Mar 2023 12:45:20 GMT  
		Size: 50.4 MB (50355514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862d41b96b9b8c37267f9bb50226c9d63fc5a8df2310f511837355e187e090a`  
		Last Modified: Thu, 23 Mar 2023 12:45:51 GMT  
		Size: 167.3 MB (167288602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e7277cb741804ffe9213d32a419f6738ef4494fbd33db9326b55282dfbc1dd6b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.1 MB (314135667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c57708eddbf78525fe399f52d71e35653f6c3298641025d07fcc3323777584`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:07:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f993d5b17f32f4b8a535c25e182e5d8412625beee450e513ca57036e8fdd6dc`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 54.7 MB (54676038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26edf98ece5babdb6b65e76738cef2c2d05e7075161753d3ba95cd84480d211`  
		Last Modified: Wed, 12 Apr 2023 01:14:02 GMT  
		Size: 189.7 MB (189727693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ff274b300c58e39b8abdacecdee25d47651abe32a696616b92656ca392bd5d21
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.2 MB (328223380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5eee57e4ddbeaa9219392349db2bc711541f424d58a97b4a86ad5bd768ff773`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:06:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:07:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ccf9a5e34ba2345ce265a9a11c93ee254e1f3616dfd1c1deda6e2f7d614c8`  
		Last Modified: Wed, 12 Apr 2023 01:14:53 GMT  
		Size: 5.3 MB (5293626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4988d5e4328f031f6884a7351766aa8a2806c9cdca38d354477fc537eaa4911f`  
		Last Modified: Wed, 12 Apr 2023 01:14:54 GMT  
		Size: 11.2 MB (11249875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660a2befd486d43a308dd1561f57efeafe1f13defd6439d34aeb5efec783ee3d`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 55.9 MB (55922746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f09985282f12d05c5724bcbb0481a94f66820112bafc34a1d990dfdf74a52fc`  
		Last Modified: Wed, 12 Apr 2023 01:16:02 GMT  
		Size: 199.7 MB (199724315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ec42db429d0c72964b3b977754bc6918c60d4bf420eae2d6e4a643f9213a7305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301083947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537e8272f594cfb2548e2fb1974050af3569e7a7791f1ed883845f968edd9f25`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:15:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:21:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f79f6951926609a68e21aee7e612375637f7c12703c62b028fd60a22e2d9bfd`  
		Last Modified: Thu, 23 Mar 2023 07:34:02 GMT  
		Size: 4.9 MB (4922133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b6297024241cbdae60b7afa1bce7cc669d998e17b209e8b133df9e13da064`  
		Last Modified: Thu, 23 Mar 2023 07:34:04 GMT  
		Size: 10.7 MB (10662010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9437ab03a3b730ed3d31f18a79500c8ce379f2a971ed27695d60f38e887121b2`  
		Last Modified: Thu, 23 Mar 2023 07:34:50 GMT  
		Size: 53.3 MB (53306810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173435a2410e4cdc681e9bd4a44f44da5e7905b9826d94efbc91429ed38126f1`  
		Last Modified: Thu, 23 Mar 2023 07:36:46 GMT  
		Size: 178.9 MB (178928274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:474394b72495ae1d639248919c45100c0ee19cbc80fb7c3c85583baff857f075
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330989722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021c337c98a3039aa29eead547f736d517042181f44162b2088727645ce4a56f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:15:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:16:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:18:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805b891b319592a15b7da9a474b2f36e32ed9b8a720d14bbbe4d08422343b19`  
		Last Modified: Thu, 23 Mar 2023 13:24:55 GMT  
		Size: 5.4 MB (5415174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdb7e2b62c4c7c555894be507d7ccaf7aeca0f8c9088a9082ad4cd37dc97f28`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 11.6 MB (11629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac3f4f172050b21a6f17c30c60794779e7d5c150f1111240477b89240ad7f6`  
		Last Modified: Thu, 23 Mar 2023 13:25:22 GMT  
		Size: 58.9 MB (58864543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2fa2e478c864805494dbe6350071ba59af5a4f830abf55dc17559fb0228fa`  
		Last Modified: Thu, 23 Mar 2023 13:26:19 GMT  
		Size: 196.2 MB (196159312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:478709c66fdeffea827bb22297605067d97172933185294b18da02b3b071e7a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296079415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62811c5341c95a39adc789318a1ba301b0fae01b6b77e3b4a63a1693c43fa76d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:27:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2973b8c98f9da7833ab9cd69185dd958a8939a30136cdcfedb66ce775db358ee`  
		Last Modified: Wed, 12 Apr 2023 00:32:48 GMT  
		Size: 5.1 MB (5149313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f740d13ac612bf8b6489559a7945ec1439fee2d5eba455ab0db047cd3f30a9a`  
		Last Modified: Wed, 12 Apr 2023 00:32:49 GMT  
		Size: 10.8 MB (10766104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c0067783f401b099adca196dce9e464e66236e49faba106e2f04ac73a90df7`  
		Last Modified: Wed, 12 Apr 2023 00:33:02 GMT  
		Size: 54.1 MB (54061843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b5accdd9fd68a290692e1a0a3d853312f236ae0463540b5fdd97d598cc7a6`  
		Last Modified: Wed, 12 Apr 2023 00:33:28 GMT  
		Size: 172.8 MB (172815473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:f741d28fe1b0cc0efb79143127f1976105e90bcd5f8d3ee1156b614359102f57
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
$ docker pull buildpack-deps@sha256:acd62d4d9773006a9d0acddc08a4cbf7637d1c975e67459b52a7dc093bdfc271
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71096181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af19f7b630d3d79df60c6a9ae3051940c35c240094ef6e54f4f7843577467896`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:03091d90e79cf371dee743c2a8537556060a22246a5c1a68d53f63e201715f4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68201855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39fd3f1fac0693a3efcdf720af9216deb72c54ed024f9c8edfa061944f26d405`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:15:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49db155cdf8645f599affcbbbc75eb928b0a9d010c4ac54afcfa9d7e4fa85e0`  
		Last Modified: Wed, 12 Apr 2023 01:21:15 GMT  
		Size: 5.1 MB (5072827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936087cbd048148575fda58348506149db80a2699e99ae2042086628c0e5a38`  
		Last Modified: Wed, 12 Apr 2023 01:21:16 GMT  
		Size: 10.6 MB (10573853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1a22995743cfb2d45a6e602149e28ca1cf97d11b4cfcfc399ef35af9031dd5e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65364004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24957d317bdf2878226957903bdd121664355551e42b707fa62dd818a6d62b9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca667140ff247fc759283fc9ff4cafbe304d1777ffc70e1bd593b63151c31a`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 4.9 MB (4934357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879c254431e9965afb23e55a148faffd29450a9218269f769be95d6e9673a93`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 10.2 MB (10217859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a5537c32568d575a5a3bb0f96138a7cf42dc7d590729308b1ed7538fbdd433e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69731936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0130b5aae27ce4286f62ae8a2e5324e811b8d862aa0aea6923a7b461615ccf17`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:39321899797ed2861f1e87a3547e2e911faa2ce033098728aa240b793dd8232b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72576319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1535cd25f9ea155765a6cae9f83a5e50a533888ddb926700a119b7e91a0a0f1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ccf9a5e34ba2345ce265a9a11c93ee254e1f3616dfd1c1deda6e2f7d614c8`  
		Last Modified: Wed, 12 Apr 2023 01:14:53 GMT  
		Size: 5.3 MB (5293626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4988d5e4328f031f6884a7351766aa8a2806c9cdca38d354477fc537eaa4911f`  
		Last Modified: Wed, 12 Apr 2023 01:14:54 GMT  
		Size: 11.2 MB (11249875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:789809484997dabb78f971ed5b5198ad03b3c5b386ff5390bf32623ca9f71d48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68848863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b9683947fb7fece88ffefd3d805752e5e334f37bb5341634f0f876c6312227`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f79f6951926609a68e21aee7e612375637f7c12703c62b028fd60a22e2d9bfd`  
		Last Modified: Thu, 23 Mar 2023 07:34:02 GMT  
		Size: 4.9 MB (4922133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b6297024241cbdae60b7afa1bce7cc669d998e17b209e8b133df9e13da064`  
		Last Modified: Thu, 23 Mar 2023 07:34:04 GMT  
		Size: 10.7 MB (10662010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2200286e371e1ef3505ddd402bec8d821eddd2e8315003a4fd7bd3d43cfa7b4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75965867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa7c4a6c3a4cac50b9dcd36af9e7bf0ce438b9c24e26debfb67020874d078cb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:15:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805b891b319592a15b7da9a474b2f36e32ed9b8a720d14bbbe4d08422343b19`  
		Last Modified: Thu, 23 Mar 2023 13:24:55 GMT  
		Size: 5.4 MB (5415174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdb7e2b62c4c7c555894be507d7ccaf7aeca0f8c9088a9082ad4cd37dc97f28`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 11.6 MB (11629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5726b9b13d1328b42898380f57612273babbfe94f7918919e3553ca203957c96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69202099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d3f520b42352a1bbcb04c9c67c162e7870ac7063005e1cbfb804dea99188dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2973b8c98f9da7833ab9cd69185dd958a8939a30136cdcfedb66ce775db358ee`  
		Last Modified: Wed, 12 Apr 2023 00:32:48 GMT  
		Size: 5.1 MB (5149313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f740d13ac612bf8b6489559a7945ec1439fee2d5eba455ab0db047cd3f30a9a`  
		Last Modified: Wed, 12 Apr 2023 00:32:49 GMT  
		Size: 10.8 MB (10766104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:4fba0beac07f82d041571a394110dca419cbb71285de82105ae04e9c7401fd9c
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
$ docker pull buildpack-deps@sha256:22e8a94a63b1cf94bc6e69418b975d41cb9ca48640b8b3a48002eb9c65039abb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8cd24e709af1ad98665077ad3ae2b89451839cb3a36350db232d6ce523d0d60`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b89f3c7f7da8adf032a33a75d1b659cee33179ecb88ea0ba75e4fc58ebe63a6`  
		Last Modified: Wed, 12 Apr 2023 07:57:46 GMT  
		Size: 54.6 MB (54584801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ea05ef84678632f8c536876f2c7f5fc619fc524fc4b7dea24106ccb4b55809a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120542472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640f06156014acf4823a54fa99d9d265ad6efe6eda17f48174918044c3a2ea19`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:15:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:16:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49db155cdf8645f599affcbbbc75eb928b0a9d010c4ac54afcfa9d7e4fa85e0`  
		Last Modified: Wed, 12 Apr 2023 01:21:15 GMT  
		Size: 5.1 MB (5072827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936087cbd048148575fda58348506149db80a2699e99ae2042086628c0e5a38`  
		Last Modified: Wed, 12 Apr 2023 01:21:16 GMT  
		Size: 10.6 MB (10573853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0bf11569c39ee4f3d8515112046a55f14f39e54c6f0ea26271033c090f77d2`  
		Last Modified: Wed, 12 Apr 2023 01:21:35 GMT  
		Size: 52.3 MB (52340617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4e954e4c9de72e8e1118eb94583ab2f5f6dde3064d1c9ac34b712cd3ba6a1f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115719518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c576aa271c58013d567de0474bf19f0a9b589c98e78c3e2609b5f4dccb1bfc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca667140ff247fc759283fc9ff4cafbe304d1777ffc70e1bd593b63151c31a`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 4.9 MB (4934357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879c254431e9965afb23e55a148faffd29450a9218269f769be95d6e9673a93`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 10.2 MB (10217859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64c4a1b9916f6da6f286835522f27f11a812694e5f878e87468d4c6b90b343e`  
		Last Modified: Thu, 23 Mar 2023 12:45:20 GMT  
		Size: 50.4 MB (50355514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8932a28128c9d2abaed3ae68d2641c6738ab07bf083ca8886920e13ce37bbce3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124407974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d7143247bb9728129c637c315a5d5529383d57dfbf55c6999d1479a6f6dee2b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:07:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f993d5b17f32f4b8a535c25e182e5d8412625beee450e513ca57036e8fdd6dc`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 54.7 MB (54676038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2af50719cfc3c1165d1e75a99045d98388d375c4dcf2cafd5526a78d50080eab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128499065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863e942eeec226faacc53f695802b0b24e7dd766b5e4a9498a0d7c62e92c702`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:06:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ccf9a5e34ba2345ce265a9a11c93ee254e1f3616dfd1c1deda6e2f7d614c8`  
		Last Modified: Wed, 12 Apr 2023 01:14:53 GMT  
		Size: 5.3 MB (5293626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4988d5e4328f031f6884a7351766aa8a2806c9cdca38d354477fc537eaa4911f`  
		Last Modified: Wed, 12 Apr 2023 01:14:54 GMT  
		Size: 11.2 MB (11249875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660a2befd486d43a308dd1561f57efeafe1f13defd6439d34aeb5efec783ee3d`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 55.9 MB (55922746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a9ec515744077c37744762c48a381049165872c3140692bfa932f9cec2efd549
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122155673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6653fbf81293b8dbce803c3de0330f89c7b15f3d502575b1d0c255336c26a706`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:15:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f79f6951926609a68e21aee7e612375637f7c12703c62b028fd60a22e2d9bfd`  
		Last Modified: Thu, 23 Mar 2023 07:34:02 GMT  
		Size: 4.9 MB (4922133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b6297024241cbdae60b7afa1bce7cc669d998e17b209e8b133df9e13da064`  
		Last Modified: Thu, 23 Mar 2023 07:34:04 GMT  
		Size: 10.7 MB (10662010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9437ab03a3b730ed3d31f18a79500c8ce379f2a971ed27695d60f38e887121b2`  
		Last Modified: Thu, 23 Mar 2023 07:34:50 GMT  
		Size: 53.3 MB (53306810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:308a8f8623e3d18d4ca7d0dcbd1fc6759e17b9a128dde3c2f263439cba80795c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134830410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5026643d3fb952f674886305718eb0a8a22bc3e0a6ba7cf3c44b76b61ce8d04`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:15:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:16:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805b891b319592a15b7da9a474b2f36e32ed9b8a720d14bbbe4d08422343b19`  
		Last Modified: Thu, 23 Mar 2023 13:24:55 GMT  
		Size: 5.4 MB (5415174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdb7e2b62c4c7c555894be507d7ccaf7aeca0f8c9088a9082ad4cd37dc97f28`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 11.6 MB (11629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac3f4f172050b21a6f17c30c60794779e7d5c150f1111240477b89240ad7f6`  
		Last Modified: Thu, 23 Mar 2023 13:25:22 GMT  
		Size: 58.9 MB (58864543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dfe7b376859cc874a19230408e2042b1d984722eca290ce8cced0e27c6bdc7bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123263942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0184582450f7852885e4f2a6aaf51c5ec9ce0ff2ce9cd9b877a945b87bfd33c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:27:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2973b8c98f9da7833ab9cd69185dd958a8939a30136cdcfedb66ce775db358ee`  
		Last Modified: Wed, 12 Apr 2023 00:32:48 GMT  
		Size: 5.1 MB (5149313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f740d13ac612bf8b6489559a7945ec1439fee2d5eba455ab0db047cd3f30a9a`  
		Last Modified: Wed, 12 Apr 2023 00:32:49 GMT  
		Size: 10.8 MB (10766104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c0067783f401b099adca196dce9e464e66236e49faba106e2f04ac73a90df7`  
		Last Modified: Wed, 12 Apr 2023 00:33:02 GMT  
		Size: 54.1 MB (54061843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:9220571f3d9e6eefa8a367d60fefcd69c92c5bd591364a08f9c0f8f6adc96607
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2ea103832a6fac73696522edc50dc0aa8c41a2073edb2d29685224196ed046e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.0 MB (312037541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055f98e5c72e14d3f944a8a2f131602966cfd07c563d5884eddb16a00be4c875`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:54:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b253aeafeaa7e0671bb60008df01de101a38a045ff7bc656e3b0fbfc7c05cca5`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 7.9 MB (7863355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2201bd995cccf12851a50820de03d34a17011dcbb9ac9fdf3a50c952cbb131`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 10.0 MB (10001452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de76e268b103d05fa8960e0f77951ff54b912b63429c34f5d6adfd09f5f9ee2`  
		Last Modified: Wed, 12 Apr 2023 07:58:44 GMT  
		Size: 51.9 MB (51876420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a8df5894511ce28a05e2925a75e8a4acbd0634c39ad734fdfba8e23d1b1569`  
		Last Modified: Wed, 12 Apr 2023 07:59:14 GMT  
		Size: 191.8 MB (191847588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:02fd9794c7da040f3ef1d7dd0c0712ab7683702b42b2a51e61ab533b528b764d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.9 MB (277871011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15256ef87a3aabbd62493903b36c4f9b28de5b55c797bcfc8455138b602cf77c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Mar 2023 23:23:23 GMT
ADD file:dabb9dad1d8086faa890c6425e759e27f1052d9677aa640dd310def49d8a5bc5 in / 
# Fri, 24 Mar 2023 23:23:24 GMT
CMD ["bash"]
# Sat, 25 Mar 2023 01:03:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Mar 2023 01:03:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Apr 2023 23:15:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 07 Apr 2023 23:17:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09b82635e0c9396d28359dea2597b070f13d2e7fbdd1b9cb395b7f7a1cd09d59`  
		Last Modified: Fri, 24 Mar 2023 23:28:44 GMT  
		Size: 45.9 MB (45915861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be96c3cc707a08b828f7785eb0ec3a8a556466f537aa6de458e43a19667d155`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 7.2 MB (7153944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65e90f973c6f54fcc28489eb109e74c36765dd1293a930f62889f9f1ac1f75`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 9.3 MB (9348989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c951b868b2dee5c41bb5bc49ed01649d3b23457f73f686de3257e3922c4237`  
		Last Modified: Fri, 07 Apr 2023 23:18:43 GMT  
		Size: 47.4 MB (47395369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22d1abb7637dd224bb51a637438918a121d198e654c56e2207e8bca99b6ba2d`  
		Last Modified: Fri, 07 Apr 2023 23:19:12 GMT  
		Size: 168.1 MB (168056848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5e8e3f3212dcc5c0e3442e591cffe69a01891021308eca92c8b3bc2803c31459
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.6 MB (302601726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0303fb5950d191d02ab39565ca367ca55dc2b108c9b7ba4d645ed85d1a074d1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:10:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208fd617b499747daceba851b67da426c285d1e306b316a193f06968123f49da`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 7.7 MB (7732136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efadebfda1423d1b70a0e991e9ff8bb2e3fe0b08d55562359a004c265fc7c86`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe7e7c438113f5e58417f97e7eb0a755b17ee63eebd85a7c3b86a2aad4c993e`  
		Last Modified: Wed, 12 Apr 2023 01:14:27 GMT  
		Size: 52.2 MB (52191713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33997ebd7335eb6f55d98725b5fb8e4899166098d6db119cd6f6bc7055ffa858`  
		Last Modified: Wed, 12 Apr 2023 01:14:51 GMT  
		Size: 183.4 MB (183435664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:76a9d8ac8ca52b47077a29022657b9bdc9facd485bf6f6bc8c7115ed9915e020
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.5 MB (321464682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb3655fb3b861afdfc5e7da86468a57acd97ab2b796815bf255141ce4e9ec42c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:11 GMT
ADD file:8299e58c7e43af1f3b9fdb9bd37e3f37cf619a97ef1b87d60ca66860d646d526 in / 
# Wed, 12 Apr 2023 00:39:11 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:08:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d15e1c2a3da7d675c2513d7ceab1d0f33ced9a82bed63d9a11ce71f1218d232`  
		Last Modified: Wed, 12 Apr 2023 00:43:07 GMT  
		Size: 51.2 MB (51206167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af123d7f5c8b1197b6040820195efacf1a57299baf71416c7a63281566cdc199`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 8.0 MB (8034011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3af175eda8706326ac898703f9aafb47e7e08ec08318794c6838efa8f3d3bc`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 10.3 MB (10345678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cbd6d7217bf920da02e590f88fbfb42fb3162969840a3b17eb25c762247c04`  
		Last Modified: Wed, 12 Apr 2023 01:16:35 GMT  
		Size: 53.5 MB (53471080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d0a6f1efbd6131f1ae888ea393318f9d32a3e8ad8b8c97207c3a5b7a3ed9bc`  
		Last Modified: Wed, 12 Apr 2023 01:17:17 GMT  
		Size: 198.4 MB (198407746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:640a378736a09f13765f1e7113e5082c0e5afbad023a3bc5fd16061f36d68106
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7f26d8de0d9b1472f4b76a591461f81e28dd4469eed96b3bb172a93adde9779f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68313533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:212d47455d74a1b460742fc95270dd155e5dccb7f8cf98d1b0166a911a42e56f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b253aeafeaa7e0671bb60008df01de101a38a045ff7bc656e3b0fbfc7c05cca5`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 7.9 MB (7863355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2201bd995cccf12851a50820de03d34a17011dcbb9ac9fdf3a50c952cbb131`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 10.0 MB (10001452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8c8d5fcfcee6383cfd57156be5815dd7406a36072a56878ea28be0754c13d629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62418794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27f682abc8f89b3916f2a6eeef8f25431524f50af3bac2d7eccbba6aea38a8b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Mar 2023 23:23:23 GMT
ADD file:dabb9dad1d8086faa890c6425e759e27f1052d9677aa640dd310def49d8a5bc5 in / 
# Fri, 24 Mar 2023 23:23:24 GMT
CMD ["bash"]
# Sat, 25 Mar 2023 01:03:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Mar 2023 01:03:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:09b82635e0c9396d28359dea2597b070f13d2e7fbdd1b9cb395b7f7a1cd09d59`  
		Last Modified: Fri, 24 Mar 2023 23:28:44 GMT  
		Size: 45.9 MB (45915861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be96c3cc707a08b828f7785eb0ec3a8a556466f537aa6de458e43a19667d155`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 7.2 MB (7153944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65e90f973c6f54fcc28489eb109e74c36765dd1293a930f62889f9f1ac1f75`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 9.3 MB (9348989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f4f9c875a9f7cdaa332594325c8c868d26a05ef018355a11554c8b1b5657b625
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66974349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25cefdb01c939d204ba6d7c49b6053a29c8ad035592de81e899acd889fd70fc2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208fd617b499747daceba851b67da426c285d1e306b316a193f06968123f49da`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 7.7 MB (7732136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efadebfda1423d1b70a0e991e9ff8bb2e3fe0b08d55562359a004c265fc7c86`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:da84dcb1542b8a34ef0e6ebd7f50eeb5da1bf9f8c87c221b3d3a2bd81c81de56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69585856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:256da6b06a3adecebaf9bba1b763d651016b84bfec4ad7bc9dbe24e15f37894a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:11 GMT
ADD file:8299e58c7e43af1f3b9fdb9bd37e3f37cf619a97ef1b87d60ca66860d646d526 in / 
# Wed, 12 Apr 2023 00:39:11 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2d15e1c2a3da7d675c2513d7ceab1d0f33ced9a82bed63d9a11ce71f1218d232`  
		Last Modified: Wed, 12 Apr 2023 00:43:07 GMT  
		Size: 51.2 MB (51206167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af123d7f5c8b1197b6040820195efacf1a57299baf71416c7a63281566cdc199`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 8.0 MB (8034011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3af175eda8706326ac898703f9aafb47e7e08ec08318794c6838efa8f3d3bc`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 10.3 MB (10345678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:2d4209bed38ccbaafe80aa66292d82ca537b2ef985ab3f0ac7743ce258f39660
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0559dadbf61570961c0fad2acef618449ab55dc06360900e44639acdfc52d29b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120189953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ba89d7351401c33e1d4f3e124b255947cc4bf33b68236db9d8985829c0c1420`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b253aeafeaa7e0671bb60008df01de101a38a045ff7bc656e3b0fbfc7c05cca5`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 7.9 MB (7863355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2201bd995cccf12851a50820de03d34a17011dcbb9ac9fdf3a50c952cbb131`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 10.0 MB (10001452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de76e268b103d05fa8960e0f77951ff54b912b63429c34f5d6adfd09f5f9ee2`  
		Last Modified: Wed, 12 Apr 2023 07:58:44 GMT  
		Size: 51.9 MB (51876420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:73ce5e0aec65d7a74a776adbc4a7f73e23a098cc443305405cf91545d7428a1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109814163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93145c7f3983a14d63ebc6172d40d92d34548b31354e82b5de20eeb2dc2db6b6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Mar 2023 23:23:23 GMT
ADD file:dabb9dad1d8086faa890c6425e759e27f1052d9677aa640dd310def49d8a5bc5 in / 
# Fri, 24 Mar 2023 23:23:24 GMT
CMD ["bash"]
# Sat, 25 Mar 2023 01:03:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Mar 2023 01:03:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Apr 2023 23:15:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09b82635e0c9396d28359dea2597b070f13d2e7fbdd1b9cb395b7f7a1cd09d59`  
		Last Modified: Fri, 24 Mar 2023 23:28:44 GMT  
		Size: 45.9 MB (45915861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be96c3cc707a08b828f7785eb0ec3a8a556466f537aa6de458e43a19667d155`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 7.2 MB (7153944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65e90f973c6f54fcc28489eb109e74c36765dd1293a930f62889f9f1ac1f75`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 9.3 MB (9348989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c951b868b2dee5c41bb5bc49ed01649d3b23457f73f686de3257e3922c4237`  
		Last Modified: Fri, 07 Apr 2023 23:18:43 GMT  
		Size: 47.4 MB (47395369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:96e03d67380daeace99ddc589fb25df608d86e8a2d78ef9d4635323c7774934b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119166062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2ed8743d8648e388b28b2c5274b320ccc3352bca03a56d3d0b65c133c5acf9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208fd617b499747daceba851b67da426c285d1e306b316a193f06968123f49da`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 7.7 MB (7732136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efadebfda1423d1b70a0e991e9ff8bb2e3fe0b08d55562359a004c265fc7c86`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe7e7c438113f5e58417f97e7eb0a755b17ee63eebd85a7c3b86a2aad4c993e`  
		Last Modified: Wed, 12 Apr 2023 01:14:27 GMT  
		Size: 52.2 MB (52191713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0e2e0b3634ba26d3880a8dad7170dc329234f18b5b9b38e0bd3c4637cbe27ace
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123056936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67dfa6883f98d7b82d1d95b560a9f118e646738acef237ff47081baf6ed84941`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:11 GMT
ADD file:8299e58c7e43af1f3b9fdb9bd37e3f37cf619a97ef1b87d60ca66860d646d526 in / 
# Wed, 12 Apr 2023 00:39:11 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:08:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d15e1c2a3da7d675c2513d7ceab1d0f33ced9a82bed63d9a11ce71f1218d232`  
		Last Modified: Wed, 12 Apr 2023 00:43:07 GMT  
		Size: 51.2 MB (51206167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af123d7f5c8b1197b6040820195efacf1a57299baf71416c7a63281566cdc199`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 8.0 MB (8034011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3af175eda8706326ac898703f9aafb47e7e08ec08318794c6838efa8f3d3bc`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 10.3 MB (10345678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cbd6d7217bf920da02e590f88fbfb42fb3162969840a3b17eb25c762247c04`  
		Last Modified: Wed, 12 Apr 2023 01:16:35 GMT  
		Size: 53.5 MB (53471080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:f741d28fe1b0cc0efb79143127f1976105e90bcd5f8d3ee1156b614359102f57
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
$ docker pull buildpack-deps@sha256:acd62d4d9773006a9d0acddc08a4cbf7637d1c975e67459b52a7dc093bdfc271
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71096181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af19f7b630d3d79df60c6a9ae3051940c35c240094ef6e54f4f7843577467896`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:03091d90e79cf371dee743c2a8537556060a22246a5c1a68d53f63e201715f4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68201855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39fd3f1fac0693a3efcdf720af9216deb72c54ed024f9c8edfa061944f26d405`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:15:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49db155cdf8645f599affcbbbc75eb928b0a9d010c4ac54afcfa9d7e4fa85e0`  
		Last Modified: Wed, 12 Apr 2023 01:21:15 GMT  
		Size: 5.1 MB (5072827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936087cbd048148575fda58348506149db80a2699e99ae2042086628c0e5a38`  
		Last Modified: Wed, 12 Apr 2023 01:21:16 GMT  
		Size: 10.6 MB (10573853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1a22995743cfb2d45a6e602149e28ca1cf97d11b4cfcfc399ef35af9031dd5e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65364004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24957d317bdf2878226957903bdd121664355551e42b707fa62dd818a6d62b9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca667140ff247fc759283fc9ff4cafbe304d1777ffc70e1bd593b63151c31a`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 4.9 MB (4934357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879c254431e9965afb23e55a148faffd29450a9218269f769be95d6e9673a93`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 10.2 MB (10217859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a5537c32568d575a5a3bb0f96138a7cf42dc7d590729308b1ed7538fbdd433e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69731936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0130b5aae27ce4286f62ae8a2e5324e811b8d862aa0aea6923a7b461615ccf17`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:39321899797ed2861f1e87a3547e2e911faa2ce033098728aa240b793dd8232b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72576319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1535cd25f9ea155765a6cae9f83a5e50a533888ddb926700a119b7e91a0a0f1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ccf9a5e34ba2345ce265a9a11c93ee254e1f3616dfd1c1deda6e2f7d614c8`  
		Last Modified: Wed, 12 Apr 2023 01:14:53 GMT  
		Size: 5.3 MB (5293626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4988d5e4328f031f6884a7351766aa8a2806c9cdca38d354477fc537eaa4911f`  
		Last Modified: Wed, 12 Apr 2023 01:14:54 GMT  
		Size: 11.2 MB (11249875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:789809484997dabb78f971ed5b5198ad03b3c5b386ff5390bf32623ca9f71d48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68848863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b9683947fb7fece88ffefd3d805752e5e334f37bb5341634f0f876c6312227`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f79f6951926609a68e21aee7e612375637f7c12703c62b028fd60a22e2d9bfd`  
		Last Modified: Thu, 23 Mar 2023 07:34:02 GMT  
		Size: 4.9 MB (4922133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b6297024241cbdae60b7afa1bce7cc669d998e17b209e8b133df9e13da064`  
		Last Modified: Thu, 23 Mar 2023 07:34:04 GMT  
		Size: 10.7 MB (10662010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2200286e371e1ef3505ddd402bec8d821eddd2e8315003a4fd7bd3d43cfa7b4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75965867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa7c4a6c3a4cac50b9dcd36af9e7bf0ce438b9c24e26debfb67020874d078cb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:15:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805b891b319592a15b7da9a474b2f36e32ed9b8a720d14bbbe4d08422343b19`  
		Last Modified: Thu, 23 Mar 2023 13:24:55 GMT  
		Size: 5.4 MB (5415174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdb7e2b62c4c7c555894be507d7ccaf7aeca0f8c9088a9082ad4cd37dc97f28`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 11.6 MB (11629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5726b9b13d1328b42898380f57612273babbfe94f7918919e3553ca203957c96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69202099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d3f520b42352a1bbcb04c9c67c162e7870ac7063005e1cbfb804dea99188dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2973b8c98f9da7833ab9cd69185dd958a8939a30136cdcfedb66ce775db358ee`  
		Last Modified: Wed, 12 Apr 2023 00:32:48 GMT  
		Size: 5.1 MB (5149313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f740d13ac612bf8b6489559a7945ec1439fee2d5eba455ab0db047cd3f30a9a`  
		Last Modified: Wed, 12 Apr 2023 00:32:49 GMT  
		Size: 10.8 MB (10766104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:19c0f7f64b8335561e884c84493a4a3480f90912af313ce1584b55dac0410045
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
$ docker pull buildpack-deps@sha256:a499d7cf331a38e4daf02148cf1f4b908048eab65947d337c4954bf635d37592
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245775730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7906168918fbe41e4eacbec9b2252ee5a4c8d9ab004d3ba2719b59d4a9719c3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:25:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:25:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:26:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:28:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bc9af4214222561c992590ace8ae277238c112e32760c1ff3ef6caf8ca4f6`  
		Last Modified: Thu, 16 Mar 2023 05:42:20 GMT  
		Size: 7.7 MB (7739206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155d64edd9d618f19a8fecb84dfbc4cf87eff8210625c22cc9634721fba93a7f`  
		Last Modified: Thu, 16 Mar 2023 05:42:19 GMT  
		Size: 3.6 MB (3627138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231a0ed819686e9daf3eef08ba444c6b7ebd1f65cdb1fe72aef57a0f6bb50b44`  
		Last Modified: Thu, 16 Mar 2023 05:42:37 GMT  
		Size: 60.7 MB (60741678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd7ee9669c83df2d803ace7367f27ea8d15d3ef24e11274c8810ecfb106739c`  
		Last Modified: Thu, 16 Mar 2023 05:43:05 GMT  
		Size: 145.1 MB (145089640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7328be0f102351eef287e2517d6ee5c2bbe3f4148f3a5ea2cfe48671892d56ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211775407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dddfdd3085f4ab0f9a8671e25b13cea8ae4112cca857278022e03057c9cada`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:48:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:48:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:49:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:50:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47332fc42b573d4baf56c0357c8403f43cd7e32995cd91e98f1b63904c165edc`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 6.7 MB (6726111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7608366f198edf1178000bf5d347ad633c37686847555ad129799eb689113`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 3.1 MB (3104510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53730f672819fbb90234967569a7b902545c30edae9b2a899cbd60f6d11c64d1`  
		Last Modified: Thu, 16 Mar 2023 04:09:01 GMT  
		Size: 55.4 MB (55433480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053c5c89030c8bd301889d79a2fc68e023925bd9527dc1fc7cab71f8a4bae26f`  
		Last Modified: Thu, 16 Mar 2023 04:09:28 GMT  
		Size: 121.9 MB (121924824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ff57e910e4f7e1d0490a538306c2bc5f7d3c3be91bc6b6d4949901ec3f2a24a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235999544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83ed8c452dfe38712e7bd28165dece30e24886b5d4095feddafa309b723f28c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:03:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:04:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:07:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada92025b6d5b0737643d0b1828f2344b2cdb92c860a121d471b8f0c87875d0c`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 7.6 MB (7602314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d3bbdc78821c82e7efb7e6b25412a925801281a52d89ff278c1440c1682f2`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 3.6 MB (3617260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f381dea6869d6e20db1531b80e454b1082f1678f0397903199ce41446330364`  
		Last Modified: Thu, 16 Mar 2023 04:22:52 GMT  
		Size: 60.8 MB (60817533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0abeae2a014e811b1cd94b6bf883f31eeea92a20e0e001d1142493ed5a2c9e`  
		Last Modified: Thu, 16 Mar 2023 04:23:14 GMT  
		Size: 136.8 MB (136766276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3e9e963156b739e06ca605543ef30f47c13d2f94fa896e98194fbbffdf0948d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269621988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:554288919fbda3305223d05afd514cd056b314df8de2d1ed100be57b04e2fdac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:15:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:17:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:22:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35c7876eb976fb68d0f3bf24f227b6220a73f879e77ad564d913af35104da2eb`  
		Last Modified: Thu, 16 Mar 2023 01:58:06 GMT  
		Size: 33.3 MB (33300378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6346be203b914f77b544d394d2d63c301d06a7b8926cd30449cdb5a3046edc`  
		Last Modified: Thu, 16 Mar 2023 03:49:06 GMT  
		Size: 8.7 MB (8692841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabdc66fc416ff468476139eca7bc89d467220b030d725d5715d0f79364e4c8`  
		Last Modified: Thu, 16 Mar 2023 03:49:04 GMT  
		Size: 4.5 MB (4486834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a7f4b71be518565ac628205f8fc97a71ee63e098c11a5602ff80ad69427db1`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 69.6 MB (69553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87bf022fbd7e81163adf826c15b5acbc213f43f5ea50267acaa3fb720dbf501`  
		Last Modified: Thu, 16 Mar 2023 03:50:23 GMT  
		Size: 153.6 MB (153588308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1d9d8256bc33bab81422b7a398094681d9648a8c654df7a6c1eeebdd004a1e38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226375246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00868f7fb08f67a580a9e48f17f152318ef7cd6afe9d8b40e94cbf0615c43b56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:46:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:47:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:49:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:422c367cdac1ee2f6bd9ea546c8e5a643af0847a822d04ba202af409973273ad`  
		Last Modified: Thu, 16 Mar 2023 01:40:19 GMT  
		Size: 27.0 MB (27016120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a483453055472ff48de1fd6d705ef6ead7ebb9e0846c4954ba91b6fb7660d5`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 7.4 MB (7379309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348a385bccd245fea6b55ab45b16d2bd72f5a321f2339d63941b14ea5af141e`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 3.5 MB (3542074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75aaa62969cac1411806a644c6dfa90c4b1cdbb89ee7952acb34e84da5caa83`  
		Last Modified: Thu, 16 Mar 2023 02:02:05 GMT  
		Size: 60.0 MB (60015921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae1a1a48eef579da3815ca10377b205802a368ab7293d343e8f40d7fed0be9c`  
		Last Modified: Thu, 16 Mar 2023 02:02:29 GMT  
		Size: 128.4 MB (128421822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:603fe1ece48d066ae790ee69b12733fa30d45465034083519f2bfba9c81e5875
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
$ docker pull buildpack-deps@sha256:244b89a7f94d393b379d796cf11687de045affc0a8ec223b9c140cf08cd1d583
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39944412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:502631fc74e69f270fc93f0d999f3c9fd1757effb421af66951f8fde5428f4d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:25:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:25:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bc9af4214222561c992590ace8ae277238c112e32760c1ff3ef6caf8ca4f6`  
		Last Modified: Thu, 16 Mar 2023 05:42:20 GMT  
		Size: 7.7 MB (7739206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155d64edd9d618f19a8fecb84dfbc4cf87eff8210625c22cc9634721fba93a7f`  
		Last Modified: Thu, 16 Mar 2023 05:42:19 GMT  
		Size: 3.6 MB (3627138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1e8bc526fbffc69c9d0e626081bc81793a560032e1e3c4d3a449f5a60672d96f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34417103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c33bbc0c141172ce22bf7cf86bda316933123e335366e1ea9deba8bd6b964d00`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:48:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:48:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47332fc42b573d4baf56c0357c8403f43cd7e32995cd91e98f1b63904c165edc`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 6.7 MB (6726111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7608366f198edf1178000bf5d347ad633c37686847555ad129799eb689113`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 3.1 MB (3104510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ffc84a0fcbb9d176e50ebb0222e5eeb290a58fb42bf38dc74b182632e8e2e222
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38415735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce8c193e0e6515f7fb45285ce5e80b324f558869d3e85d6ccb9c186b56de169b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:03:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada92025b6d5b0737643d0b1828f2344b2cdb92c860a121d471b8f0c87875d0c`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 7.6 MB (7602314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d3bbdc78821c82e7efb7e6b25412a925801281a52d89ff278c1440c1682f2`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 3.6 MB (3617260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6bcb7bbe9e71ec3bf79e404b8dca4821d0a8a8d3e0ba52087d4db6b77cfa2e2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46480053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2030d035639fd89c4173ce60293f8f470778669b33f7cb717d29c96ea46f603`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:15:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:35c7876eb976fb68d0f3bf24f227b6220a73f879e77ad564d913af35104da2eb`  
		Last Modified: Thu, 16 Mar 2023 01:58:06 GMT  
		Size: 33.3 MB (33300378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6346be203b914f77b544d394d2d63c301d06a7b8926cd30449cdb5a3046edc`  
		Last Modified: Thu, 16 Mar 2023 03:49:06 GMT  
		Size: 8.7 MB (8692841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabdc66fc416ff468476139eca7bc89d467220b030d725d5715d0f79364e4c8`  
		Last Modified: Thu, 16 Mar 2023 03:49:04 GMT  
		Size: 4.5 MB (4486834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1c1099e10a2fe4905babce95ad918aafac037e6865e1dd2de6bebf8c1b1b282f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37937503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e125599525fdd8c0449dd97ad937ff4d8e51359718898ac7bf028fcc1e0ef9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:46:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:422c367cdac1ee2f6bd9ea546c8e5a643af0847a822d04ba202af409973273ad`  
		Last Modified: Thu, 16 Mar 2023 01:40:19 GMT  
		Size: 27.0 MB (27016120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a483453055472ff48de1fd6d705ef6ead7ebb9e0846c4954ba91b6fb7660d5`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 7.4 MB (7379309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348a385bccd245fea6b55ab45b16d2bd72f5a321f2339d63941b14ea5af141e`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 3.5 MB (3542074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:9103aa62d5027f1fb05a5d84099d7267fbe850182634fd6e3c294d06663c8a95
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
$ docker pull buildpack-deps@sha256:f50962aa19f626f477ccc1d83a5c7a2c58f82d9ed60236522a10c4283117c4c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100686090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db3508b90f202b776567efc3d8a59364ad1cf351a3a715e39aa46e5fbc8c68b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:25:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:25:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:26:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2bc9af4214222561c992590ace8ae277238c112e32760c1ff3ef6caf8ca4f6`  
		Last Modified: Thu, 16 Mar 2023 05:42:20 GMT  
		Size: 7.7 MB (7739206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155d64edd9d618f19a8fecb84dfbc4cf87eff8210625c22cc9634721fba93a7f`  
		Last Modified: Thu, 16 Mar 2023 05:42:19 GMT  
		Size: 3.6 MB (3627138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231a0ed819686e9daf3eef08ba444c6b7ebd1f65cdb1fe72aef57a0f6bb50b44`  
		Last Modified: Thu, 16 Mar 2023 05:42:37 GMT  
		Size: 60.7 MB (60741678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:58f3602ee4c39695c30963274b5faeb2d2167ace201af9f3f4c6eacbf8649880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89850583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77759cced7d3cf207131d1c31211cac9b8d4c861cb3cedfedc5392380534046e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:48:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:48:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:49:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47332fc42b573d4baf56c0357c8403f43cd7e32995cd91e98f1b63904c165edc`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 6.7 MB (6726111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7608366f198edf1178000bf5d347ad633c37686847555ad129799eb689113`  
		Last Modified: Thu, 16 Mar 2023 04:08:41 GMT  
		Size: 3.1 MB (3104510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53730f672819fbb90234967569a7b902545c30edae9b2a899cbd60f6d11c64d1`  
		Last Modified: Thu, 16 Mar 2023 04:09:01 GMT  
		Size: 55.4 MB (55433480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cd02558f0a6dfba6c29fb4fd3b69d47d7ed610742c110ad3d48dd3665b3969c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99233268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385e737702d65ec663825da56324f18677ab4add5cb2c78ea43971cfa1d0310d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:03:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:04:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada92025b6d5b0737643d0b1828f2344b2cdb92c860a121d471b8f0c87875d0c`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 7.6 MB (7602314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d3bbdc78821c82e7efb7e6b25412a925801281a52d89ff278c1440c1682f2`  
		Last Modified: Thu, 16 Mar 2023 04:22:35 GMT  
		Size: 3.6 MB (3617260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f381dea6869d6e20db1531b80e454b1082f1678f0397903199ce41446330364`  
		Last Modified: Thu, 16 Mar 2023 04:22:52 GMT  
		Size: 60.8 MB (60817533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:04aa4f32a7113bd9a0200497ffd5fbaeff2317498842cec9c830351405426a17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116033680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76b46c4ec83bd6f7f1c891f7e7a478529374a2b66b1958647d5603fbf251d8f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:15:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:17:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35c7876eb976fb68d0f3bf24f227b6220a73f879e77ad564d913af35104da2eb`  
		Last Modified: Thu, 16 Mar 2023 01:58:06 GMT  
		Size: 33.3 MB (33300378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6346be203b914f77b544d394d2d63c301d06a7b8926cd30449cdb5a3046edc`  
		Last Modified: Thu, 16 Mar 2023 03:49:06 GMT  
		Size: 8.7 MB (8692841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabdc66fc416ff468476139eca7bc89d467220b030d725d5715d0f79364e4c8`  
		Last Modified: Thu, 16 Mar 2023 03:49:04 GMT  
		Size: 4.5 MB (4486834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a7f4b71be518565ac628205f8fc97a71ee63e098c11a5602ff80ad69427db1`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 69.6 MB (69553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:92b7d5e1a84baf82d1937e88aa05702580caababdba82c5b27730cf1ad6a71e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (97953424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:240ac351ad3ff93ba8dfd9d10b19e92cfa3c8bcba3868e4927134e37ce7ec2e9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:46:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:46:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:47:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:422c367cdac1ee2f6bd9ea546c8e5a643af0847a822d04ba202af409973273ad`  
		Last Modified: Thu, 16 Mar 2023 01:40:19 GMT  
		Size: 27.0 MB (27016120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a483453055472ff48de1fd6d705ef6ead7ebb9e0846c4954ba91b6fb7660d5`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 7.4 MB (7379309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348a385bccd245fea6b55ab45b16d2bd72f5a321f2339d63941b14ea5af141e`  
		Last Modified: Thu, 16 Mar 2023 02:01:49 GMT  
		Size: 3.5 MB (3542074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75aaa62969cac1411806a644c6dfa90c4b1cdbb89ee7952acb34e84da5caa83`  
		Last Modified: Thu, 16 Mar 2023 02:02:05 GMT  
		Size: 60.0 MB (60015921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy`

```console
$ docker pull buildpack-deps@sha256:fe20c1a1fa7749ce93af04e56c2a46297e6b236eeddbdb8fd780ec58784c121a
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
$ docker pull buildpack-deps@sha256:c7af89fe20e8b370fa3d84c23f5dbb048e01cfd38fbc12c1e02232c1a84af80f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (250022556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375da4bb35d8bd52aa3070617888fd8aea7a8aec9a99774cdd1df6a8a87cd5ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:29:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:29:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:29:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:32:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7490ba7e16ba382ca21015280e2ee6dad31879a1f043029e350a8e429770f36`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.8 MB (3788671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeb23ea57c359eecf9e21c40ddb69f738e9121008fd4956d733ba66d3b7eb38`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.6 MB (3561600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c00a0ea05e6a2089233e7238bbed0ffbf7b2655f03195967e2083ee623899`  
		Last Modified: Thu, 16 Mar 2023 05:43:30 GMT  
		Size: 39.4 MB (39352910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa902bb14f17725bbd311e77e44da0ef803e68e0965c5f95635eb83f288b5d4`  
		Last Modified: Thu, 16 Mar 2023 05:44:00 GMT  
		Size: 172.9 MB (172889412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:548a747004a966f5fe24d920b0b67a7e2f63d2f84ee8a998d73573f3534d291c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216673703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2805f8c5309daa5cfffe1813e3cf819142f1ed5ef4f8e6be329cbcad71c2d30`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:51:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:51:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:52:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:55:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d54aa809ca004a01d3a10bf7017a1fb216f185fd9d0f210f1bc9512298c1`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.5 MB (3540124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caec72904127d7cb95dfd39a3f311865b026d929e1440427ec21122be6e15db3`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.7 MB (3714418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b259dc20995aa828e48008def151ea3da6891615621976f66dc6b63fdbda38a`  
		Last Modified: Thu, 16 Mar 2023 04:09:57 GMT  
		Size: 41.9 MB (41908320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d21e83a1a0d8dfe0c0f53e1f8d51356e226e68eb9de5b136253db03ceac4e7`  
		Last Modified: Thu, 16 Mar 2023 04:10:26 GMT  
		Size: 140.5 MB (140485444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bc8bb348a53f7d9f3e309b375c7fd76b56a0c48f89c849a9c6ade599cdc8180a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241329007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffb8e18683ff48d54f07c675683997a40a1555dde02c54147d8d9d48aa756df`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:08:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:08:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aef66b301cbfe4ff1bb09357ccf381140239a236438d27a992d076491a3a066`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.8 MB (3760501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693278d975de74bdcb529fd46771b1335b9501b8f479a3c8128b69375f7945a8`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.5 MB (3536190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfc2e7bfd914b57fdeae1d187ca7a12534443f9e2a6142287dab73c0296ade8`  
		Last Modified: Thu, 16 Mar 2023 04:23:36 GMT  
		Size: 39.2 MB (39243621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2292b558961f2b5d5b6555b004730bdf51c7012b78b0a9474df76b1674aaa26`  
		Last Modified: Thu, 16 Mar 2023 04:24:01 GMT  
		Size: 166.4 MB (166401141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d098228e71918993c4063a767b2eef4e86f48651116a36ecd3b3faa15276d498
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271846871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55eaa1527dc94604178ceeb1d0dd71d0ef94cf7213d605391668aa27d2fb142e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:24:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:29:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda6a81b65d142865ef5dbb2df2e98c084dc995272e55f804a36f283c6f9cc0a`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.3 MB (4262063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ead6720a64b98a3aff60731463b608c0b67ecd6e1da5fdea16027f2602fed35`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.2 MB (4234751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d902f277ddd72c79a705e87198d386aa6f00888bd94535ac236140f709bbdce`  
		Last Modified: Thu, 16 Mar 2023 03:50:57 GMT  
		Size: 43.8 MB (43768451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e52f20a783e0f77850e23839602213aca9d779491820b6b87d582377010ff1`  
		Last Modified: Thu, 16 Mar 2023 03:51:51 GMT  
		Size: 183.9 MB (183869878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d8f68fa9506203d2ae62c96ff52ca734da392b0abdf6fb87d0b095d32da75234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223696064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:027fabc11727fa0a1d019f1c51338d85905a5113cdc2c03b8c1fbb1f2a852c17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:49:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:50:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:52:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfb18fcfcf98f525d6770606600d80d5413262ce3575995b49064988c1bd147`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.8 MB (3792844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072af6d5dacbd70c88a5e91a5627fe4a95af544c4db1b250a263452128dc9cab`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.5 MB (3472886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b80aecb29fcddae2ca64d4c31faa682b41b3206400c727d5eec25c7d83c8630`  
		Last Modified: Thu, 16 Mar 2023 02:02:54 GMT  
		Size: 39.3 MB (39284857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277c8fbd8d44bf1475a44df6398ba9159c13423417cffb98f23824dca61b4a1d`  
		Last Modified: Thu, 16 Mar 2023 02:03:19 GMT  
		Size: 148.5 MB (148497878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:1950ad34a10c685de875a9d2f586a239612590e033635f7ca3b07cd333c35d88
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
$ docker pull buildpack-deps@sha256:e1f00c6daf4cd328bbef9c52e6c60f18a47e5b716ef5a5d78542c90635025d20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37780234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb7e40d800141c3758097d639c8f71da7d755a34a9ce59dabba14aac2a540ee`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:29:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:29:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7490ba7e16ba382ca21015280e2ee6dad31879a1f043029e350a8e429770f36`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.8 MB (3788671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeb23ea57c359eecf9e21c40ddb69f738e9121008fd4956d733ba66d3b7eb38`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.6 MB (3561600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d14e02d71154d77fa15e8fe99c09399a29cf9cd6a168b06bf6cfdc6cbdd98960
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34279939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:831a4c6176514fb8d4452ddac355efa1a3da26e98087da273d6c3bcc34ba38e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:51:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:51:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d54aa809ca004a01d3a10bf7017a1fb216f185fd9d0f210f1bc9512298c1`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.5 MB (3540124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caec72904127d7cb95dfd39a3f311865b026d929e1440427ec21122be6e15db3`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.7 MB (3714418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fa825f78772b21eb6d058d2d80e48ded564c870a66ec077b8219225d6f515c2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35684245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd233dec7831ce72a921837b590af2d1f8f8d87f1b119fae78edba2ea730316`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:08:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aef66b301cbfe4ff1bb09357ccf381140239a236438d27a992d076491a3a066`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.8 MB (3760501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693278d975de74bdcb529fd46771b1335b9501b8f479a3c8128b69375f7945a8`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.5 MB (3536190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:057ed8d3115324cc3a7cbde4dad9bc42768a3cfeeb98aa5a2342d57a704ea2b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44208542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d825634c6ab1942263dbe9f71d6b27d39b833fb4013c32ad433760b35351762d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda6a81b65d142865ef5dbb2df2e98c084dc995272e55f804a36f283c6f9cc0a`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.3 MB (4262063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ead6720a64b98a3aff60731463b608c0b67ecd6e1da5fdea16027f2602fed35`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.2 MB (4234751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b22525cdcb82e2ef5355054b43872f265a7e983b5de76a9606921cde9d74b610
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35913329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a514140debee8dd2b4218d8d1975fc7b1e4623707f2083cffa6cdbd3f7e11228`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:49:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfb18fcfcf98f525d6770606600d80d5413262ce3575995b49064988c1bd147`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.8 MB (3792844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072af6d5dacbd70c88a5e91a5627fe4a95af544c4db1b250a263452128dc9cab`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.5 MB (3472886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:79b0f9319ebb640493eaf8539641f9fc67a08f10ec5fc2f8a7d9a447fd786055
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
$ docker pull buildpack-deps@sha256:f34fd3d1a17609e88da35bc2a959ddd09a4cff838e251132a6a4551b7f710a8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77133144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e9805e59e9e583a30a563cbac116296ba8acf152f10fabcbecc2d3f99f8b6ab`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:29:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:29:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:29:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7490ba7e16ba382ca21015280e2ee6dad31879a1f043029e350a8e429770f36`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.8 MB (3788671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeb23ea57c359eecf9e21c40ddb69f738e9121008fd4956d733ba66d3b7eb38`  
		Last Modified: Thu, 16 Mar 2023 05:43:15 GMT  
		Size: 3.6 MB (3561600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c00a0ea05e6a2089233e7238bbed0ffbf7b2655f03195967e2083ee623899`  
		Last Modified: Thu, 16 Mar 2023 05:43:30 GMT  
		Size: 39.4 MB (39352910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8249c9a5f7475ad02f242ade08a27052609481d8cd35ae4089fa7ecb14295c45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76188259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b7c6edcb5acd77a3e2b70af5afcda9bef5dcb2ee9c21e24297ee96426322b6e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:51:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:51:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:52:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d54aa809ca004a01d3a10bf7017a1fb216f185fd9d0f210f1bc9512298c1`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.5 MB (3540124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caec72904127d7cb95dfd39a3f311865b026d929e1440427ec21122be6e15db3`  
		Last Modified: Thu, 16 Mar 2023 04:09:39 GMT  
		Size: 3.7 MB (3714418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b259dc20995aa828e48008def151ea3da6891615621976f66dc6b63fdbda38a`  
		Last Modified: Thu, 16 Mar 2023 04:09:57 GMT  
		Size: 41.9 MB (41908320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6857aefe9fc47abf0d2d28e21e046b63e6be875de53f2b1fd49dea88192e4560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74927866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9591d5aa5d0b25f21dfa798fa26b330206f083d8ca36701124b4a875b6c2c4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:08:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:08:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aef66b301cbfe4ff1bb09357ccf381140239a236438d27a992d076491a3a066`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.8 MB (3760501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693278d975de74bdcb529fd46771b1335b9501b8f479a3c8128b69375f7945a8`  
		Last Modified: Thu, 16 Mar 2023 04:23:23 GMT  
		Size: 3.5 MB (3536190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfc2e7bfd914b57fdeae1d187ca7a12534443f9e2a6142287dab73c0296ade8`  
		Last Modified: Thu, 16 Mar 2023 04:23:36 GMT  
		Size: 39.2 MB (39243621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d8da9e38d3c74aa25f5da85d9e692795099198656dfb38ba3058d5cc1c3284d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87976993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a899652169ee26f65829047e0799b9409330896911f49369b3b425b1315c02b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:24:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda6a81b65d142865ef5dbb2df2e98c084dc995272e55f804a36f283c6f9cc0a`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.3 MB (4262063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ead6720a64b98a3aff60731463b608c0b67ecd6e1da5fdea16027f2602fed35`  
		Last Modified: Thu, 16 Mar 2023 03:50:35 GMT  
		Size: 4.2 MB (4234751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d902f277ddd72c79a705e87198d386aa6f00888bd94535ac236140f709bbdce`  
		Last Modified: Thu, 16 Mar 2023 03:50:57 GMT  
		Size: 43.8 MB (43768451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9b906aa81cc60290a664f0ff6bcb0f491cac7dd31f6cc7fbb73f4f2823d84ca0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75198186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:accf40ea7a4019526a1b76f2c48458f738926fa6bb6f285ca24c9c03b98771ed`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:49:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:50:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfb18fcfcf98f525d6770606600d80d5413262ce3575995b49064988c1bd147`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.8 MB (3792844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072af6d5dacbd70c88a5e91a5627fe4a95af544c4db1b250a263452128dc9cab`  
		Last Modified: Thu, 16 Mar 2023 02:02:37 GMT  
		Size: 3.5 MB (3472886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b80aecb29fcddae2ca64d4c31faa682b41b3206400c727d5eec25c7d83c8630`  
		Last Modified: Thu, 16 Mar 2023 02:02:54 GMT  
		Size: 39.3 MB (39284857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:175fb2896f655cccf6e13731e9e6d786c9c69630240717433c43d615958e67a3
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
$ docker pull buildpack-deps@sha256:6e3f3abbace0fcfb2e2393b134bb14479e39d5f78d9cfb25875150cbdcee2887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.8 MB (258751145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab725b6129919899348d2631b8bccdf236f9217de9abad4c65d0db0e544d4cd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:05 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:07 GMT
ADD file:3492508b382c909e968c4d8467b9acbd5f61ed6ca69c8a47241f930d90de7158 in / 
# Wed, 08 Mar 2023 05:58:07 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:33:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:33:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:34:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:36:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17a407a0ba4a4df07961f83dc5f45a6167aef7c4f6ca31fb67cb40abd601132d`  
		Last Modified: Thu, 16 Mar 2023 05:44:13 GMT  
		Size: 27.5 MB (27482092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3ce1e417f7729d7a549758b735166f99e55a7991459164e9a2cdee45bf49a4`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 6.8 MB (6770607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7f86ef9e483dabe62f207ba172ab1901264fcb5d62bd81ef5221c8ce9d67b3`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 3.6 MB (3635351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c5edfb2bc00433326244b5dd4da0315012e82e1b065c452afd8f40148f3180`  
		Last Modified: Thu, 16 Mar 2023 05:44:28 GMT  
		Size: 39.7 MB (39740353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6dbdd9f6c26e43b8b352fa3493515965ff36d7b264eb1458b635d095f086e`  
		Last Modified: Thu, 16 Mar 2023 05:45:00 GMT  
		Size: 181.1 MB (181122742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:962f9fa1a90ddfb86df762aa441ae2acbadf5a937ad2d29897e0eecae5e45c79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221867223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c52237c7765716061da64dd0c0e9e6c1a561f72d56a75d92470700609eb300b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:55:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:55:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:55:49 GMT
ADD file:827330b6c59e67c5d2edd3ceb3492b97865b15f9246f14710f478d12e94d2048 in / 
# Wed, 08 Mar 2023 05:55:49 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:56:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:57:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6408fcff70bde57e1c23e7502a9476939cc569e2eff3e9e9adca350cb5b4dac1`  
		Last Modified: Thu, 16 Mar 2023 04:10:41 GMT  
		Size: 25.9 MB (25890803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467248c617f5da80617561605e184647a03bc6ee0731094ea5fa1a10a9d97d12`  
		Last Modified: Thu, 16 Mar 2023 04:10:38 GMT  
		Size: 5.9 MB (5941308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084ed064758ff6efc72c5bfa16404dd5e5a7196c6704c9bfce54fffbe511f026`  
		Last Modified: Thu, 16 Mar 2023 04:10:37 GMT  
		Size: 3.8 MB (3801366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4d5295b37133c15e99cf4caa18ed1036eb41e583b687ff4e31eeb39287307d`  
		Last Modified: Thu, 16 Mar 2023 04:10:58 GMT  
		Size: 42.6 MB (42608451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b2ee1d700f51191bf1f9fda529c4cc2b75e353b7a936061fd2fe96c9f78678`  
		Last Modified: Thu, 16 Mar 2023 04:11:28 GMT  
		Size: 143.6 MB (143625295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:146ce1a60825f205a892808cd7a290d6b1a6e5898ad0d9210c66123d35dfe859
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.7 MB (246723891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2280a8119a9d7647830181ac7ce5e7c0e62f3a61d806d7003efd469a9f943063`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:57:57 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:57:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:57:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:57:58 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:57:59 GMT
ADD file:884e00dc91bf6d392fa3d117913cc2534177128322d89137bfb8b2734bc38579 in / 
# Wed, 08 Mar 2023 05:58:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:12:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:16:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:254a784e837e29e485a63351d1a7aba22a34cad2c55e16264bd25ec0add89463`  
		Last Modified: Thu, 16 Mar 2023 04:24:12 GMT  
		Size: 26.7 MB (26703428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5262eba6308f5bd6759d8fe45a1d30f1c39e36af3ffc10b11c84e335e3cf5`  
		Last Modified: Thu, 16 Mar 2023 04:24:10 GMT  
		Size: 6.6 MB (6600337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d93a07df4f2da69d3c85f944e8fa42f4e401cfb09edbff605d5863469a8c37`  
		Last Modified: Thu, 16 Mar 2023 04:24:09 GMT  
		Size: 3.6 MB (3604205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c46f9dfcefdff9c3932f840ec8ab4bf6808e7f4ade97eaf2a7ff68143dc8ac6`  
		Last Modified: Thu, 16 Mar 2023 04:24:25 GMT  
		Size: 39.5 MB (39516410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84953c5033e8f35541798119d0992d31f9b11c41d8790751581f9da4f03c7ff9`  
		Last Modified: Thu, 16 Mar 2023 04:24:51 GMT  
		Size: 170.3 MB (170299511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:06669921677d024d21c8b5bf374e4c76980db68187ef23ed12b774f09cc2e817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281308399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d473e407ad7791542b97cc0a0c2d858cd32beea41851e3dd56e8bdba1362ef37`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:03 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:06 GMT
ADD file:583061e8201c03de4747860e734200b6c35b449443a1382ad8e8efc6f7e9ea13 in / 
# Wed, 08 Mar 2023 05:58:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:30:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:31:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:36:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ec1f8fff860753bb5de879722c39643b2fecee25466efe51120479c4cd7647f`  
		Last Modified: Thu, 16 Mar 2023 03:52:17 GMT  
		Size: 32.1 MB (32098861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00fc14ce944c08bb40e1940367da097dd6113e4621903eedbeb83cf9caea6cc`  
		Last Modified: Thu, 16 Mar 2023 03:52:08 GMT  
		Size: 7.7 MB (7748081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75e7525a0f6794b3368a8aecf0b1c8c88ab38a7de79a51f2cc03b69581df2f`  
		Last Modified: Thu, 16 Mar 2023 03:52:07 GMT  
		Size: 4.4 MB (4362802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181a3a7eb1466bfe41561019eef321a775ae9583da803da64216210ccba3f91d`  
		Last Modified: Thu, 16 Mar 2023 03:52:39 GMT  
		Size: 44.1 MB (44142002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c199734d8e3b9bc7a3c36814098b8d531785794c938276dc46411ec36cdb0d`  
		Last Modified: Thu, 16 Mar 2023 03:53:36 GMT  
		Size: 193.0 MB (192956653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5b34f6d4e61a65640b7b2c4ebfea0b28a3aa10a05e87019ea523c5d3597d47a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228629856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597b8cfc1db04a45533b44e8f28ad50b5fc7e01b8423c09757ed1daeb251d21c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 06:11:04 GMT
ARG RELEASE
# Wed, 08 Mar 2023 06:11:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 06:11:06 GMT
ADD file:974d67ca1d5bcaacbc707820609d36af0d7ed3ff7179a702a4aa56dcc43f79f3 in / 
# Wed, 08 Mar 2023 06:11:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:53:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:53:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:55:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e94c7036e7dc9a2d6666b2f4fc00019c0540bd3edd16e54289a9d6b7134b349`  
		Last Modified: Thu, 16 Mar 2023 02:03:35 GMT  
		Size: 26.0 MB (26029370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc60d216fdfa5dd36e7941c80e0ea9d1b8c692a8c067ad512585b6ae40bd6e99`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 6.5 MB (6461878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c257c035538e42c9fb24b73041a70d92b99378d720c80bc418d8ed7900e2d15c`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 3.6 MB (3625230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2543f565e0a12ed697a188c8d0c2e00c8788a6dee791dbf852c2b335985834`  
		Last Modified: Thu, 16 Mar 2023 02:03:48 GMT  
		Size: 39.6 MB (39559711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a414ee64d952ecb156be9cb912b41983739a5bd309bf9db2c7cc6cba5ffdc2`  
		Last Modified: Thu, 16 Mar 2023 02:04:16 GMT  
		Size: 153.0 MB (152953667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:82f90458af310619116662064c4a1bfd08da721e3ac46a1452047c268517fde0
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
$ docker pull buildpack-deps@sha256:4a0ea70e27ab3ee9d260740e1e11ef06f009589299eaa372b3313a5d617480bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37888050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83a06332258b828506b4757d4fa816eb9f29440d4e56282a9a38e120f33cd5c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:05 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:07 GMT
ADD file:3492508b382c909e968c4d8467b9acbd5f61ed6ca69c8a47241f930d90de7158 in / 
# Wed, 08 Mar 2023 05:58:07 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:33:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:33:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:17a407a0ba4a4df07961f83dc5f45a6167aef7c4f6ca31fb67cb40abd601132d`  
		Last Modified: Thu, 16 Mar 2023 05:44:13 GMT  
		Size: 27.5 MB (27482092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3ce1e417f7729d7a549758b735166f99e55a7991459164e9a2cdee45bf49a4`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 6.8 MB (6770607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7f86ef9e483dabe62f207ba172ab1901264fcb5d62bd81ef5221c8ce9d67b3`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 3.6 MB (3635351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4af883c5eab3c2380a46236ca3ca95f3048243965b2e897814c48e8260dfa2c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35633477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094d55cec9f8dc3d95b8ee21b11560284d162a4571f93b0b44109e9fe8e3d0cc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:55:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:55:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:55:49 GMT
ADD file:827330b6c59e67c5d2edd3ceb3492b97865b15f9246f14710f478d12e94d2048 in / 
# Wed, 08 Mar 2023 05:55:49 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:56:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6408fcff70bde57e1c23e7502a9476939cc569e2eff3e9e9adca350cb5b4dac1`  
		Last Modified: Thu, 16 Mar 2023 04:10:41 GMT  
		Size: 25.9 MB (25890803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467248c617f5da80617561605e184647a03bc6ee0731094ea5fa1a10a9d97d12`  
		Last Modified: Thu, 16 Mar 2023 04:10:38 GMT  
		Size: 5.9 MB (5941308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084ed064758ff6efc72c5bfa16404dd5e5a7196c6704c9bfce54fffbe511f026`  
		Last Modified: Thu, 16 Mar 2023 04:10:37 GMT  
		Size: 3.8 MB (3801366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f7410e86839d94189da0421368263daad23e4532602532ebebb243959a6589bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36907970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11201af935ca582771cd9c1d5a25562f6956d2d83b5561f776ff20235996f3a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:57:57 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:57:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:57:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:57:58 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:57:59 GMT
ADD file:884e00dc91bf6d392fa3d117913cc2534177128322d89137bfb8b2734bc38579 in / 
# Wed, 08 Mar 2023 05:58:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:12:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:254a784e837e29e485a63351d1a7aba22a34cad2c55e16264bd25ec0add89463`  
		Last Modified: Thu, 16 Mar 2023 04:24:12 GMT  
		Size: 26.7 MB (26703428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5262eba6308f5bd6759d8fe45a1d30f1c39e36af3ffc10b11c84e335e3cf5`  
		Last Modified: Thu, 16 Mar 2023 04:24:10 GMT  
		Size: 6.6 MB (6600337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d93a07df4f2da69d3c85f944e8fa42f4e401cfb09edbff605d5863469a8c37`  
		Last Modified: Thu, 16 Mar 2023 04:24:09 GMT  
		Size: 3.6 MB (3604205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6760f29c9bdcdc308fcf3afb3ca98c719d1c0c3e8c5a5bea33cc33c3db2550d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44209744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14fbb219e4d625d407f193f60f7c075595d470a92f731343a064f26b3a6c72a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:03 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:06 GMT
ADD file:583061e8201c03de4747860e734200b6c35b449443a1382ad8e8efc6f7e9ea13 in / 
# Wed, 08 Mar 2023 05:58:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:30:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6ec1f8fff860753bb5de879722c39643b2fecee25466efe51120479c4cd7647f`  
		Last Modified: Thu, 16 Mar 2023 03:52:17 GMT  
		Size: 32.1 MB (32098861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00fc14ce944c08bb40e1940367da097dd6113e4621903eedbeb83cf9caea6cc`  
		Last Modified: Thu, 16 Mar 2023 03:52:08 GMT  
		Size: 7.7 MB (7748081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75e7525a0f6794b3368a8aecf0b1c8c88ab38a7de79a51f2cc03b69581df2f`  
		Last Modified: Thu, 16 Mar 2023 03:52:07 GMT  
		Size: 4.4 MB (4362802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d2366f9c8542e47115c50c026f6cf9ccda7aaf6b859307b5ca9f1f1c0cf8a50b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36116478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ee7ee58323c7f6349967f769687f47de069565561ee8264351d32a8d0ecd22e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 06:11:04 GMT
ARG RELEASE
# Wed, 08 Mar 2023 06:11:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 06:11:06 GMT
ADD file:974d67ca1d5bcaacbc707820609d36af0d7ed3ff7179a702a4aa56dcc43f79f3 in / 
# Wed, 08 Mar 2023 06:11:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:53:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3e94c7036e7dc9a2d6666b2f4fc00019c0540bd3edd16e54289a9d6b7134b349`  
		Last Modified: Thu, 16 Mar 2023 02:03:35 GMT  
		Size: 26.0 MB (26029370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc60d216fdfa5dd36e7941c80e0ea9d1b8c692a8c067ad512585b6ae40bd6e99`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 6.5 MB (6461878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c257c035538e42c9fb24b73041a70d92b99378d720c80bc418d8ed7900e2d15c`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 3.6 MB (3625230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:aa76817af3e5497173c1e3d3e67c0365b99897e5b1e315ac4910b2920c424f95
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
$ docker pull buildpack-deps@sha256:e6378630b29880479224ed0c4d5c760022695b18656bb1a04f7ee4c840c365fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77628403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4098822eb5aa2de33de31a2e39c977e7c97b73cb3d43bf8ad263135afdc338a7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:05 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:07 GMT
ADD file:3492508b382c909e968c4d8467b9acbd5f61ed6ca69c8a47241f930d90de7158 in / 
# Wed, 08 Mar 2023 05:58:07 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:33:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:33:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:34:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17a407a0ba4a4df07961f83dc5f45a6167aef7c4f6ca31fb67cb40abd601132d`  
		Last Modified: Thu, 16 Mar 2023 05:44:13 GMT  
		Size: 27.5 MB (27482092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3ce1e417f7729d7a549758b735166f99e55a7991459164e9a2cdee45bf49a4`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 6.8 MB (6770607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7f86ef9e483dabe62f207ba172ab1901264fcb5d62bd81ef5221c8ce9d67b3`  
		Last Modified: Thu, 16 Mar 2023 05:44:09 GMT  
		Size: 3.6 MB (3635351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c5edfb2bc00433326244b5dd4da0315012e82e1b065c452afd8f40148f3180`  
		Last Modified: Thu, 16 Mar 2023 05:44:28 GMT  
		Size: 39.7 MB (39740353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:90515c216502433efbdc090e03b1210bf49d905412b2c6c1d721854daf004502
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78241928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de12f85f2fcdabf5af043eb805c6ed21fdfbdfac456a33d4e17ae057800a5a0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:55:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:55:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:55:49 GMT
ADD file:827330b6c59e67c5d2edd3ceb3492b97865b15f9246f14710f478d12e94d2048 in / 
# Wed, 08 Mar 2023 05:55:49 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:56:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:57:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6408fcff70bde57e1c23e7502a9476939cc569e2eff3e9e9adca350cb5b4dac1`  
		Last Modified: Thu, 16 Mar 2023 04:10:41 GMT  
		Size: 25.9 MB (25890803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467248c617f5da80617561605e184647a03bc6ee0731094ea5fa1a10a9d97d12`  
		Last Modified: Thu, 16 Mar 2023 04:10:38 GMT  
		Size: 5.9 MB (5941308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084ed064758ff6efc72c5bfa16404dd5e5a7196c6704c9bfce54fffbe511f026`  
		Last Modified: Thu, 16 Mar 2023 04:10:37 GMT  
		Size: 3.8 MB (3801366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4d5295b37133c15e99cf4caa18ed1036eb41e583b687ff4e31eeb39287307d`  
		Last Modified: Thu, 16 Mar 2023 04:10:58 GMT  
		Size: 42.6 MB (42608451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7ea350ea72f5dc34447ad0ad32230ca304a8954c691d5e2219aeb1c3d33dd977
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76424380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc47c377e953ab11b6623e2d24bbe50bdb550a956e97f3bf19941a13663ae09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:57:57 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:57:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:57:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:57:58 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:57:59 GMT
ADD file:884e00dc91bf6d392fa3d117913cc2534177128322d89137bfb8b2734bc38579 in / 
# Wed, 08 Mar 2023 05:58:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:12:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:12:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:254a784e837e29e485a63351d1a7aba22a34cad2c55e16264bd25ec0add89463`  
		Last Modified: Thu, 16 Mar 2023 04:24:12 GMT  
		Size: 26.7 MB (26703428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5262eba6308f5bd6759d8fe45a1d30f1c39e36af3ffc10b11c84e335e3cf5`  
		Last Modified: Thu, 16 Mar 2023 04:24:10 GMT  
		Size: 6.6 MB (6600337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d93a07df4f2da69d3c85f944e8fa42f4e401cfb09edbff605d5863469a8c37`  
		Last Modified: Thu, 16 Mar 2023 04:24:09 GMT  
		Size: 3.6 MB (3604205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c46f9dfcefdff9c3932f840ec8ab4bf6808e7f4ade97eaf2a7ff68143dc8ac6`  
		Last Modified: Thu, 16 Mar 2023 04:24:25 GMT  
		Size: 39.5 MB (39516410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:47814ff7d3d0680f98234b1b77e52c20623de4ea381d7d64b45058c0420e3b98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88351746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6520324913b2522ab60f497720b420e064788b9c36489fc9db9df6e7ccd90d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:03 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:06 GMT
ADD file:583061e8201c03de4747860e734200b6c35b449443a1382ad8e8efc6f7e9ea13 in / 
# Wed, 08 Mar 2023 05:58:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:30:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:31:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ec1f8fff860753bb5de879722c39643b2fecee25466efe51120479c4cd7647f`  
		Last Modified: Thu, 16 Mar 2023 03:52:17 GMT  
		Size: 32.1 MB (32098861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00fc14ce944c08bb40e1940367da097dd6113e4621903eedbeb83cf9caea6cc`  
		Last Modified: Thu, 16 Mar 2023 03:52:08 GMT  
		Size: 7.7 MB (7748081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75e7525a0f6794b3368a8aecf0b1c8c88ab38a7de79a51f2cc03b69581df2f`  
		Last Modified: Thu, 16 Mar 2023 03:52:07 GMT  
		Size: 4.4 MB (4362802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181a3a7eb1466bfe41561019eef321a775ae9583da803da64216210ccba3f91d`  
		Last Modified: Thu, 16 Mar 2023 03:52:39 GMT  
		Size: 44.1 MB (44142002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9bbf357cfc90c5b3effb70b70ec060ca6b1b3e1a6867604c88d94fbbbe77399d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75676189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e90e10986384324d54a15fec854faff368bcba346fce3c6b1ff80c08f0998a0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 06:11:04 GMT
ARG RELEASE
# Wed, 08 Mar 2023 06:11:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 06:11:06 GMT
ADD file:974d67ca1d5bcaacbc707820609d36af0d7ed3ff7179a702a4aa56dcc43f79f3 in / 
# Wed, 08 Mar 2023 06:11:06 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:53:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:53:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e94c7036e7dc9a2d6666b2f4fc00019c0540bd3edd16e54289a9d6b7134b349`  
		Last Modified: Thu, 16 Mar 2023 02:03:35 GMT  
		Size: 26.0 MB (26029370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc60d216fdfa5dd36e7941c80e0ea9d1b8c692a8c067ad512585b6ae40bd6e99`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 6.5 MB (6461878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c257c035538e42c9fb24b73041a70d92b99378d720c80bc418d8ed7900e2d15c`  
		Last Modified: Thu, 16 Mar 2023 02:03:32 GMT  
		Size: 3.6 MB (3625230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2543f565e0a12ed697a188c8d0c2e00c8788a6dee791dbf852c2b335985834`  
		Last Modified: Thu, 16 Mar 2023 02:03:48 GMT  
		Size: 39.6 MB (39559711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:422b4400e1ae3a5aa208dc236e3dc05e3db66b72387ac2d7b11bee187ff87f7d
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
$ docker pull buildpack-deps@sha256:4156d4c78d3e29a9aa11a5528a08847352e66895bb0a75cec05f4d43752fb8f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322492485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09bd8b383fcae8260115c949f68a3ccbe1df72567c4e1ad6f53b72329c1c5e1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b89f3c7f7da8adf032a33a75d1b659cee33179ecb88ea0ba75e4fc58ebe63a6`  
		Last Modified: Wed, 12 Apr 2023 07:57:46 GMT  
		Size: 54.6 MB (54584801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d62772179761f8fddfaed03ed2bdf7078b103b193d18d79a9b49364830d56cf`  
		Last Modified: Wed, 12 Apr 2023 07:58:19 GMT  
		Size: 196.8 MB (196811503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:5307e4d5147eb64f430d2a521eee4a5504ed8c4a0d7d98aa81c28190c2c963d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295551904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62bc4c385631ea22e58568f3c02e7102b4f9f8f5a1ebb96d7e82bf8764dbecae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:15:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:16:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:17:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49db155cdf8645f599affcbbbc75eb928b0a9d010c4ac54afcfa9d7e4fa85e0`  
		Last Modified: Wed, 12 Apr 2023 01:21:15 GMT  
		Size: 5.1 MB (5072827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936087cbd048148575fda58348506149db80a2699e99ae2042086628c0e5a38`  
		Last Modified: Wed, 12 Apr 2023 01:21:16 GMT  
		Size: 10.6 MB (10573853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0bf11569c39ee4f3d8515112046a55f14f39e54c6f0ea26271033c090f77d2`  
		Last Modified: Wed, 12 Apr 2023 01:21:35 GMT  
		Size: 52.3 MB (52340617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622390f39404d88752f248bc2136a55baca97d5324d43689204df0157d284282`  
		Last Modified: Wed, 12 Apr 2023 01:22:13 GMT  
		Size: 175.0 MB (175009432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f9e1d777129a6edd74d7bf1c46bceacdb0494da93b4f6f30b9e3e1ddc047be34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (283008120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49b8799c6deee224d45f54f351a870631cfae0b6039cfe91ea6c3adf9a1810e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:41:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca667140ff247fc759283fc9ff4cafbe304d1777ffc70e1bd593b63151c31a`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 4.9 MB (4934357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879c254431e9965afb23e55a148faffd29450a9218269f769be95d6e9673a93`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 10.2 MB (10217859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64c4a1b9916f6da6f286835522f27f11a812694e5f878e87468d4c6b90b343e`  
		Last Modified: Thu, 23 Mar 2023 12:45:20 GMT  
		Size: 50.4 MB (50355514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862d41b96b9b8c37267f9bb50226c9d63fc5a8df2310f511837355e187e090a`  
		Last Modified: Thu, 23 Mar 2023 12:45:51 GMT  
		Size: 167.3 MB (167288602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e7277cb741804ffe9213d32a419f6738ef4494fbd33db9326b55282dfbc1dd6b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.1 MB (314135667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c57708eddbf78525fe399f52d71e35653f6c3298641025d07fcc3323777584`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:07:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f993d5b17f32f4b8a535c25e182e5d8412625beee450e513ca57036e8fdd6dc`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 54.7 MB (54676038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26edf98ece5babdb6b65e76738cef2c2d05e7075161753d3ba95cd84480d211`  
		Last Modified: Wed, 12 Apr 2023 01:14:02 GMT  
		Size: 189.7 MB (189727693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ff274b300c58e39b8abdacecdee25d47651abe32a696616b92656ca392bd5d21
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.2 MB (328223380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5eee57e4ddbeaa9219392349db2bc711541f424d58a97b4a86ad5bd768ff773`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:06:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:07:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ccf9a5e34ba2345ce265a9a11c93ee254e1f3616dfd1c1deda6e2f7d614c8`  
		Last Modified: Wed, 12 Apr 2023 01:14:53 GMT  
		Size: 5.3 MB (5293626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4988d5e4328f031f6884a7351766aa8a2806c9cdca38d354477fc537eaa4911f`  
		Last Modified: Wed, 12 Apr 2023 01:14:54 GMT  
		Size: 11.2 MB (11249875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660a2befd486d43a308dd1561f57efeafe1f13defd6439d34aeb5efec783ee3d`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 55.9 MB (55922746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f09985282f12d05c5724bcbb0481a94f66820112bafc34a1d990dfdf74a52fc`  
		Last Modified: Wed, 12 Apr 2023 01:16:02 GMT  
		Size: 199.7 MB (199724315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ec42db429d0c72964b3b977754bc6918c60d4bf420eae2d6e4a643f9213a7305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301083947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537e8272f594cfb2548e2fb1974050af3569e7a7791f1ed883845f968edd9f25`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:15:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:21:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f79f6951926609a68e21aee7e612375637f7c12703c62b028fd60a22e2d9bfd`  
		Last Modified: Thu, 23 Mar 2023 07:34:02 GMT  
		Size: 4.9 MB (4922133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b6297024241cbdae60b7afa1bce7cc669d998e17b209e8b133df9e13da064`  
		Last Modified: Thu, 23 Mar 2023 07:34:04 GMT  
		Size: 10.7 MB (10662010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9437ab03a3b730ed3d31f18a79500c8ce379f2a971ed27695d60f38e887121b2`  
		Last Modified: Thu, 23 Mar 2023 07:34:50 GMT  
		Size: 53.3 MB (53306810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173435a2410e4cdc681e9bd4a44f44da5e7905b9826d94efbc91429ed38126f1`  
		Last Modified: Thu, 23 Mar 2023 07:36:46 GMT  
		Size: 178.9 MB (178928274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:474394b72495ae1d639248919c45100c0ee19cbc80fb7c3c85583baff857f075
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330989722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021c337c98a3039aa29eead547f736d517042181f44162b2088727645ce4a56f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:15:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:16:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:18:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805b891b319592a15b7da9a474b2f36e32ed9b8a720d14bbbe4d08422343b19`  
		Last Modified: Thu, 23 Mar 2023 13:24:55 GMT  
		Size: 5.4 MB (5415174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdb7e2b62c4c7c555894be507d7ccaf7aeca0f8c9088a9082ad4cd37dc97f28`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 11.6 MB (11629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac3f4f172050b21a6f17c30c60794779e7d5c150f1111240477b89240ad7f6`  
		Last Modified: Thu, 23 Mar 2023 13:25:22 GMT  
		Size: 58.9 MB (58864543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2fa2e478c864805494dbe6350071ba59af5a4f830abf55dc17559fb0228fa`  
		Last Modified: Thu, 23 Mar 2023 13:26:19 GMT  
		Size: 196.2 MB (196159312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:478709c66fdeffea827bb22297605067d97172933185294b18da02b3b071e7a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296079415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62811c5341c95a39adc789318a1ba301b0fae01b6b77e3b4a63a1693c43fa76d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:27:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2973b8c98f9da7833ab9cd69185dd958a8939a30136cdcfedb66ce775db358ee`  
		Last Modified: Wed, 12 Apr 2023 00:32:48 GMT  
		Size: 5.1 MB (5149313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f740d13ac612bf8b6489559a7945ec1439fee2d5eba455ab0db047cd3f30a9a`  
		Last Modified: Wed, 12 Apr 2023 00:32:49 GMT  
		Size: 10.8 MB (10766104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c0067783f401b099adca196dce9e464e66236e49faba106e2f04ac73a90df7`  
		Last Modified: Wed, 12 Apr 2023 00:33:02 GMT  
		Size: 54.1 MB (54061843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b5accdd9fd68a290692e1a0a3d853312f236ae0463540b5fdd97d598cc7a6`  
		Last Modified: Wed, 12 Apr 2023 00:33:28 GMT  
		Size: 172.8 MB (172815473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar`

```console
$ docker pull buildpack-deps@sha256:560e0088301609081b9f373dec446d2e62c1a2d6649abeb3fcc344e1e47bf596
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
$ docker pull buildpack-deps@sha256:287222a734407093da8bd5d1aa36fbb68ec0bedd34f5d3d6c953369ee20930b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.8 MB (265813027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81d6e1c88be1ef8bc7e4711555c9bc2801e4ae6d1ba36047cc5ccfc957d722a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:37:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:37:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:40:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbd9104be902889dc21019a0f5023f798f3d4659871b7eff4e60ea6f1496df08`  
		Last Modified: Thu, 16 Mar 2023 05:45:13 GMT  
		Size: 27.5 MB (27533123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926546ac77ef389dea10f2f48a9435499b9fd85ce007f054787873fba3ba820`  
		Last Modified: Thu, 16 Mar 2023 05:45:10 GMT  
		Size: 6.7 MB (6653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e02fdac0efdc0f5d71c45d6ab71b8cf2421156adfbe3dd6673c198b60f5e696`  
		Last Modified: Thu, 16 Mar 2023 05:45:09 GMT  
		Size: 3.7 MB (3689653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57775961ac4b5f4df9ba21c9a454eec60eced52106a9c3c6480abe04fd31e975`  
		Last Modified: Thu, 16 Mar 2023 05:45:29 GMT  
		Size: 44.3 MB (44251085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d411862c594e5099f7d047ca155efc294f71792fc959ab9aa3e07e449b5f29ae`  
		Last Modified: Thu, 16 Mar 2023 05:46:00 GMT  
		Size: 183.7 MB (183685294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:155908323c4e07137e4866c58870f6590c6de3ca0b3cbd687cd8ec6672e62b57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.4 MB (230430758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86991c1a884508bddd7bad77896595630d8d44bf3cfe5080600a260675f86e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:01:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:04:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2e2ff6a76c080ab34fadea2f47efdf4e1606b1482ed2e4597e51810a467b28a`  
		Last Modified: Thu, 16 Mar 2023 04:11:42 GMT  
		Size: 25.4 MB (25359548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003fc5922aae3f4274356fca42181568c983c95440b266598d0a8b3307f981b3`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 5.8 MB (5819049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f573392ff6ba3d538b9dd78eaac78c3a48a8719f2c3a366e5031c24433553af7`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 3.9 MB (3850947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e5edf4553807d09a5e079189ad8abe94fa20ac8d3b91a1fdee74ffbbfc465a`  
		Last Modified: Thu, 16 Mar 2023 04:12:00 GMT  
		Size: 48.3 MB (48335132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4f27e394d3d3e059ce90e3503f32ac8d096f2652745ce86e56fa4bb4b25ab5`  
		Last Modified: Thu, 16 Mar 2023 04:12:30 GMT  
		Size: 147.1 MB (147066082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e9b21ae0c7c9575c3bdbcc4e38e37afc2bf155d4304484b260fc63b65decc3d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.0 MB (255963478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c30df20c0e7ce6c6b1e087b68175313ed2ed3632a7707c2078dd03a949b607b9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:17:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:20:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bd94ab779df0c538759342d8eef230b315e98979bcac4604e94fb874397461b`  
		Last Modified: Thu, 16 Mar 2023 04:25:04 GMT  
		Size: 26.9 MB (26945660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df8402fa00c99b6f8233d0c6452e59cfe2742b9b2c9f44a504aaa45a0516cd3`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 6.5 MB (6484575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa45039d5b2736a9624493cbbbf9200c134de7ddb8696ce87c68dad417e12f4`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 3.6 MB (3648517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5195e2054b68f924f77b2db71706b518fdc87c9c6f3d900adad8e6eec601fb`  
		Last Modified: Thu, 16 Mar 2023 04:25:18 GMT  
		Size: 44.1 MB (44054619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afa7d18844d07a4d0a59be44ee5dfea5fae8e0ed488bf7cd0a5c87e6b4ab3cc`  
		Last Modified: Thu, 16 Mar 2023 04:25:44 GMT  
		Size: 174.8 MB (174830107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3f87acc02cf05e895c5cdca40f10af0846f6beef7f7d0d413e64336ebe514f6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.1 MB (290142434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e375ebe6881fcb8e14ab34fd4f73359da22f443ac83cbcc5448356866acd3d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:38:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:45:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c13086b2cdc797d6ae8ae49964c3990abf6b026e7f643db84a65b7f084366f08`  
		Last Modified: Thu, 16 Mar 2023 03:53:59 GMT  
		Size: 32.0 MB (31970021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb512502a00877ef190b1815b85439c23acfccd37a17990ec798b2bea4e21069`  
		Last Modified: Thu, 16 Mar 2023 03:53:49 GMT  
		Size: 7.6 MB (7632987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c926d392a0489ac95be096f121aa71205ac931a151fc7c4564fc57444078c1fd`  
		Last Modified: Thu, 16 Mar 2023 03:53:48 GMT  
		Size: 4.4 MB (4408510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2857f7a011d6755514a89958db979d33059396ce8ea89c6552489bef9035282b`  
		Last Modified: Thu, 16 Mar 2023 03:54:23 GMT  
		Size: 48.9 MB (48926165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0775c8324947137c1777a6bb6e389e8f1ae322fbca889c73a00a2c57a91e8a1b`  
		Last Modified: Thu, 16 Mar 2023 03:55:20 GMT  
		Size: 197.2 MB (197204751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:45e836f4bee45e343d3d20e203bbab10f5eaad7b0934027e11c1be55ebca27a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.1 MB (237149064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1505c6374943ba67de8bcae872902c1bc61e99bc98f23769939466c5ae877c8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:56:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:58:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:413472b726c3207e3bafacfb65a3db7c0c8692445502e7d2ad70b1585e534841`  
		Last Modified: Thu, 16 Mar 2023 02:04:26 GMT  
		Size: 26.2 MB (26162786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef961f5d29313e42026cc5111865e26af7782293f64f5eca11172750d63f804`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 6.3 MB (6335431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b09797bd3d78e6694a4d023216c32e3665a913d5dcd639c47a00674aa9bd5f`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 3.7 MB (3674242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ac168459f3e70bf00dbc80bd6a3cca0005c0e36d3ecf7fd0ae2395921677c5`  
		Last Modified: Thu, 16 Mar 2023 02:04:40 GMT  
		Size: 44.1 MB (44081685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4a0858837f3c6eeaa709f1bf472664e892f57a6f75cf799ebf86f41ac8b732`  
		Last Modified: Thu, 16 Mar 2023 02:05:08 GMT  
		Size: 156.9 MB (156894920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-curl`

```console
$ docker pull buildpack-deps@sha256:3c92603c3c4cfdf54434d189f6ea4b878e2f864e9756808938df4b7b261813e9
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
$ docker pull buildpack-deps@sha256:88cc8d8450e2140b02c76ab91eb047c03405b2b54809c53dd5850a6b766b84cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37876648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9541ffb4362b8ed33942bce7957eb33fc7b9063e91e93e93d47fecd801deb76d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:37:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dbd9104be902889dc21019a0f5023f798f3d4659871b7eff4e60ea6f1496df08`  
		Last Modified: Thu, 16 Mar 2023 05:45:13 GMT  
		Size: 27.5 MB (27533123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926546ac77ef389dea10f2f48a9435499b9fd85ce007f054787873fba3ba820`  
		Last Modified: Thu, 16 Mar 2023 05:45:10 GMT  
		Size: 6.7 MB (6653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e02fdac0efdc0f5d71c45d6ab71b8cf2421156adfbe3dd6673c198b60f5e696`  
		Last Modified: Thu, 16 Mar 2023 05:45:09 GMT  
		Size: 3.7 MB (3689653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:614fca6a30bbfe066856c014a147fa326ec793122ed0e9624732cb670ce2e85f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35029544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24b29040dc3a4ce8a013430cf3b9e64653cb7a9d0e2b07e0b725dc6c71041281`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:01:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f2e2ff6a76c080ab34fadea2f47efdf4e1606b1482ed2e4597e51810a467b28a`  
		Last Modified: Thu, 16 Mar 2023 04:11:42 GMT  
		Size: 25.4 MB (25359548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003fc5922aae3f4274356fca42181568c983c95440b266598d0a8b3307f981b3`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 5.8 MB (5819049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f573392ff6ba3d538b9dd78eaac78c3a48a8719f2c3a366e5031c24433553af7`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 3.9 MB (3850947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9bfb20d764824394d6318a1e3ea3ca8dc572a7fc5d2174fe2057b50bb244e9e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37078752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629f7f7e4b34d738f867a79f3b2bb90546a32a19fe6bb8ad427d42c1d6153cc7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:17:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5bd94ab779df0c538759342d8eef230b315e98979bcac4604e94fb874397461b`  
		Last Modified: Thu, 16 Mar 2023 04:25:04 GMT  
		Size: 26.9 MB (26945660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df8402fa00c99b6f8233d0c6452e59cfe2742b9b2c9f44a504aaa45a0516cd3`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 6.5 MB (6484575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa45039d5b2736a9624493cbbbf9200c134de7ddb8696ce87c68dad417e12f4`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 3.6 MB (3648517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a5df0b199035bf5963b942dadf1b32fc61120f2d0605e2a9fad2cabc1839a7b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44011518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1611814033075adc80702cce1f81c5df91554f4e75044921f9b25158d1cbe296`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:38:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c13086b2cdc797d6ae8ae49964c3990abf6b026e7f643db84a65b7f084366f08`  
		Last Modified: Thu, 16 Mar 2023 03:53:59 GMT  
		Size: 32.0 MB (31970021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb512502a00877ef190b1815b85439c23acfccd37a17990ec798b2bea4e21069`  
		Last Modified: Thu, 16 Mar 2023 03:53:49 GMT  
		Size: 7.6 MB (7632987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c926d392a0489ac95be096f121aa71205ac931a151fc7c4564fc57444078c1fd`  
		Last Modified: Thu, 16 Mar 2023 03:53:48 GMT  
		Size: 4.4 MB (4408510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7d87ab98ab8a33299dd743e4394ecfd4148bae746acec49a6fffefb7e01b57ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36172459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8450951ba16b57ce51376ee52be443e0ef4c01e6ab2e5b0789a6a004768c0358`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:413472b726c3207e3bafacfb65a3db7c0c8692445502e7d2ad70b1585e534841`  
		Last Modified: Thu, 16 Mar 2023 02:04:26 GMT  
		Size: 26.2 MB (26162786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef961f5d29313e42026cc5111865e26af7782293f64f5eca11172750d63f804`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 6.3 MB (6335431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b09797bd3d78e6694a4d023216c32e3665a913d5dcd639c47a00674aa9bd5f`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 3.7 MB (3674242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:4e0401bf1ba398dfbd820acc7da7a7b48bebe090d46f525f29b42f1e54334bf7
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
$ docker pull buildpack-deps@sha256:8c474a27635a29ce1f6daffda32528a0aa48b6f589ecf88490b158f33a571f15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82127733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46a0d94344b399c5d7604309d08fcd4a61f68a8911fd92690bd5f4a46d9c8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:37:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:37:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbd9104be902889dc21019a0f5023f798f3d4659871b7eff4e60ea6f1496df08`  
		Last Modified: Thu, 16 Mar 2023 05:45:13 GMT  
		Size: 27.5 MB (27533123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926546ac77ef389dea10f2f48a9435499b9fd85ce007f054787873fba3ba820`  
		Last Modified: Thu, 16 Mar 2023 05:45:10 GMT  
		Size: 6.7 MB (6653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e02fdac0efdc0f5d71c45d6ab71b8cf2421156adfbe3dd6673c198b60f5e696`  
		Last Modified: Thu, 16 Mar 2023 05:45:09 GMT  
		Size: 3.7 MB (3689653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57775961ac4b5f4df9ba21c9a454eec60eced52106a9c3c6480abe04fd31e975`  
		Last Modified: Thu, 16 Mar 2023 05:45:29 GMT  
		Size: 44.3 MB (44251085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6b08244e2bc4db9fd4a22095b42d9044de738c27f0c4f78a9fd1303fb5e9459e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83364676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad34d38cd21a977e6a4b1485518ff8873988b314b13cb4796e11b2ed4ec4d693`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:01:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2e2ff6a76c080ab34fadea2f47efdf4e1606b1482ed2e4597e51810a467b28a`  
		Last Modified: Thu, 16 Mar 2023 04:11:42 GMT  
		Size: 25.4 MB (25359548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003fc5922aae3f4274356fca42181568c983c95440b266598d0a8b3307f981b3`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 5.8 MB (5819049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f573392ff6ba3d538b9dd78eaac78c3a48a8719f2c3a366e5031c24433553af7`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 3.9 MB (3850947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e5edf4553807d09a5e079189ad8abe94fa20ac8d3b91a1fdee74ffbbfc465a`  
		Last Modified: Thu, 16 Mar 2023 04:12:00 GMT  
		Size: 48.3 MB (48335132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7718090c669d397351860cb0345fd87226c3f44bfc63156d13b88ee8b6bb13c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81133371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:794f72335c8bb0cbfaa191b6c8873dca8c9aeca030e74c1f1e6e88e9df6cfe91`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:17:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bd94ab779df0c538759342d8eef230b315e98979bcac4604e94fb874397461b`  
		Last Modified: Thu, 16 Mar 2023 04:25:04 GMT  
		Size: 26.9 MB (26945660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df8402fa00c99b6f8233d0c6452e59cfe2742b9b2c9f44a504aaa45a0516cd3`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 6.5 MB (6484575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa45039d5b2736a9624493cbbbf9200c134de7ddb8696ce87c68dad417e12f4`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 3.6 MB (3648517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5195e2054b68f924f77b2db71706b518fdc87c9c6f3d900adad8e6eec601fb`  
		Last Modified: Thu, 16 Mar 2023 04:25:18 GMT  
		Size: 44.1 MB (44054619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:80776e57275eac4ab14959cc2eb0aa5c39dfbc1eac936218d2bd4714c32b6d34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92937683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86884dca514275133e923ec8f78e2785269d5ed21433f44077b1e44c33e5751b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:38:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c13086b2cdc797d6ae8ae49964c3990abf6b026e7f643db84a65b7f084366f08`  
		Last Modified: Thu, 16 Mar 2023 03:53:59 GMT  
		Size: 32.0 MB (31970021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb512502a00877ef190b1815b85439c23acfccd37a17990ec798b2bea4e21069`  
		Last Modified: Thu, 16 Mar 2023 03:53:49 GMT  
		Size: 7.6 MB (7632987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c926d392a0489ac95be096f121aa71205ac931a151fc7c4564fc57444078c1fd`  
		Last Modified: Thu, 16 Mar 2023 03:53:48 GMT  
		Size: 4.4 MB (4408510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2857f7a011d6755514a89958db979d33059396ce8ea89c6552489bef9035282b`  
		Last Modified: Thu, 16 Mar 2023 03:54:23 GMT  
		Size: 48.9 MB (48926165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:be8e1571ea2945b768f155c85a9fc4d617a62103e27b12291a1b9e88c5ae2f53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80254144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad371214c349f4a458439e817f999971228fed0bcf6aceaccbb08508cf9c8a0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:56:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:413472b726c3207e3bafacfb65a3db7c0c8692445502e7d2ad70b1585e534841`  
		Last Modified: Thu, 16 Mar 2023 02:04:26 GMT  
		Size: 26.2 MB (26162786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef961f5d29313e42026cc5111865e26af7782293f64f5eca11172750d63f804`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 6.3 MB (6335431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b09797bd3d78e6694a4d023216c32e3665a913d5dcd639c47a00674aa9bd5f`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 3.7 MB (3674242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ac168459f3e70bf00dbc80bd6a3cca0005c0e36d3ecf7fd0ae2395921677c5`  
		Last Modified: Thu, 16 Mar 2023 02:04:40 GMT  
		Size: 44.1 MB (44081685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:9220571f3d9e6eefa8a367d60fefcd69c92c5bd591364a08f9c0f8f6adc96607
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2ea103832a6fac73696522edc50dc0aa8c41a2073edb2d29685224196ed046e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.0 MB (312037541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055f98e5c72e14d3f944a8a2f131602966cfd07c563d5884eddb16a00be4c875`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:54:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b253aeafeaa7e0671bb60008df01de101a38a045ff7bc656e3b0fbfc7c05cca5`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 7.9 MB (7863355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2201bd995cccf12851a50820de03d34a17011dcbb9ac9fdf3a50c952cbb131`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 10.0 MB (10001452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de76e268b103d05fa8960e0f77951ff54b912b63429c34f5d6adfd09f5f9ee2`  
		Last Modified: Wed, 12 Apr 2023 07:58:44 GMT  
		Size: 51.9 MB (51876420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a8df5894511ce28a05e2925a75e8a4acbd0634c39ad734fdfba8e23d1b1569`  
		Last Modified: Wed, 12 Apr 2023 07:59:14 GMT  
		Size: 191.8 MB (191847588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:02fd9794c7da040f3ef1d7dd0c0712ab7683702b42b2a51e61ab533b528b764d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.9 MB (277871011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15256ef87a3aabbd62493903b36c4f9b28de5b55c797bcfc8455138b602cf77c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Mar 2023 23:23:23 GMT
ADD file:dabb9dad1d8086faa890c6425e759e27f1052d9677aa640dd310def49d8a5bc5 in / 
# Fri, 24 Mar 2023 23:23:24 GMT
CMD ["bash"]
# Sat, 25 Mar 2023 01:03:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Mar 2023 01:03:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Apr 2023 23:15:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 07 Apr 2023 23:17:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09b82635e0c9396d28359dea2597b070f13d2e7fbdd1b9cb395b7f7a1cd09d59`  
		Last Modified: Fri, 24 Mar 2023 23:28:44 GMT  
		Size: 45.9 MB (45915861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be96c3cc707a08b828f7785eb0ec3a8a556466f537aa6de458e43a19667d155`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 7.2 MB (7153944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65e90f973c6f54fcc28489eb109e74c36765dd1293a930f62889f9f1ac1f75`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 9.3 MB (9348989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c951b868b2dee5c41bb5bc49ed01649d3b23457f73f686de3257e3922c4237`  
		Last Modified: Fri, 07 Apr 2023 23:18:43 GMT  
		Size: 47.4 MB (47395369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22d1abb7637dd224bb51a637438918a121d198e654c56e2207e8bca99b6ba2d`  
		Last Modified: Fri, 07 Apr 2023 23:19:12 GMT  
		Size: 168.1 MB (168056848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5e8e3f3212dcc5c0e3442e591cffe69a01891021308eca92c8b3bc2803c31459
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.6 MB (302601726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0303fb5950d191d02ab39565ca367ca55dc2b108c9b7ba4d645ed85d1a074d1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:10:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208fd617b499747daceba851b67da426c285d1e306b316a193f06968123f49da`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 7.7 MB (7732136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efadebfda1423d1b70a0e991e9ff8bb2e3fe0b08d55562359a004c265fc7c86`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe7e7c438113f5e58417f97e7eb0a755b17ee63eebd85a7c3b86a2aad4c993e`  
		Last Modified: Wed, 12 Apr 2023 01:14:27 GMT  
		Size: 52.2 MB (52191713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33997ebd7335eb6f55d98725b5fb8e4899166098d6db119cd6f6bc7055ffa858`  
		Last Modified: Wed, 12 Apr 2023 01:14:51 GMT  
		Size: 183.4 MB (183435664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:76a9d8ac8ca52b47077a29022657b9bdc9facd485bf6f6bc8c7115ed9915e020
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.5 MB (321464682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb3655fb3b861afdfc5e7da86468a57acd97ab2b796815bf255141ce4e9ec42c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:11 GMT
ADD file:8299e58c7e43af1f3b9fdb9bd37e3f37cf619a97ef1b87d60ca66860d646d526 in / 
# Wed, 12 Apr 2023 00:39:11 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:08:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d15e1c2a3da7d675c2513d7ceab1d0f33ced9a82bed63d9a11ce71f1218d232`  
		Last Modified: Wed, 12 Apr 2023 00:43:07 GMT  
		Size: 51.2 MB (51206167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af123d7f5c8b1197b6040820195efacf1a57299baf71416c7a63281566cdc199`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 8.0 MB (8034011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3af175eda8706326ac898703f9aafb47e7e08ec08318794c6838efa8f3d3bc`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 10.3 MB (10345678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cbd6d7217bf920da02e590f88fbfb42fb3162969840a3b17eb25c762247c04`  
		Last Modified: Wed, 12 Apr 2023 01:16:35 GMT  
		Size: 53.5 MB (53471080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d0a6f1efbd6131f1ae888ea393318f9d32a3e8ad8b8c97207c3a5b7a3ed9bc`  
		Last Modified: Wed, 12 Apr 2023 01:17:17 GMT  
		Size: 198.4 MB (198407746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:640a378736a09f13765f1e7113e5082c0e5afbad023a3bc5fd16061f36d68106
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7f26d8de0d9b1472f4b76a591461f81e28dd4469eed96b3bb172a93adde9779f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68313533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:212d47455d74a1b460742fc95270dd155e5dccb7f8cf98d1b0166a911a42e56f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b253aeafeaa7e0671bb60008df01de101a38a045ff7bc656e3b0fbfc7c05cca5`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 7.9 MB (7863355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2201bd995cccf12851a50820de03d34a17011dcbb9ac9fdf3a50c952cbb131`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 10.0 MB (10001452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8c8d5fcfcee6383cfd57156be5815dd7406a36072a56878ea28be0754c13d629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62418794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27f682abc8f89b3916f2a6eeef8f25431524f50af3bac2d7eccbba6aea38a8b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Mar 2023 23:23:23 GMT
ADD file:dabb9dad1d8086faa890c6425e759e27f1052d9677aa640dd310def49d8a5bc5 in / 
# Fri, 24 Mar 2023 23:23:24 GMT
CMD ["bash"]
# Sat, 25 Mar 2023 01:03:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Mar 2023 01:03:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:09b82635e0c9396d28359dea2597b070f13d2e7fbdd1b9cb395b7f7a1cd09d59`  
		Last Modified: Fri, 24 Mar 2023 23:28:44 GMT  
		Size: 45.9 MB (45915861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be96c3cc707a08b828f7785eb0ec3a8a556466f537aa6de458e43a19667d155`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 7.2 MB (7153944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65e90f973c6f54fcc28489eb109e74c36765dd1293a930f62889f9f1ac1f75`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 9.3 MB (9348989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f4f9c875a9f7cdaa332594325c8c868d26a05ef018355a11554c8b1b5657b625
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66974349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25cefdb01c939d204ba6d7c49b6053a29c8ad035592de81e899acd889fd70fc2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208fd617b499747daceba851b67da426c285d1e306b316a193f06968123f49da`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 7.7 MB (7732136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efadebfda1423d1b70a0e991e9ff8bb2e3fe0b08d55562359a004c265fc7c86`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:da84dcb1542b8a34ef0e6ebd7f50eeb5da1bf9f8c87c221b3d3a2bd81c81de56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69585856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:256da6b06a3adecebaf9bba1b763d651016b84bfec4ad7bc9dbe24e15f37894a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:11 GMT
ADD file:8299e58c7e43af1f3b9fdb9bd37e3f37cf619a97ef1b87d60ca66860d646d526 in / 
# Wed, 12 Apr 2023 00:39:11 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2d15e1c2a3da7d675c2513d7ceab1d0f33ced9a82bed63d9a11ce71f1218d232`  
		Last Modified: Wed, 12 Apr 2023 00:43:07 GMT  
		Size: 51.2 MB (51206167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af123d7f5c8b1197b6040820195efacf1a57299baf71416c7a63281566cdc199`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 8.0 MB (8034011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3af175eda8706326ac898703f9aafb47e7e08ec08318794c6838efa8f3d3bc`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 10.3 MB (10345678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:2d4209bed38ccbaafe80aa66292d82ca537b2ef985ab3f0ac7743ce258f39660
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0559dadbf61570961c0fad2acef618449ab55dc06360900e44639acdfc52d29b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120189953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ba89d7351401c33e1d4f3e124b255947cc4bf33b68236db9d8985829c0c1420`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b253aeafeaa7e0671bb60008df01de101a38a045ff7bc656e3b0fbfc7c05cca5`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 7.9 MB (7863355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2201bd995cccf12851a50820de03d34a17011dcbb9ac9fdf3a50c952cbb131`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 10.0 MB (10001452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de76e268b103d05fa8960e0f77951ff54b912b63429c34f5d6adfd09f5f9ee2`  
		Last Modified: Wed, 12 Apr 2023 07:58:44 GMT  
		Size: 51.9 MB (51876420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:73ce5e0aec65d7a74a776adbc4a7f73e23a098cc443305405cf91545d7428a1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109814163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93145c7f3983a14d63ebc6172d40d92d34548b31354e82b5de20eeb2dc2db6b6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Mar 2023 23:23:23 GMT
ADD file:dabb9dad1d8086faa890c6425e759e27f1052d9677aa640dd310def49d8a5bc5 in / 
# Fri, 24 Mar 2023 23:23:24 GMT
CMD ["bash"]
# Sat, 25 Mar 2023 01:03:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Mar 2023 01:03:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Apr 2023 23:15:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09b82635e0c9396d28359dea2597b070f13d2e7fbdd1b9cb395b7f7a1cd09d59`  
		Last Modified: Fri, 24 Mar 2023 23:28:44 GMT  
		Size: 45.9 MB (45915861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be96c3cc707a08b828f7785eb0ec3a8a556466f537aa6de458e43a19667d155`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 7.2 MB (7153944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65e90f973c6f54fcc28489eb109e74c36765dd1293a930f62889f9f1ac1f75`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 9.3 MB (9348989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c951b868b2dee5c41bb5bc49ed01649d3b23457f73f686de3257e3922c4237`  
		Last Modified: Fri, 07 Apr 2023 23:18:43 GMT  
		Size: 47.4 MB (47395369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:96e03d67380daeace99ddc589fb25df608d86e8a2d78ef9d4635323c7774934b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119166062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2ed8743d8648e388b28b2c5274b320ccc3352bca03a56d3d0b65c133c5acf9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208fd617b499747daceba851b67da426c285d1e306b316a193f06968123f49da`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 7.7 MB (7732136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efadebfda1423d1b70a0e991e9ff8bb2e3fe0b08d55562359a004c265fc7c86`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe7e7c438113f5e58417f97e7eb0a755b17ee63eebd85a7c3b86a2aad4c993e`  
		Last Modified: Wed, 12 Apr 2023 01:14:27 GMT  
		Size: 52.2 MB (52191713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0e2e0b3634ba26d3880a8dad7170dc329234f18b5b9b38e0bd3c4637cbe27ace
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123056936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67dfa6883f98d7b82d1d95b560a9f118e646738acef237ff47081baf6ed84941`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:11 GMT
ADD file:8299e58c7e43af1f3b9fdb9bd37e3f37cf619a97ef1b87d60ca66860d646d526 in / 
# Wed, 12 Apr 2023 00:39:11 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:08:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d15e1c2a3da7d675c2513d7ceab1d0f33ced9a82bed63d9a11ce71f1218d232`  
		Last Modified: Wed, 12 Apr 2023 00:43:07 GMT  
		Size: 51.2 MB (51206167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af123d7f5c8b1197b6040820195efacf1a57299baf71416c7a63281566cdc199`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 8.0 MB (8034011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3af175eda8706326ac898703f9aafb47e7e08ec08318794c6838efa8f3d3bc`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 10.3 MB (10345678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cbd6d7217bf920da02e590f88fbfb42fb3162969840a3b17eb25c762247c04`  
		Last Modified: Wed, 12 Apr 2023 01:16:35 GMT  
		Size: 53.5 MB (53471080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:4fba0beac07f82d041571a394110dca419cbb71285de82105ae04e9c7401fd9c
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
$ docker pull buildpack-deps@sha256:22e8a94a63b1cf94bc6e69418b975d41cb9ca48640b8b3a48002eb9c65039abb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8cd24e709af1ad98665077ad3ae2b89451839cb3a36350db232d6ce523d0d60`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b89f3c7f7da8adf032a33a75d1b659cee33179ecb88ea0ba75e4fc58ebe63a6`  
		Last Modified: Wed, 12 Apr 2023 07:57:46 GMT  
		Size: 54.6 MB (54584801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ea05ef84678632f8c536876f2c7f5fc619fc524fc4b7dea24106ccb4b55809a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120542472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640f06156014acf4823a54fa99d9d265ad6efe6eda17f48174918044c3a2ea19`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:15:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:16:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49db155cdf8645f599affcbbbc75eb928b0a9d010c4ac54afcfa9d7e4fa85e0`  
		Last Modified: Wed, 12 Apr 2023 01:21:15 GMT  
		Size: 5.1 MB (5072827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936087cbd048148575fda58348506149db80a2699e99ae2042086628c0e5a38`  
		Last Modified: Wed, 12 Apr 2023 01:21:16 GMT  
		Size: 10.6 MB (10573853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0bf11569c39ee4f3d8515112046a55f14f39e54c6f0ea26271033c090f77d2`  
		Last Modified: Wed, 12 Apr 2023 01:21:35 GMT  
		Size: 52.3 MB (52340617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4e954e4c9de72e8e1118eb94583ab2f5f6dde3064d1c9ac34b712cd3ba6a1f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115719518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c576aa271c58013d567de0474bf19f0a9b589c98e78c3e2609b5f4dccb1bfc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca667140ff247fc759283fc9ff4cafbe304d1777ffc70e1bd593b63151c31a`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 4.9 MB (4934357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879c254431e9965afb23e55a148faffd29450a9218269f769be95d6e9673a93`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 10.2 MB (10217859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64c4a1b9916f6da6f286835522f27f11a812694e5f878e87468d4c6b90b343e`  
		Last Modified: Thu, 23 Mar 2023 12:45:20 GMT  
		Size: 50.4 MB (50355514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8932a28128c9d2abaed3ae68d2641c6738ab07bf083ca8886920e13ce37bbce3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124407974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d7143247bb9728129c637c315a5d5529383d57dfbf55c6999d1479a6f6dee2b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:07:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f993d5b17f32f4b8a535c25e182e5d8412625beee450e513ca57036e8fdd6dc`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 54.7 MB (54676038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2af50719cfc3c1165d1e75a99045d98388d375c4dcf2cafd5526a78d50080eab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128499065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863e942eeec226faacc53f695802b0b24e7dd766b5e4a9498a0d7c62e92c702`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:06:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ccf9a5e34ba2345ce265a9a11c93ee254e1f3616dfd1c1deda6e2f7d614c8`  
		Last Modified: Wed, 12 Apr 2023 01:14:53 GMT  
		Size: 5.3 MB (5293626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4988d5e4328f031f6884a7351766aa8a2806c9cdca38d354477fc537eaa4911f`  
		Last Modified: Wed, 12 Apr 2023 01:14:54 GMT  
		Size: 11.2 MB (11249875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660a2befd486d43a308dd1561f57efeafe1f13defd6439d34aeb5efec783ee3d`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 55.9 MB (55922746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a9ec515744077c37744762c48a381049165872c3140692bfa932f9cec2efd549
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122155673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6653fbf81293b8dbce803c3de0330f89c7b15f3d502575b1d0c255336c26a706`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:15:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f79f6951926609a68e21aee7e612375637f7c12703c62b028fd60a22e2d9bfd`  
		Last Modified: Thu, 23 Mar 2023 07:34:02 GMT  
		Size: 4.9 MB (4922133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b6297024241cbdae60b7afa1bce7cc669d998e17b209e8b133df9e13da064`  
		Last Modified: Thu, 23 Mar 2023 07:34:04 GMT  
		Size: 10.7 MB (10662010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9437ab03a3b730ed3d31f18a79500c8ce379f2a971ed27695d60f38e887121b2`  
		Last Modified: Thu, 23 Mar 2023 07:34:50 GMT  
		Size: 53.3 MB (53306810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:308a8f8623e3d18d4ca7d0dcbd1fc6759e17b9a128dde3c2f263439cba80795c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134830410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5026643d3fb952f674886305718eb0a8a22bc3e0a6ba7cf3c44b76b61ce8d04`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:15:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:16:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805b891b319592a15b7da9a474b2f36e32ed9b8a720d14bbbe4d08422343b19`  
		Last Modified: Thu, 23 Mar 2023 13:24:55 GMT  
		Size: 5.4 MB (5415174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdb7e2b62c4c7c555894be507d7ccaf7aeca0f8c9088a9082ad4cd37dc97f28`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 11.6 MB (11629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac3f4f172050b21a6f17c30c60794779e7d5c150f1111240477b89240ad7f6`  
		Last Modified: Thu, 23 Mar 2023 13:25:22 GMT  
		Size: 58.9 MB (58864543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dfe7b376859cc874a19230408e2042b1d984722eca290ce8cced0e27c6bdc7bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123263942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0184582450f7852885e4f2a6aaf51c5ec9ce0ff2ce9cd9b877a945b87bfd33c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:27:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2973b8c98f9da7833ab9cd69185dd958a8939a30136cdcfedb66ce775db358ee`  
		Last Modified: Wed, 12 Apr 2023 00:32:48 GMT  
		Size: 5.1 MB (5149313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f740d13ac612bf8b6489559a7945ec1439fee2d5eba455ab0db047cd3f30a9a`  
		Last Modified: Wed, 12 Apr 2023 00:32:49 GMT  
		Size: 10.8 MB (10766104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c0067783f401b099adca196dce9e464e66236e49faba106e2f04ac73a90df7`  
		Last Modified: Wed, 12 Apr 2023 00:33:02 GMT  
		Size: 54.1 MB (54061843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:6fa31d2839b2176bb4d92e7cb1bf4f0acdac4ca440650d2d937bfd713779f3a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1cb95d972e0a2c28195432ae6f0b584389e01e1938354a98b61c2d0e4c79f44f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.0 MB (350981822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9133db89f5b5ae7caee0f8cca02226caaa3b22832a67d2a4bfc68f2ca38dfccf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:55 GMT
ADD file:0936f6fccda991ba27a7f73ca61c23a436b7ca417e504b66d5a68f2283e1e81d in / 
# Wed, 12 Apr 2023 00:20:55 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:54:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:54:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:55:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:003dca91ec623536e08abc4e1bb2849836a84c44f82e24b97fd5423162a4d46e`  
		Last Modified: Wed, 12 Apr 2023 00:25:13 GMT  
		Size: 49.3 MB (49287652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486f0b6179599c75a087e6850c42ef248d973e29a6898ed99c9bccdae08d2cd2`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 9.1 MB (9082764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f184ca8dda7ed83dd9d21d6c880d4e15976f35814156a0a67df81423067f4b8`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 11.4 MB (11422423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76159e5040abc54c8e269f5e87ba68551c98fa9a6a06c9d7af5eae5f9f3ee57b`  
		Last Modified: Wed, 12 Apr 2023 07:59:41 GMT  
		Size: 64.3 MB (64257071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108d0b8f8755100dc81501ff3e762f953171a4a1230223973781ad90f85c1a53`  
		Last Modified: Wed, 12 Apr 2023 08:00:14 GMT  
		Size: 216.9 MB (216931912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7c5689a7aafd87d157899f6caf4601d66e8e391aef6483970f37553b5a868314
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.5 MB (318503660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:321ba3c06205c499df306cc1b5cfded148321e0a03dea6b3028714995c1f7d03`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:48 GMT
ADD file:b02c911309a1b69d235b76dab369d523653c62374b0173ee9f1b65017607f9d6 in / 
# Wed, 12 Apr 2023 00:48:48 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:18:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:18:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:19:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8699c4859220eb7e4f2a5ae13e4dd5f9143cb7144e2a02a3eb381a79416524bf`  
		Last Modified: Wed, 12 Apr 2023 00:51:27 GMT  
		Size: 48.1 MB (48109671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b565bf44c40ab65f5193c4fbfd752809f50e95e2c4b2397728f42419979d7c`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 8.5 MB (8522810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8db076a21199a98e758a14876a91c9a890bb606e6d9d483862bcb73bc5cfbb`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 11.1 MB (11065853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466720607b58ed4036916fa9d7cb2e82a3ca95f0e5ec8e2ef908744cd3e409ec`  
		Last Modified: Wed, 12 Apr 2023 01:22:44 GMT  
		Size: 61.7 MB (61667229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df42d9b3dd685881fab45c09a19f6d1505f1612856e8b0acca62c90e5aa6457`  
		Last Modified: Wed, 12 Apr 2023 01:23:20 GMT  
		Size: 189.1 MB (189138097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:13bc1f7227e4eb190e2425e9ae9baaa9afa595247f7c48578dae477f5206c282
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.1 MB (299089852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82add4ff4f01d1f31c7d61d6b83e243c99fc38f0cb8fbe94fc118eaf5a75103`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:28:43 GMT
ADD file:628ac1300ca273dba23c7d617164bc6e664cdebb4106910020d7b3dcb39429c8 in / 
# Thu, 23 Mar 2023 01:28:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:42:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:42:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:42:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:43:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53d7f1f008e91cd29c47c933b404c16fc1d4cf64b8699ad1269e882f53ca6e2d`  
		Last Modified: Thu, 23 Mar 2023 01:34:10 GMT  
		Size: 45.9 MB (45911196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61016f9e9c2f44cda61da9f54267fbafe7fef3695caec3c87c6d5ae9eb452ae4`  
		Last Modified: Thu, 23 Mar 2023 12:46:05 GMT  
		Size: 8.2 MB (8168245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4226b16c6b7093dc765001b6e5615e8150c8d19be6c96ea1171e1ad13654f5`  
		Last Modified: Thu, 23 Mar 2023 12:46:04 GMT  
		Size: 10.7 MB (10704470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889e5e2259a7026a6a42309e4673ccd18c4288dce5b85e2039cb7238e36ce3fe`  
		Last Modified: Thu, 23 Mar 2023 12:46:22 GMT  
		Size: 59.4 MB (59373909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd2df18bf0523ee48067a579083ad967febe18f6eda98aa82f65c4fbb8ff974`  
		Last Modified: Thu, 23 Mar 2023 12:46:53 GMT  
		Size: 174.9 MB (174932032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ddc7753bdf44aa12263963bdb9942af3b69f4ed4dad7430d1a9eecabd6381d97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.1 MB (342096356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e722281a223374a931912368ece55c74201c7f46e39795b84006341333ddb0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:21 GMT
ADD file:2784bc6dba1e1dbea293e074ebf51fa7d89cb5545ea63ba2ed75b74d067387d4 in / 
# Wed, 12 Apr 2023 00:40:22 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:10:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:10:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:10:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43d214f7ab3ca35a0c9ed4d8cdf62b36248aba2fa1bbac4ecd64e82ba2520b70`  
		Last Modified: Wed, 12 Apr 2023 00:43:58 GMT  
		Size: 49.3 MB (49327656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d9e5d2b2df062d16ffea4a022a4c09ce904fb96ec3fa4712a1d936593ae2a`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 8.9 MB (8915031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd2b1a4cab3b4ac2bb4a7e9aaaa60ce806e3c49a8726f7baf5a10ba5e0e89fb`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 11.4 MB (11389544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff14914c0381e1889d1db49b1b39da80ae3a347cf1af048e2ae0eb42aec87a12`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 64.2 MB (64154048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f54a27824f720f86861a2776e1cc4e2f54563a9d0f0b56d1a6ec034866e3f8`  
		Last Modified: Wed, 12 Apr 2023 01:15:45 GMT  
		Size: 208.3 MB (208310077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:413efb8fbcbb35e21e9437afbee83ae1bdcf365d62cc1261952b77c46884fede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (352984444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09e361eb5030e9416d576bb6456af5b6f82090e0ffcde0ac62558e2c5fa198c1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:51 GMT
ADD file:31710a830769b5e1f2612e1cd05380f677714bf52f61a54adbc7424087fd1378 in / 
# Wed, 12 Apr 2023 00:39:52 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:11:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:13:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35e4af56b8bda58bf958814bc36c8e3a9a1d719c8582c0f33d7d69cc5b416211`  
		Last Modified: Wed, 12 Apr 2023 00:44:24 GMT  
		Size: 50.3 MB (50310899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145bb18c860aae65312434f79bce9d784a4824ef455202efca0f687a388037fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 9.3 MB (9263774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2063c41d1dff24f54b6a7d8edde21610fe37e02b35ed369be0ccf9f64cdc43fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 11.8 MB (11827096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3196dd70f259df7354dba37d732f79f68e602883ec8838b2cfcd0515de5c5c`  
		Last Modified: Wed, 12 Apr 2023 01:17:49 GMT  
		Size: 66.1 MB (66127351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc32f4359c6fe3187a1f8bab45e405139e65a8f45a4858a27e1059dd58842672`  
		Last Modified: Wed, 12 Apr 2023 01:18:36 GMT  
		Size: 215.5 MB (215455324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3862aaeea79e1c28e659f99f4d362b54d636ab87938c521b7e6c32cd660f4359
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.5 MB (321528438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d166a77be6f0012f9af9d61d3c7ad01ee0b80e1584627a75c08c07fee6b7e9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:18:32 GMT
ADD file:2d913f7b6c2e804834958b3d144bd7b5150a438e2aaa73cdf2f1be1c64d10100 in / 
# Thu, 23 Mar 2023 05:18:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:24:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:30:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c1a140184ad386a37a5446dba474a2a8498dff7ae8d2ccd2957aaf8dc1682e`  
		Last Modified: Thu, 23 Mar 2023 05:26:35 GMT  
		Size: 49.3 MB (49291603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaeb19ea7953e3c0a2cce0d76910d46a1fc5e289c90379ecb81b3e5ba2a0c16`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 8.4 MB (8439874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecc4eca24f781c1e786d1fc88cb24202f1248f85adc06cf1b375f5607ec2d93`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 11.2 MB (11170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3768b306fba92d6a836552b3ee3a1bb755cd0f7d6618ca028d0643fde06553`  
		Last Modified: Thu, 23 Mar 2023 07:37:53 GMT  
		Size: 63.1 MB (63099163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cde7245b1c56e104d5370eab7caa185d690ab7a9d05dd04502c112995eedf9c`  
		Last Modified: Thu, 23 Mar 2023 07:39:55 GMT  
		Size: 189.5 MB (189526884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1cd92695e70eee806ffc668ffc3613c1ae37e09e9905ff84a9ad42e7353a4a07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.8 MB (358843576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff6cf39c1a7a6027c3f5251567633ab1cfbf3af110fb104f2f31ece459b538e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:20:05 GMT
ADD file:3534cf3f10dae5b70c64865fd70cf5b9aa6ace6be9caa2d69518d6d59c4943fa in / 
# Thu, 23 Mar 2023 01:20:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:18:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:19:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8de2c12bac6cdfac096a845424e637222b157d221d8080dfc0e3cd14581716d5`  
		Last Modified: Thu, 23 Mar 2023 01:24:47 GMT  
		Size: 53.3 MB (53290173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ffcd14b130bc950e2e794bcf2e09ddffa8e18668803aa384fc8de743e9d8d2`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 9.7 MB (9661589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecca2a654e1b66be833e49110ac475ae4995f36d83ba12ad0396e8f4cf953872`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 12.2 MB (12185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5053cb00528479013fa5db3eb35bb36ff11628a7f8c9c6ae0310021f09a7005`  
		Last Modified: Thu, 23 Mar 2023 13:26:59 GMT  
		Size: 69.7 MB (69740333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb6e33785c280f1561e4dcdae27bfcb7e802b5b52d2ebf732730e9c11c4c717`  
		Last Modified: Thu, 23 Mar 2023 13:27:58 GMT  
		Size: 214.0 MB (213966262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:b9c02baf674d938d6af39d2f681786407b07e39dcc6c0ef663bbfa3027bb41f6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.0 MB (361040206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcff52053934b6b9001b1f614aafda9141bd8e31a4b2680e51f8d44353d4a4ed`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:05 GMT
ADD file:b8c0cf42f791d92283c2c47cf2ed446fb98a7cde685c9b923c89cadb86ddad31 in / 
# Wed, 12 Apr 2023 00:09:07 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:32:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:35:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:43:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6178d7c3b8603b1579d72ad9f5bda8fd22627feccccd498dad946eddfe96d27a`  
		Last Modified: Wed, 12 Apr 2023 00:12:25 GMT  
		Size: 45.5 MB (45494949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd056fe810f7c94134b5c26af6939949c18bfa4868dbc9f81ea8d7a25a0daf4c`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 8.1 MB (8117374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f8d5394c046224d62d5170fd151d4339e0f5131b1503bf3eafecefe1ec7a10`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 10.8 MB (10794055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0c6cc5fb9f28304c05335b3e21ed5e3cce359b94731f04cc903938689ebc19`  
		Last Modified: Wed, 12 Apr 2023 00:45:23 GMT  
		Size: 59.7 MB (59741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16f9d49dc3af209b4bcf7ce13172c2a5a76516c0d39580db79da7b27eaf387f`  
		Last Modified: Wed, 12 Apr 2023 00:50:51 GMT  
		Size: 236.9 MB (236892651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9287c8095d9220df2f988981ac641e97e22f861d9bd87aa2a19a9e6cf396a687
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.0 MB (319011191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:914264ef0379c6c6c2f67b9eb3fd0e99ffc0016a3f81cb006225180ad93d3a77`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:19 GMT
ADD file:0593fbca11f3d4a9b2b916ee99bb70651af04ea1275262f12e9b0e5c07e81f0e in / 
# Wed, 12 Apr 2023 00:01:29 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:28:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:28:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:29:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1844a6b5cc32e25703d3a6ac2115866157b1f856d7463d0dca8443fea51061f1`  
		Last Modified: Wed, 12 Apr 2023 00:05:31 GMT  
		Size: 47.7 MB (47665068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f306dc6c45f3e2637390b46a2dce7fb061bb8be6ae7c72c47bba97d84b99d256`  
		Last Modified: Wed, 12 Apr 2023 00:33:37 GMT  
		Size: 8.7 MB (8713548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676682574fe22f1cac8016a4f36ad54898c4313e0609a7e88e75e035e32444b`  
		Last Modified: Wed, 12 Apr 2023 00:33:36 GMT  
		Size: 11.3 MB (11288124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f9748f029581dd4821ad6e7d4da7ab4a31600128a2411dda2639c9b92fe58`  
		Last Modified: Wed, 12 Apr 2023 00:33:51 GMT  
		Size: 63.3 MB (63260422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81adcc7796eb9dd6b2ccee5b41b08f31d903a15caab787b2edc99367e1c15497`  
		Last Modified: Wed, 12 Apr 2023 00:34:19 GMT  
		Size: 188.1 MB (188084029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:f113f3ff3a042b006496b153fb9364e5d5aaab208637bec3fd6bf0ba65e447a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:162b0f4bf898e2f30f86c124dae307c51fcefaf8e30eba8f3d0538d5b88b1533
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69792839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895c4767319db895fdd9034df03472e20114f0f8c5ae8c9ce85f116db05635b8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:55 GMT
ADD file:0936f6fccda991ba27a7f73ca61c23a436b7ca417e504b66d5a68f2283e1e81d in / 
# Wed, 12 Apr 2023 00:20:55 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:54:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:54:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:003dca91ec623536e08abc4e1bb2849836a84c44f82e24b97fd5423162a4d46e`  
		Last Modified: Wed, 12 Apr 2023 00:25:13 GMT  
		Size: 49.3 MB (49287652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486f0b6179599c75a087e6850c42ef248d973e29a6898ed99c9bccdae08d2cd2`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 9.1 MB (9082764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f184ca8dda7ed83dd9d21d6c880d4e15976f35814156a0a67df81423067f4b8`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 11.4 MB (11422423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8b516bb4199218b93e0828691cca7924741a8012ef412cd89ec797180b9ad014
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67698334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9438faefdd9540401ef284f3ce81a1c9c2829d48e27358bfaecfb65aedfa6e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:48 GMT
ADD file:b02c911309a1b69d235b76dab369d523653c62374b0173ee9f1b65017607f9d6 in / 
# Wed, 12 Apr 2023 00:48:48 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:18:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8699c4859220eb7e4f2a5ae13e4dd5f9143cb7144e2a02a3eb381a79416524bf`  
		Last Modified: Wed, 12 Apr 2023 00:51:27 GMT  
		Size: 48.1 MB (48109671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b565bf44c40ab65f5193c4fbfd752809f50e95e2c4b2397728f42419979d7c`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 8.5 MB (8522810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8db076a21199a98e758a14876a91c9a890bb606e6d9d483862bcb73bc5cfbb`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 11.1 MB (11065853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f45638145f3049bdd8569f5e3e37f9012b169c009beecbf423abcfede1b90b6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64783911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfccb40ab0d880192527f3c9058b284e721f369d3a6a86d097ac545f40dc846c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:28:43 GMT
ADD file:628ac1300ca273dba23c7d617164bc6e664cdebb4106910020d7b3dcb39429c8 in / 
# Thu, 23 Mar 2023 01:28:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:42:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:42:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:53d7f1f008e91cd29c47c933b404c16fc1d4cf64b8699ad1269e882f53ca6e2d`  
		Last Modified: Thu, 23 Mar 2023 01:34:10 GMT  
		Size: 45.9 MB (45911196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61016f9e9c2f44cda61da9f54267fbafe7fef3695caec3c87c6d5ae9eb452ae4`  
		Last Modified: Thu, 23 Mar 2023 12:46:05 GMT  
		Size: 8.2 MB (8168245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4226b16c6b7093dc765001b6e5615e8150c8d19be6c96ea1171e1ad13654f5`  
		Last Modified: Thu, 23 Mar 2023 12:46:04 GMT  
		Size: 10.7 MB (10704470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c3e4535c3a32e860c9cdcb87e33d91d91a05de0caebac0e396b682b23449f890
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69632231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f59a19733f90d03e40a3a26aa25904ff3dd15a57aa3bc07c4723ab3a166147dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:21 GMT
ADD file:2784bc6dba1e1dbea293e074ebf51fa7d89cb5545ea63ba2ed75b74d067387d4 in / 
# Wed, 12 Apr 2023 00:40:22 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:10:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:10:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:43d214f7ab3ca35a0c9ed4d8cdf62b36248aba2fa1bbac4ecd64e82ba2520b70`  
		Last Modified: Wed, 12 Apr 2023 00:43:58 GMT  
		Size: 49.3 MB (49327656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d9e5d2b2df062d16ffea4a022a4c09ce904fb96ec3fa4712a1d936593ae2a`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 8.9 MB (8915031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd2b1a4cab3b4ac2bb4a7e9aaaa60ce806e3c49a8726f7baf5a10ba5e0e89fb`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 11.4 MB (11389544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7fd624c3066dfa1ca3da4f7665c730788104cdc2cb90f94fe839582a1a20bff9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71401769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10d2d9289ea8eef61411b36e3c5358bc3e57f93d19422a12cdce3b5d7d7e922d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:51 GMT
ADD file:31710a830769b5e1f2612e1cd05380f677714bf52f61a54adbc7424087fd1378 in / 
# Wed, 12 Apr 2023 00:39:52 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:35e4af56b8bda58bf958814bc36c8e3a9a1d719c8582c0f33d7d69cc5b416211`  
		Last Modified: Wed, 12 Apr 2023 00:44:24 GMT  
		Size: 50.3 MB (50310899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145bb18c860aae65312434f79bce9d784a4824ef455202efca0f687a388037fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 9.3 MB (9263774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2063c41d1dff24f54b6a7d8edde21610fe37e02b35ed369be0ccf9f64cdc43fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 11.8 MB (11827096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1cb13e8dab0a14d667e4d9b265c749ae59a611e6862763377f1c8e34e0112c01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68902391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54d7ab7b13f29c59bc95210628c83870c56bc3b074d787b15d305d64a13d17d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:18:32 GMT
ADD file:2d913f7b6c2e804834958b3d144bd7b5150a438e2aaa73cdf2f1be1c64d10100 in / 
# Thu, 23 Mar 2023 05:18:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:83c1a140184ad386a37a5446dba474a2a8498dff7ae8d2ccd2957aaf8dc1682e`  
		Last Modified: Thu, 23 Mar 2023 05:26:35 GMT  
		Size: 49.3 MB (49291603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaeb19ea7953e3c0a2cce0d76910d46a1fc5e289c90379ecb81b3e5ba2a0c16`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 8.4 MB (8439874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecc4eca24f781c1e786d1fc88cb24202f1248f85adc06cf1b375f5607ec2d93`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 11.2 MB (11170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:85bf0cae57000ef766ea7ed7d8f16d94925cfc5dfe0ffdef79a82c81cfdb0bd8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75136981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f95dec386d645db16ef52d1d12753c4acc5e8cd37261e08c733828e13efe122`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:20:05 GMT
ADD file:3534cf3f10dae5b70c64865fd70cf5b9aa6ace6be9caa2d69518d6d59c4943fa in / 
# Thu, 23 Mar 2023 01:20:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:18:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:19:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8de2c12bac6cdfac096a845424e637222b157d221d8080dfc0e3cd14581716d5`  
		Last Modified: Thu, 23 Mar 2023 01:24:47 GMT  
		Size: 53.3 MB (53290173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ffcd14b130bc950e2e794bcf2e09ddffa8e18668803aa384fc8de743e9d8d2`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 9.7 MB (9661589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecca2a654e1b66be833e49110ac475ae4995f36d83ba12ad0396e8f4cf953872`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 12.2 MB (12185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:b6ecdf5c65f021e05c80106a2cc8a598f2fb062039c62b358a2a42fc40f3d4d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64406378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc1ea8528f7edf3edcdff9fd62663fec45eaf492953562405ce7f8504695160`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:05 GMT
ADD file:b8c0cf42f791d92283c2c47cf2ed446fb98a7cde685c9b923c89cadb86ddad31 in / 
# Wed, 12 Apr 2023 00:09:07 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:32:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6178d7c3b8603b1579d72ad9f5bda8fd22627feccccd498dad946eddfe96d27a`  
		Last Modified: Wed, 12 Apr 2023 00:12:25 GMT  
		Size: 45.5 MB (45494949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd056fe810f7c94134b5c26af6939949c18bfa4868dbc9f81ea8d7a25a0daf4c`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 8.1 MB (8117374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f8d5394c046224d62d5170fd151d4339e0f5131b1503bf3eafecefe1ec7a10`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 10.8 MB (10794055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2a32ff0d5208b6ad040a9cb58b776824b3c95030e002745b9128549a0e88a98e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67666740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d98184dbb030d39270ec3b57dcd40af7dc1cb4c8755f6afe805779ab651c12`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:19 GMT
ADD file:0593fbca11f3d4a9b2b916ee99bb70651af04ea1275262f12e9b0e5c07e81f0e in / 
# Wed, 12 Apr 2023 00:01:29 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:28:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1844a6b5cc32e25703d3a6ac2115866157b1f856d7463d0dca8443fea51061f1`  
		Last Modified: Wed, 12 Apr 2023 00:05:31 GMT  
		Size: 47.7 MB (47665068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f306dc6c45f3e2637390b46a2dce7fb061bb8be6ae7c72c47bba97d84b99d256`  
		Last Modified: Wed, 12 Apr 2023 00:33:37 GMT  
		Size: 8.7 MB (8713548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676682574fe22f1cac8016a4f36ad54898c4313e0609a7e88e75e035e32444b`  
		Last Modified: Wed, 12 Apr 2023 00:33:36 GMT  
		Size: 11.3 MB (11288124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:b1ae960627b5c823f2a9f1b9a5985b38e09b4277cda102446472f1ddf77ccde3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d9f6278d7e0c871b5bcdc327298a29c7c00a8a0504891c4ad2631c374b75a01c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134049910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd617366d1cce33570b6dcf04f7eac2404f89e0bece798cb7e973cbd704f667`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:55 GMT
ADD file:0936f6fccda991ba27a7f73ca61c23a436b7ca417e504b66d5a68f2283e1e81d in / 
# Wed, 12 Apr 2023 00:20:55 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:54:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:54:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:003dca91ec623536e08abc4e1bb2849836a84c44f82e24b97fd5423162a4d46e`  
		Last Modified: Wed, 12 Apr 2023 00:25:13 GMT  
		Size: 49.3 MB (49287652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486f0b6179599c75a087e6850c42ef248d973e29a6898ed99c9bccdae08d2cd2`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 9.1 MB (9082764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f184ca8dda7ed83dd9d21d6c880d4e15976f35814156a0a67df81423067f4b8`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 11.4 MB (11422423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76159e5040abc54c8e269f5e87ba68551c98fa9a6a06c9d7af5eae5f9f3ee57b`  
		Last Modified: Wed, 12 Apr 2023 07:59:41 GMT  
		Size: 64.3 MB (64257071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c0b4a3eae58bd274c266cb60478e79df6446cb058ebcb7beec816064f9c69b75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129365563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b15a5f5bf525f6d5ed1af6bc9d3b44768864d1199c3f26e961d670e918851d7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:48 GMT
ADD file:b02c911309a1b69d235b76dab369d523653c62374b0173ee9f1b65017607f9d6 in / 
# Wed, 12 Apr 2023 00:48:48 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:18:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:18:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8699c4859220eb7e4f2a5ae13e4dd5f9143cb7144e2a02a3eb381a79416524bf`  
		Last Modified: Wed, 12 Apr 2023 00:51:27 GMT  
		Size: 48.1 MB (48109671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b565bf44c40ab65f5193c4fbfd752809f50e95e2c4b2397728f42419979d7c`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 8.5 MB (8522810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8db076a21199a98e758a14876a91c9a890bb606e6d9d483862bcb73bc5cfbb`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 11.1 MB (11065853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466720607b58ed4036916fa9d7cb2e82a3ca95f0e5ec8e2ef908744cd3e409ec`  
		Last Modified: Wed, 12 Apr 2023 01:22:44 GMT  
		Size: 61.7 MB (61667229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1bcd239105aa63dc35ccb13a3762579403f20339f19a8b5e4e3fa462e8efc5c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124157820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f8c81ddf581c824df2e636b5d3c3658ea69e1ee1d68768b20b0c899586cd2f8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:28:43 GMT
ADD file:628ac1300ca273dba23c7d617164bc6e664cdebb4106910020d7b3dcb39429c8 in / 
# Thu, 23 Mar 2023 01:28:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:42:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:42:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:42:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53d7f1f008e91cd29c47c933b404c16fc1d4cf64b8699ad1269e882f53ca6e2d`  
		Last Modified: Thu, 23 Mar 2023 01:34:10 GMT  
		Size: 45.9 MB (45911196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61016f9e9c2f44cda61da9f54267fbafe7fef3695caec3c87c6d5ae9eb452ae4`  
		Last Modified: Thu, 23 Mar 2023 12:46:05 GMT  
		Size: 8.2 MB (8168245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4226b16c6b7093dc765001b6e5615e8150c8d19be6c96ea1171e1ad13654f5`  
		Last Modified: Thu, 23 Mar 2023 12:46:04 GMT  
		Size: 10.7 MB (10704470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889e5e2259a7026a6a42309e4673ccd18c4288dce5b85e2039cb7238e36ce3fe`  
		Last Modified: Thu, 23 Mar 2023 12:46:22 GMT  
		Size: 59.4 MB (59373909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:909145f5f8b9a67acd7be2b62e379fe6c15950dee01727de50e4cc961c962502
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133786279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c7d9c27ae042d56e7ca69c21a7a5a690294d166c8196d78574264d9160d8957`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:21 GMT
ADD file:2784bc6dba1e1dbea293e074ebf51fa7d89cb5545ea63ba2ed75b74d067387d4 in / 
# Wed, 12 Apr 2023 00:40:22 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:10:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:10:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:10:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43d214f7ab3ca35a0c9ed4d8cdf62b36248aba2fa1bbac4ecd64e82ba2520b70`  
		Last Modified: Wed, 12 Apr 2023 00:43:58 GMT  
		Size: 49.3 MB (49327656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d9e5d2b2df062d16ffea4a022a4c09ce904fb96ec3fa4712a1d936593ae2a`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 8.9 MB (8915031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd2b1a4cab3b4ac2bb4a7e9aaaa60ce806e3c49a8726f7baf5a10ba5e0e89fb`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 11.4 MB (11389544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff14914c0381e1889d1db49b1b39da80ae3a347cf1af048e2ae0eb42aec87a12`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 64.2 MB (64154048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8e5134589fb0e6d388a1a4741142104956636747431cf809398cd58520b6da78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137529120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acc693ca7c37b5ced8d79a021265f81c4cecbc277909bb33bb103fd1302a0b37`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:51 GMT
ADD file:31710a830769b5e1f2612e1cd05380f677714bf52f61a54adbc7424087fd1378 in / 
# Wed, 12 Apr 2023 00:39:52 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:11:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35e4af56b8bda58bf958814bc36c8e3a9a1d719c8582c0f33d7d69cc5b416211`  
		Last Modified: Wed, 12 Apr 2023 00:44:24 GMT  
		Size: 50.3 MB (50310899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145bb18c860aae65312434f79bce9d784a4824ef455202efca0f687a388037fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 9.3 MB (9263774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2063c41d1dff24f54b6a7d8edde21610fe37e02b35ed369be0ccf9f64cdc43fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 11.8 MB (11827096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3196dd70f259df7354dba37d732f79f68e602883ec8838b2cfcd0515de5c5c`  
		Last Modified: Wed, 12 Apr 2023 01:17:49 GMT  
		Size: 66.1 MB (66127351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1fe2cb894be2bc55a95b04e66763ccec91305b7c7ac438bca7d21d751c7809b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (132001554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e553975cc4545e2dfa4c801fc4f1bfe90378add106afcf9e70883c34024f725c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:18:32 GMT
ADD file:2d913f7b6c2e804834958b3d144bd7b5150a438e2aaa73cdf2f1be1c64d10100 in / 
# Thu, 23 Mar 2023 05:18:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:24:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c1a140184ad386a37a5446dba474a2a8498dff7ae8d2ccd2957aaf8dc1682e`  
		Last Modified: Thu, 23 Mar 2023 05:26:35 GMT  
		Size: 49.3 MB (49291603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaeb19ea7953e3c0a2cce0d76910d46a1fc5e289c90379ecb81b3e5ba2a0c16`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 8.4 MB (8439874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecc4eca24f781c1e786d1fc88cb24202f1248f85adc06cf1b375f5607ec2d93`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 11.2 MB (11170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3768b306fba92d6a836552b3ee3a1bb755cd0f7d6618ca028d0643fde06553`  
		Last Modified: Thu, 23 Mar 2023 07:37:53 GMT  
		Size: 63.1 MB (63099163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cb552cfa8fffc38c06c010861606d8318ff8a2aafec75e73f34a9cf665dfbcc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144877314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5972c8f16c43d5fbd1f3bb72c145ccaef4bbf62a487929661df73dadb607568`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:20:05 GMT
ADD file:3534cf3f10dae5b70c64865fd70cf5b9aa6ace6be9caa2d69518d6d59c4943fa in / 
# Thu, 23 Mar 2023 01:20:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:18:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:19:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8de2c12bac6cdfac096a845424e637222b157d221d8080dfc0e3cd14581716d5`  
		Last Modified: Thu, 23 Mar 2023 01:24:47 GMT  
		Size: 53.3 MB (53290173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ffcd14b130bc950e2e794bcf2e09ddffa8e18668803aa384fc8de743e9d8d2`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 9.7 MB (9661589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecca2a654e1b66be833e49110ac475ae4995f36d83ba12ad0396e8f4cf953872`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 12.2 MB (12185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5053cb00528479013fa5db3eb35bb36ff11628a7f8c9c6ae0310021f09a7005`  
		Last Modified: Thu, 23 Mar 2023 13:26:59 GMT  
		Size: 69.7 MB (69740333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:bcd300a4e07d706f2fd9f306c4c32864622137e94ae3c3c4670ea905ee0beff3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124147555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:397d717b57a8049a3da1ad949d9ed38c1e6d2518bf8f6c629c18545c03f04445`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:05 GMT
ADD file:b8c0cf42f791d92283c2c47cf2ed446fb98a7cde685c9b923c89cadb86ddad31 in / 
# Wed, 12 Apr 2023 00:09:07 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:32:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:35:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6178d7c3b8603b1579d72ad9f5bda8fd22627feccccd498dad946eddfe96d27a`  
		Last Modified: Wed, 12 Apr 2023 00:12:25 GMT  
		Size: 45.5 MB (45494949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd056fe810f7c94134b5c26af6939949c18bfa4868dbc9f81ea8d7a25a0daf4c`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 8.1 MB (8117374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f8d5394c046224d62d5170fd151d4339e0f5131b1503bf3eafecefe1ec7a10`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 10.8 MB (10794055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0c6cc5fb9f28304c05335b3e21ed5e3cce359b94731f04cc903938689ebc19`  
		Last Modified: Wed, 12 Apr 2023 00:45:23 GMT  
		Size: 59.7 MB (59741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ab7bb732a3d488865f2b887c55fbefc2e0041d528429e377f1f5ee84b43bda25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130927162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dba9e0d63f399d18f4d3f0cd3f58b4eee0e1d16c71d855c9f9b0bd4e250d67b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:19 GMT
ADD file:0593fbca11f3d4a9b2b916ee99bb70651af04ea1275262f12e9b0e5c07e81f0e in / 
# Wed, 12 Apr 2023 00:01:29 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:28:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:28:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1844a6b5cc32e25703d3a6ac2115866157b1f856d7463d0dca8443fea51061f1`  
		Last Modified: Wed, 12 Apr 2023 00:05:31 GMT  
		Size: 47.7 MB (47665068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f306dc6c45f3e2637390b46a2dce7fb061bb8be6ae7c72c47bba97d84b99d256`  
		Last Modified: Wed, 12 Apr 2023 00:33:37 GMT  
		Size: 8.7 MB (8713548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676682574fe22f1cac8016a4f36ad54898c4313e0609a7e88e75e035e32444b`  
		Last Modified: Wed, 12 Apr 2023 00:33:36 GMT  
		Size: 11.3 MB (11288124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f9748f029581dd4821ad6e7d4da7ab4a31600128a2411dda2639c9b92fe58`  
		Last Modified: Wed, 12 Apr 2023 00:33:51 GMT  
		Size: 63.3 MB (63260422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:422b4400e1ae3a5aa208dc236e3dc05e3db66b72387ac2d7b11bee187ff87f7d
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
$ docker pull buildpack-deps@sha256:4156d4c78d3e29a9aa11a5528a08847352e66895bb0a75cec05f4d43752fb8f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322492485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09bd8b383fcae8260115c949f68a3ccbe1df72567c4e1ad6f53b72329c1c5e1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b89f3c7f7da8adf032a33a75d1b659cee33179ecb88ea0ba75e4fc58ebe63a6`  
		Last Modified: Wed, 12 Apr 2023 07:57:46 GMT  
		Size: 54.6 MB (54584801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d62772179761f8fddfaed03ed2bdf7078b103b193d18d79a9b49364830d56cf`  
		Last Modified: Wed, 12 Apr 2023 07:58:19 GMT  
		Size: 196.8 MB (196811503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:5307e4d5147eb64f430d2a521eee4a5504ed8c4a0d7d98aa81c28190c2c963d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295551904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62bc4c385631ea22e58568f3c02e7102b4f9f8f5a1ebb96d7e82bf8764dbecae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:15:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:16:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:17:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49db155cdf8645f599affcbbbc75eb928b0a9d010c4ac54afcfa9d7e4fa85e0`  
		Last Modified: Wed, 12 Apr 2023 01:21:15 GMT  
		Size: 5.1 MB (5072827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936087cbd048148575fda58348506149db80a2699e99ae2042086628c0e5a38`  
		Last Modified: Wed, 12 Apr 2023 01:21:16 GMT  
		Size: 10.6 MB (10573853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0bf11569c39ee4f3d8515112046a55f14f39e54c6f0ea26271033c090f77d2`  
		Last Modified: Wed, 12 Apr 2023 01:21:35 GMT  
		Size: 52.3 MB (52340617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622390f39404d88752f248bc2136a55baca97d5324d43689204df0157d284282`  
		Last Modified: Wed, 12 Apr 2023 01:22:13 GMT  
		Size: 175.0 MB (175009432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f9e1d777129a6edd74d7bf1c46bceacdb0494da93b4f6f30b9e3e1ddc047be34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (283008120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49b8799c6deee224d45f54f351a870631cfae0b6039cfe91ea6c3adf9a1810e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:41:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca667140ff247fc759283fc9ff4cafbe304d1777ffc70e1bd593b63151c31a`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 4.9 MB (4934357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879c254431e9965afb23e55a148faffd29450a9218269f769be95d6e9673a93`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 10.2 MB (10217859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64c4a1b9916f6da6f286835522f27f11a812694e5f878e87468d4c6b90b343e`  
		Last Modified: Thu, 23 Mar 2023 12:45:20 GMT  
		Size: 50.4 MB (50355514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862d41b96b9b8c37267f9bb50226c9d63fc5a8df2310f511837355e187e090a`  
		Last Modified: Thu, 23 Mar 2023 12:45:51 GMT  
		Size: 167.3 MB (167288602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e7277cb741804ffe9213d32a419f6738ef4494fbd33db9326b55282dfbc1dd6b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.1 MB (314135667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c57708eddbf78525fe399f52d71e35653f6c3298641025d07fcc3323777584`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:07:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f993d5b17f32f4b8a535c25e182e5d8412625beee450e513ca57036e8fdd6dc`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 54.7 MB (54676038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26edf98ece5babdb6b65e76738cef2c2d05e7075161753d3ba95cd84480d211`  
		Last Modified: Wed, 12 Apr 2023 01:14:02 GMT  
		Size: 189.7 MB (189727693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ff274b300c58e39b8abdacecdee25d47651abe32a696616b92656ca392bd5d21
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.2 MB (328223380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5eee57e4ddbeaa9219392349db2bc711541f424d58a97b4a86ad5bd768ff773`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:06:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:07:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ccf9a5e34ba2345ce265a9a11c93ee254e1f3616dfd1c1deda6e2f7d614c8`  
		Last Modified: Wed, 12 Apr 2023 01:14:53 GMT  
		Size: 5.3 MB (5293626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4988d5e4328f031f6884a7351766aa8a2806c9cdca38d354477fc537eaa4911f`  
		Last Modified: Wed, 12 Apr 2023 01:14:54 GMT  
		Size: 11.2 MB (11249875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660a2befd486d43a308dd1561f57efeafe1f13defd6439d34aeb5efec783ee3d`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 55.9 MB (55922746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f09985282f12d05c5724bcbb0481a94f66820112bafc34a1d990dfdf74a52fc`  
		Last Modified: Wed, 12 Apr 2023 01:16:02 GMT  
		Size: 199.7 MB (199724315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ec42db429d0c72964b3b977754bc6918c60d4bf420eae2d6e4a643f9213a7305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301083947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537e8272f594cfb2548e2fb1974050af3569e7a7791f1ed883845f968edd9f25`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:15:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:21:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f79f6951926609a68e21aee7e612375637f7c12703c62b028fd60a22e2d9bfd`  
		Last Modified: Thu, 23 Mar 2023 07:34:02 GMT  
		Size: 4.9 MB (4922133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b6297024241cbdae60b7afa1bce7cc669d998e17b209e8b133df9e13da064`  
		Last Modified: Thu, 23 Mar 2023 07:34:04 GMT  
		Size: 10.7 MB (10662010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9437ab03a3b730ed3d31f18a79500c8ce379f2a971ed27695d60f38e887121b2`  
		Last Modified: Thu, 23 Mar 2023 07:34:50 GMT  
		Size: 53.3 MB (53306810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173435a2410e4cdc681e9bd4a44f44da5e7905b9826d94efbc91429ed38126f1`  
		Last Modified: Thu, 23 Mar 2023 07:36:46 GMT  
		Size: 178.9 MB (178928274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:474394b72495ae1d639248919c45100c0ee19cbc80fb7c3c85583baff857f075
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330989722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021c337c98a3039aa29eead547f736d517042181f44162b2088727645ce4a56f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:15:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:16:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:18:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805b891b319592a15b7da9a474b2f36e32ed9b8a720d14bbbe4d08422343b19`  
		Last Modified: Thu, 23 Mar 2023 13:24:55 GMT  
		Size: 5.4 MB (5415174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdb7e2b62c4c7c555894be507d7ccaf7aeca0f8c9088a9082ad4cd37dc97f28`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 11.6 MB (11629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac3f4f172050b21a6f17c30c60794779e7d5c150f1111240477b89240ad7f6`  
		Last Modified: Thu, 23 Mar 2023 13:25:22 GMT  
		Size: 58.9 MB (58864543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc2fa2e478c864805494dbe6350071ba59af5a4f830abf55dc17559fb0228fa`  
		Last Modified: Thu, 23 Mar 2023 13:26:19 GMT  
		Size: 196.2 MB (196159312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:478709c66fdeffea827bb22297605067d97172933185294b18da02b3b071e7a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296079415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62811c5341c95a39adc789318a1ba301b0fae01b6b77e3b4a63a1693c43fa76d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:27:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2973b8c98f9da7833ab9cd69185dd958a8939a30136cdcfedb66ce775db358ee`  
		Last Modified: Wed, 12 Apr 2023 00:32:48 GMT  
		Size: 5.1 MB (5149313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f740d13ac612bf8b6489559a7945ec1439fee2d5eba455ab0db047cd3f30a9a`  
		Last Modified: Wed, 12 Apr 2023 00:32:49 GMT  
		Size: 10.8 MB (10766104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c0067783f401b099adca196dce9e464e66236e49faba106e2f04ac73a90df7`  
		Last Modified: Wed, 12 Apr 2023 00:33:02 GMT  
		Size: 54.1 MB (54061843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b5accdd9fd68a290692e1a0a3d853312f236ae0463540b5fdd97d598cc7a6`  
		Last Modified: Wed, 12 Apr 2023 00:33:28 GMT  
		Size: 172.8 MB (172815473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:f741d28fe1b0cc0efb79143127f1976105e90bcd5f8d3ee1156b614359102f57
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
$ docker pull buildpack-deps@sha256:acd62d4d9773006a9d0acddc08a4cbf7637d1c975e67459b52a7dc093bdfc271
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71096181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af19f7b630d3d79df60c6a9ae3051940c35c240094ef6e54f4f7843577467896`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:03091d90e79cf371dee743c2a8537556060a22246a5c1a68d53f63e201715f4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68201855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39fd3f1fac0693a3efcdf720af9216deb72c54ed024f9c8edfa061944f26d405`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:15:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49db155cdf8645f599affcbbbc75eb928b0a9d010c4ac54afcfa9d7e4fa85e0`  
		Last Modified: Wed, 12 Apr 2023 01:21:15 GMT  
		Size: 5.1 MB (5072827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936087cbd048148575fda58348506149db80a2699e99ae2042086628c0e5a38`  
		Last Modified: Wed, 12 Apr 2023 01:21:16 GMT  
		Size: 10.6 MB (10573853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1a22995743cfb2d45a6e602149e28ca1cf97d11b4cfcfc399ef35af9031dd5e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65364004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24957d317bdf2878226957903bdd121664355551e42b707fa62dd818a6d62b9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca667140ff247fc759283fc9ff4cafbe304d1777ffc70e1bd593b63151c31a`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 4.9 MB (4934357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879c254431e9965afb23e55a148faffd29450a9218269f769be95d6e9673a93`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 10.2 MB (10217859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a5537c32568d575a5a3bb0f96138a7cf42dc7d590729308b1ed7538fbdd433e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69731936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0130b5aae27ce4286f62ae8a2e5324e811b8d862aa0aea6923a7b461615ccf17`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:39321899797ed2861f1e87a3547e2e911faa2ce033098728aa240b793dd8232b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72576319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1535cd25f9ea155765a6cae9f83a5e50a533888ddb926700a119b7e91a0a0f1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ccf9a5e34ba2345ce265a9a11c93ee254e1f3616dfd1c1deda6e2f7d614c8`  
		Last Modified: Wed, 12 Apr 2023 01:14:53 GMT  
		Size: 5.3 MB (5293626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4988d5e4328f031f6884a7351766aa8a2806c9cdca38d354477fc537eaa4911f`  
		Last Modified: Wed, 12 Apr 2023 01:14:54 GMT  
		Size: 11.2 MB (11249875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:789809484997dabb78f971ed5b5198ad03b3c5b386ff5390bf32623ca9f71d48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68848863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b9683947fb7fece88ffefd3d805752e5e334f37bb5341634f0f876c6312227`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f79f6951926609a68e21aee7e612375637f7c12703c62b028fd60a22e2d9bfd`  
		Last Modified: Thu, 23 Mar 2023 07:34:02 GMT  
		Size: 4.9 MB (4922133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b6297024241cbdae60b7afa1bce7cc669d998e17b209e8b133df9e13da064`  
		Last Modified: Thu, 23 Mar 2023 07:34:04 GMT  
		Size: 10.7 MB (10662010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2200286e371e1ef3505ddd402bec8d821eddd2e8315003a4fd7bd3d43cfa7b4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75965867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa7c4a6c3a4cac50b9dcd36af9e7bf0ce438b9c24e26debfb67020874d078cb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:15:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805b891b319592a15b7da9a474b2f36e32ed9b8a720d14bbbe4d08422343b19`  
		Last Modified: Thu, 23 Mar 2023 13:24:55 GMT  
		Size: 5.4 MB (5415174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdb7e2b62c4c7c555894be507d7ccaf7aeca0f8c9088a9082ad4cd37dc97f28`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 11.6 MB (11629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5726b9b13d1328b42898380f57612273babbfe94f7918919e3553ca203957c96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69202099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d3f520b42352a1bbcb04c9c67c162e7870ac7063005e1cbfb804dea99188dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2973b8c98f9da7833ab9cd69185dd958a8939a30136cdcfedb66ce775db358ee`  
		Last Modified: Wed, 12 Apr 2023 00:32:48 GMT  
		Size: 5.1 MB (5149313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f740d13ac612bf8b6489559a7945ec1439fee2d5eba455ab0db047cd3f30a9a`  
		Last Modified: Wed, 12 Apr 2023 00:32:49 GMT  
		Size: 10.8 MB (10766104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:4fba0beac07f82d041571a394110dca419cbb71285de82105ae04e9c7401fd9c
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
$ docker pull buildpack-deps@sha256:22e8a94a63b1cf94bc6e69418b975d41cb9ca48640b8b3a48002eb9c65039abb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8cd24e709af1ad98665077ad3ae2b89451839cb3a36350db232d6ce523d0d60`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127e97b4daf784e08840a21765f0d4f251192ef2994d0e4a253490f81e63955b`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 5.2 MB (5166696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0336c50c9f6942b660e433b1086238eec37057c34b14c4e3b28bd7bf05bd84ba`  
		Last Modified: Wed, 12 Apr 2023 07:57:29 GMT  
		Size: 10.9 MB (10876749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b89f3c7f7da8adf032a33a75d1b659cee33179ecb88ea0ba75e4fc58ebe63a6`  
		Last Modified: Wed, 12 Apr 2023 07:57:46 GMT  
		Size: 54.6 MB (54584801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ea05ef84678632f8c536876f2c7f5fc619fc524fc4b7dea24106ccb4b55809a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120542472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640f06156014acf4823a54fa99d9d265ad6efe6eda17f48174918044c3a2ea19`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:15:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:16:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49db155cdf8645f599affcbbbc75eb928b0a9d010c4ac54afcfa9d7e4fa85e0`  
		Last Modified: Wed, 12 Apr 2023 01:21:15 GMT  
		Size: 5.1 MB (5072827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936087cbd048148575fda58348506149db80a2699e99ae2042086628c0e5a38`  
		Last Modified: Wed, 12 Apr 2023 01:21:16 GMT  
		Size: 10.6 MB (10573853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0bf11569c39ee4f3d8515112046a55f14f39e54c6f0ea26271033c090f77d2`  
		Last Modified: Wed, 12 Apr 2023 01:21:35 GMT  
		Size: 52.3 MB (52340617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4e954e4c9de72e8e1118eb94583ab2f5f6dde3064d1c9ac34b712cd3ba6a1f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115719518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c576aa271c58013d567de0474bf19f0a9b589c98e78c3e2609b5f4dccb1bfc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca667140ff247fc759283fc9ff4cafbe304d1777ffc70e1bd593b63151c31a`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 4.9 MB (4934357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1879c254431e9965afb23e55a148faffd29450a9218269f769be95d6e9673a93`  
		Last Modified: Thu, 23 Mar 2023 12:45:01 GMT  
		Size: 10.2 MB (10217859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64c4a1b9916f6da6f286835522f27f11a812694e5f878e87468d4c6b90b343e`  
		Last Modified: Thu, 23 Mar 2023 12:45:20 GMT  
		Size: 50.4 MB (50355514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8932a28128c9d2abaed3ae68d2641c6738ab07bf083ca8886920e13ce37bbce3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124407974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d7143247bb9728129c637c315a5d5529383d57dfbf55c6999d1479a6f6dee2b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:07:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5884e7f2c8c61aa845de4902fc29639b58861ae6c2d80bafe82082c0456c0740`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 5.2 MB (5152752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b792b01ed3c8dc1488cd8aac41ab7d49bb17f3fa22b2e6c846078cec81a1c00`  
		Last Modified: Wed, 12 Apr 2023 01:13:17 GMT  
		Size: 10.9 MB (10873655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f993d5b17f32f4b8a535c25e182e5d8412625beee450e513ca57036e8fdd6dc`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 54.7 MB (54676038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2af50719cfc3c1165d1e75a99045d98388d375c4dcf2cafd5526a78d50080eab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128499065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863e942eeec226faacc53f695802b0b24e7dd766b5e4a9498a0d7c62e92c702`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:06:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37ccf9a5e34ba2345ce265a9a11c93ee254e1f3616dfd1c1deda6e2f7d614c8`  
		Last Modified: Wed, 12 Apr 2023 01:14:53 GMT  
		Size: 5.3 MB (5293626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4988d5e4328f031f6884a7351766aa8a2806c9cdca38d354477fc537eaa4911f`  
		Last Modified: Wed, 12 Apr 2023 01:14:54 GMT  
		Size: 11.2 MB (11249875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660a2befd486d43a308dd1561f57efeafe1f13defd6439d34aeb5efec783ee3d`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 55.9 MB (55922746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a9ec515744077c37744762c48a381049165872c3140692bfa932f9cec2efd549
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122155673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6653fbf81293b8dbce803c3de0330f89c7b15f3d502575b1d0c255336c26a706`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:15:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f79f6951926609a68e21aee7e612375637f7c12703c62b028fd60a22e2d9bfd`  
		Last Modified: Thu, 23 Mar 2023 07:34:02 GMT  
		Size: 4.9 MB (4922133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b6297024241cbdae60b7afa1bce7cc669d998e17b209e8b133df9e13da064`  
		Last Modified: Thu, 23 Mar 2023 07:34:04 GMT  
		Size: 10.7 MB (10662010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9437ab03a3b730ed3d31f18a79500c8ce379f2a971ed27695d60f38e887121b2`  
		Last Modified: Thu, 23 Mar 2023 07:34:50 GMT  
		Size: 53.3 MB (53306810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:308a8f8623e3d18d4ca7d0dcbd1fc6759e17b9a128dde3c2f263439cba80795c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134830410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5026643d3fb952f674886305718eb0a8a22bc3e0a6ba7cf3c44b76b61ce8d04`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:15:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:16:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805b891b319592a15b7da9a474b2f36e32ed9b8a720d14bbbe4d08422343b19`  
		Last Modified: Thu, 23 Mar 2023 13:24:55 GMT  
		Size: 5.4 MB (5415174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdb7e2b62c4c7c555894be507d7ccaf7aeca0f8c9088a9082ad4cd37dc97f28`  
		Last Modified: Thu, 23 Mar 2023 13:24:56 GMT  
		Size: 11.6 MB (11629667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac3f4f172050b21a6f17c30c60794779e7d5c150f1111240477b89240ad7f6`  
		Last Modified: Thu, 23 Mar 2023 13:25:22 GMT  
		Size: 58.9 MB (58864543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dfe7b376859cc874a19230408e2042b1d984722eca290ce8cced0e27c6bdc7bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123263942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0184582450f7852885e4f2a6aaf51c5ec9ce0ff2ce9cd9b877a945b87bfd33c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:26:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:27:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2973b8c98f9da7833ab9cd69185dd958a8939a30136cdcfedb66ce775db358ee`  
		Last Modified: Wed, 12 Apr 2023 00:32:48 GMT  
		Size: 5.1 MB (5149313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f740d13ac612bf8b6489559a7945ec1439fee2d5eba455ab0db047cd3f30a9a`  
		Last Modified: Wed, 12 Apr 2023 00:32:49 GMT  
		Size: 10.8 MB (10766104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c0067783f401b099adca196dce9e464e66236e49faba106e2f04ac73a90df7`  
		Last Modified: Wed, 12 Apr 2023 00:33:02 GMT  
		Size: 54.1 MB (54061843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:acbf47c1484ea66ab4481e7cd1e28e4cf13d33200ff604e572c5d59bda54a9d7
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
$ docker pull buildpack-deps@sha256:d2831f26a1be4155a536403a4091c9fa3578d932016713ad45c204a54ef9bbe0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.9 MB (345874026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8740ff589a8566528392543b04f5042041d597aebdf89a8351ad91a78b3c798`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:35 GMT
ADD file:1cb6c660a2e3ea14b2a11bb8b80f53920c3da423a0ad7004391bfab4db4d0177 in / 
# Wed, 12 Apr 2023 00:19:36 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:48:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:49:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:49:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:50:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc556c281183180fae02d57fa6fb60ed0a99d9040936278743dc4022bfb0c686`  
		Last Modified: Wed, 12 Apr 2023 00:22:48 GMT  
		Size: 49.3 MB (49292938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8022b43d7c31d74c341d297cf10031ff0c51f596473a0c1945ee83a841094638`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 9.1 MB (9083160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db75f726ec67539c4823cb16851963ebe5838a853b0e769fd662020fad918781`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 11.4 MB (11422437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8a9e299258b84de99d6d739eb84b5b1632005f9c7723f2dd9e209fb1a8aaa3`  
		Last Modified: Wed, 12 Apr 2023 07:56:46 GMT  
		Size: 64.1 MB (64097699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5269c0251f891649bf20972368b34411b22208df54ce5c4b1b9eb649793edbb`  
		Last Modified: Wed, 12 Apr 2023 07:57:20 GMT  
		Size: 212.0 MB (211977792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ca3000a5c2c81e15247951e66c081c65117913ded0f177159d6c15adf29997c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.6 MB (314581039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7816bfe042349b0c7c87b9c180f83b2294e7e688a27afa564c62ce1bbbe48fa1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:19 GMT
ADD file:df1103dce44baa95c92287ab5016f36d5cc45c6062116ebf5273f7e79a00915c in / 
# Wed, 12 Apr 2023 00:48:20 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:15:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:795c0ca2726dffdb0e5ef6ffa341d17ec672d5915011f1a93a05e8c95a4779ae`  
		Last Modified: Wed, 12 Apr 2023 00:50:12 GMT  
		Size: 48.1 MB (48110879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e70c1a23fdf0fd320a61a2506f0ca4a391a319de8403734e4af8d678a6081fc`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 8.5 MB (8523001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27111cd5fb1057675f2e0b269790dc264d344d6e4b7ad92ff941f90a496167b`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 11.1 MB (11065924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ed8d7f4b0f78246beda91a51ddbc4ab368fe6f04bb2432498c3f5a76cbc010`  
		Last Modified: Wed, 12 Apr 2023 01:20:30 GMT  
		Size: 61.5 MB (61541287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7bffea89dcea5595c3a9d4dcd9ae2c5876dacb4265050ed658554b4d6da420`  
		Last Modified: Wed, 12 Apr 2023 01:21:06 GMT  
		Size: 185.3 MB (185339948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:83c7e12691e98dd0fc20a10fe128ccd02202938fe42a4dc9b838336aed51bceb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.9 MB (298938719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aba0af1fa024bb80f3fd7118949ea96c3eb4605028f55e173a2140e1703915e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:09:37 GMT
ADD file:084e44d77ffdb8aad1f856ec10db87922bdba3a90e06f9f1cafcb6e4284c8ff7 in / 
# Thu, 23 Mar 2023 01:09:37 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:37:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:40:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b14dce67c2fdb37d2b0eacccff5119e226c45c2906f12d6ee93d8850400824b`  
		Last Modified: Thu, 23 Mar 2023 01:32:34 GMT  
		Size: 45.9 MB (45889194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395ab26b892c3659080680521b7e37b5cee24838f59696a77cfd944e93ccd158`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 8.2 MB (8168514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788f0ce3e6e5ae63843a828f2542045686f8131e60c22d54846351e88422de`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 10.7 MB (10687642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9a3318c652dc50d1377b04d3c6d10a08df4155179df516ddbb594b1e7df246`  
		Last Modified: Thu, 23 Mar 2023 12:44:21 GMT  
		Size: 59.2 MB (59244953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23277d44a430ca9622032448c2da0203a6bd89b1246d243611b93d52ed2fa502`  
		Last Modified: Thu, 23 Mar 2023 12:44:51 GMT  
		Size: 174.9 MB (174948416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:93e13c1041833e26336a9a4362a935021cb140f05c425f7cda66b1d288da141d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (337000447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4817e1bdddcea21ae977e3e5b270332950842257559a3ae2efe4a18f83f1110e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:27 GMT
ADD file:efed18ef2a003bff7e64e7049455216e51876402083581032c35085328e416f6 in / 
# Wed, 12 Apr 2023 00:39:28 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:04:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:06:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0f987ce91d920ae0a705ed6c9824f1bbbfa282defb8986614030eb8e2bc0b4e`  
		Last Modified: Wed, 12 Apr 2023 00:41:45 GMT  
		Size: 49.3 MB (49345365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6a618ee06e99ebfbb7809c1cc4902cb717d294243f3765f170fd1c8eaf94a`  
		Last Modified: Wed, 12 Apr 2023 01:12:23 GMT  
		Size: 8.9 MB (8915044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c3f19470d2fd9e1407a7ddcbac3c316a999a143865347f221db18517e0838`  
		Last Modified: Wed, 12 Apr 2023 01:12:24 GMT  
		Size: 11.4 MB (11389565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b373ae05bf678c385bace283c65197a2bbc2a334c528ed7b58a01d93131de585`  
		Last Modified: Wed, 12 Apr 2023 01:12:39 GMT  
		Size: 64.0 MB (63974624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4f590cd785a4e380e2e92cca3c7b2d82be15d89bb52da582994cc39d9bdd5`  
		Last Modified: Wed, 12 Apr 2023 01:13:07 GMT  
		Size: 203.4 MB (203375849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:34c578f8d193ff514ac530b8922a3055877b2d87cc4e289f31e765c7450ed112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.4 MB (348376060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7d23d91b6b9538e488de01d18982225f2c00d113996363a9198e3a7dc32c14`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:30 GMT
ADD file:7718865253a3489583d40f8c7a7beede0c20cebbab68bb3e97ad2e84082afcb7 in / 
# Wed, 12 Apr 2023 00:38:30 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:02:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:03:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:05:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4ce9e81f634822e5166ef3eef875a4140795ac18afe0391433d72c7865bf67b`  
		Last Modified: Wed, 12 Apr 2023 00:41:43 GMT  
		Size: 50.3 MB (50317977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e54183fe5cb0866f886a93c0d098d38e649286a2b516b64d9658dd40f5d74b`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 9.3 MB (9264042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76896a8c48193a86329dc809066c177aedc76d55811eb32ca7c80c1ab06f66f1`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 11.8 MB (11827045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba7e1ed0df9a2a8a6501d91360cea22ab988653bf057d73c44ecb41e49f6151`  
		Last Modified: Wed, 12 Apr 2023 01:13:56 GMT  
		Size: 66.0 MB (65960427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4551baecfb99d1499518d7ef04818e3c6d649ec19322e320b452af6855389592`  
		Last Modified: Wed, 12 Apr 2023 01:14:43 GMT  
		Size: 211.0 MB (211006569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b771ae6c70d63080a0d7f3fa508cba380a502afe80ab68ab34979adbb4978d2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.4 MB (321358603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:045143f5b199fa1752d0c43df4c092cd488a99e790cf8a1b02d9edb5aaaa1645`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:15:54 GMT
ADD file:454bfcbdd9d738730885002e9124aea5e8eb4920ca5d3bf13bb9f4707023bd67 in / 
# Thu, 23 Mar 2023 05:15:59 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:03:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:05:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:12:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70edc5cd98f5a2e589d309248c77122dabf95f437c0448b99513b15ef209f244`  
		Last Modified: Thu, 23 Mar 2023 05:23:55 GMT  
		Size: 49.3 MB (49291654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74250ff8fd2374ebbb2086f535377d5246a78ee51939da5984dc42e7afe6d2f5`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 8.4 MB (8439840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c3b2ae326a6eb2a81faaff9322b317ad4788f4c53f6c3b6721724ed9f3d04`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 11.2 MB (11154181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce72fc6141c1bf4e5dcee62655f6469a6796ecc6186b5f6d227dd67b147c683`  
		Last Modified: Thu, 23 Mar 2023 07:31:48 GMT  
		Size: 62.9 MB (62937602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac50d1e65b3f5c0bb45b9748fbb137f77f5b7b2c56d8e39a47c9da1d4b420d05`  
		Last Modified: Thu, 23 Mar 2023 07:33:49 GMT  
		Size: 189.5 MB (189535326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:89a99f29891a6b80a810cf53b3c770ea325643cc1b97d0a5c10df49aeb6ee70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.7 MB (358668762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6399c6b33c24a1a9ef3642ece1d0265b6a626033822f24b9225f51bc1a08be09`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:18:49 GMT
ADD file:5e17f6075630657b8465309f99ecbfc57e325d159b54f58181b974526f2314a5 in / 
# Thu, 23 Mar 2023 01:18:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:10:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:11:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:14:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60e68956630003599038e3cfe86d6dd09ee874e8c30d9ea29b8350e0d3fa8497`  
		Last Modified: Thu, 23 Mar 2023 01:23:06 GMT  
		Size: 53.3 MB (53290316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcdbd51144dbb4a208e40072c2caf491305afb997e9161481db00137eefec5e`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 9.7 MB (9661293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bed649f1a85d37347952942e0ee256bdf515769a40a1c23cf02e65c6c90e6b1`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 12.2 MB (12168496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f138294734fe3a74e7b88ac5a9a4fe51653cff8b3ad0ba829039339f82a1a99`  
		Last Modified: Thu, 23 Mar 2023 13:23:46 GMT  
		Size: 69.6 MB (69563655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a3c96c81acee7018db01424d6026016ac1a292d63251b021cf094b1565fcde`  
		Last Modified: Thu, 23 Mar 2023 13:24:44 GMT  
		Size: 214.0 MB (213985002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f3ab35ffe09db7e9be153f5725015386c28800e98cb51a46e7c57187d5a0e602
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314808227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7150ecfe845b425b67f772c301e8610bfca04fb6c670705d638bd01b5dd34bb1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:19 GMT
ADD file:5d2b35b45a0f23e2f2e93f9c311eb34a92e4591ea27979236d801e512d44cb85 in / 
# Tue, 11 Apr 2023 23:59:31 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:24:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:25:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:26:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a09cd2374da8355612e7d4c91d55107a3f089816ae52b2c91b9e08e6a895ab1`  
		Last Modified: Wed, 12 Apr 2023 00:04:39 GMT  
		Size: 47.7 MB (47670407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d047361c12b2aeb253b1923b053dcc960101b3b3348af8f15f95f7fda2b89e4`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 8.7 MB (8713846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a462d218c24c21390b32ace449f4f47a57624b858dc05a37c31cb7f6e21c41`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 11.3 MB (11288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628da1a495c0341f28b24cb228c4984d7d8a718059c95991d67739f4a4602e4b`  
		Last Modified: Wed, 12 Apr 2023 00:32:14 GMT  
		Size: 63.1 MB (63101451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e16abe3590f67fe9ba9faa6530081d422098a3dabb4fd1cb81b378a88316bf`  
		Last Modified: Wed, 12 Apr 2023 00:32:42 GMT  
		Size: 184.0 MB (184034442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:ffce4af019ca05ac6bdf932121dba95eace904dc9236d899ed8c0f8287f80bfc
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
$ docker pull buildpack-deps@sha256:6a036620bf66ab7f03f891595654eae2995b8a08bb32443b8e130fa87c26c2b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69798535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e95348693c13cd4b3237dba422f5d46f3c7b727c7c451791d70fb9f93a80800b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:35 GMT
ADD file:1cb6c660a2e3ea14b2a11bb8b80f53920c3da423a0ad7004391bfab4db4d0177 in / 
# Wed, 12 Apr 2023 00:19:36 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:48:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:49:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cc556c281183180fae02d57fa6fb60ed0a99d9040936278743dc4022bfb0c686`  
		Last Modified: Wed, 12 Apr 2023 00:22:48 GMT  
		Size: 49.3 MB (49292938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8022b43d7c31d74c341d297cf10031ff0c51f596473a0c1945ee83a841094638`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 9.1 MB (9083160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db75f726ec67539c4823cb16851963ebe5838a853b0e769fd662020fad918781`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 11.4 MB (11422437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:66ba8371e61af6282fc38b6060f0c069dfedce71185d25e520e1124503a36408
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67699804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fc6c4cd7610510c3dbf367553fdb3b3d67108a1c4f5fef96d4fccbb8635f2db`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:19 GMT
ADD file:df1103dce44baa95c92287ab5016f36d5cc45c6062116ebf5273f7e79a00915c in / 
# Wed, 12 Apr 2023 00:48:20 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:795c0ca2726dffdb0e5ef6ffa341d17ec672d5915011f1a93a05e8c95a4779ae`  
		Last Modified: Wed, 12 Apr 2023 00:50:12 GMT  
		Size: 48.1 MB (48110879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e70c1a23fdf0fd320a61a2506f0ca4a391a319de8403734e4af8d678a6081fc`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 8.5 MB (8523001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27111cd5fb1057675f2e0b269790dc264d344d6e4b7ad92ff941f90a496167b`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 11.1 MB (11065924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1a5fd5565a96a28b5697fe91cee1bfa10686530f24736891bcc6aab90718b2ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64745350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320b1096c45b1588add1358fdcf606ea86168a27bfae2aea622165c45259f995`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:09:37 GMT
ADD file:084e44d77ffdb8aad1f856ec10db87922bdba3a90e06f9f1cafcb6e4284c8ff7 in / 
# Thu, 23 Mar 2023 01:09:37 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:37:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0b14dce67c2fdb37d2b0eacccff5119e226c45c2906f12d6ee93d8850400824b`  
		Last Modified: Thu, 23 Mar 2023 01:32:34 GMT  
		Size: 45.9 MB (45889194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395ab26b892c3659080680521b7e37b5cee24838f59696a77cfd944e93ccd158`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 8.2 MB (8168514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788f0ce3e6e5ae63843a828f2542045686f8131e60c22d54846351e88422de`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 10.7 MB (10687642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:03a892b4f8141b6f3f3c1d36591ec20f5abf8e7db913d6b06bef0195f59ada5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69649974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c5127fd80af5e1e2f2405e7610f8464a9e99f288f6b5e5afce4df2eb1aa624`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:27 GMT
ADD file:efed18ef2a003bff7e64e7049455216e51876402083581032c35085328e416f6 in / 
# Wed, 12 Apr 2023 00:39:28 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:04:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b0f987ce91d920ae0a705ed6c9824f1bbbfa282defb8986614030eb8e2bc0b4e`  
		Last Modified: Wed, 12 Apr 2023 00:41:45 GMT  
		Size: 49.3 MB (49345365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6a618ee06e99ebfbb7809c1cc4902cb717d294243f3765f170fd1c8eaf94a`  
		Last Modified: Wed, 12 Apr 2023 01:12:23 GMT  
		Size: 8.9 MB (8915044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c3f19470d2fd9e1407a7ddcbac3c316a999a143865347f221db18517e0838`  
		Last Modified: Wed, 12 Apr 2023 01:12:24 GMT  
		Size: 11.4 MB (11389565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b43a148c9da49809e8efcfafdef9c412da433e7735208795c69a14047f003874
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71409064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e15fc1cc8869eaa3b3492c5ebdad339d1c464b7630edf0a5e01a6fd94f6f3be`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:30 GMT
ADD file:7718865253a3489583d40f8c7a7beede0c20cebbab68bb3e97ad2e84082afcb7 in / 
# Wed, 12 Apr 2023 00:38:30 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:02:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a4ce9e81f634822e5166ef3eef875a4140795ac18afe0391433d72c7865bf67b`  
		Last Modified: Wed, 12 Apr 2023 00:41:43 GMT  
		Size: 50.3 MB (50317977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e54183fe5cb0866f886a93c0d098d38e649286a2b516b64d9658dd40f5d74b`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 9.3 MB (9264042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76896a8c48193a86329dc809066c177aedc76d55811eb32ca7c80c1ab06f66f1`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 11.8 MB (11827045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:cadf8f4e08099c01875c361dcd8fba3645b495aeecf0d53c2fd22a569372c184
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68885675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad6eff184509b73b66c889069c907dfd84004b8c2324f62ffbe80bc0453f87a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:15:54 GMT
ADD file:454bfcbdd9d738730885002e9124aea5e8eb4920ca5d3bf13bb9f4707023bd67 in / 
# Thu, 23 Mar 2023 05:15:59 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:03:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:70edc5cd98f5a2e589d309248c77122dabf95f437c0448b99513b15ef209f244`  
		Last Modified: Thu, 23 Mar 2023 05:23:55 GMT  
		Size: 49.3 MB (49291654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74250ff8fd2374ebbb2086f535377d5246a78ee51939da5984dc42e7afe6d2f5`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 8.4 MB (8439840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c3b2ae326a6eb2a81faaff9322b317ad4788f4c53f6c3b6721724ed9f3d04`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 11.2 MB (11154181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b2e26276ba83c4b68ff602aaa743294d6f71c408e0912d7dd1a787da5bffc9c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75120105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d6cc655a5db67e5cb97de4dfb139ff43049f64913c4d3b79788825fea30a1c9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:18:49 GMT
ADD file:5e17f6075630657b8465309f99ecbfc57e325d159b54f58181b974526f2314a5 in / 
# Thu, 23 Mar 2023 01:18:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:10:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:60e68956630003599038e3cfe86d6dd09ee874e8c30d9ea29b8350e0d3fa8497`  
		Last Modified: Thu, 23 Mar 2023 01:23:06 GMT  
		Size: 53.3 MB (53290316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcdbd51144dbb4a208e40072c2caf491305afb997e9161481db00137eefec5e`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 9.7 MB (9661293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bed649f1a85d37347952942e0ee256bdf515769a40a1c23cf02e65c6c90e6b1`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 12.2 MB (12168496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:377be7d5891b37466c736b399c0beb5ac9fdccf106bbee4e802cd0c0200a985e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67672334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75da5ea476406e76c74e365fa869cd83bc1a1cbbd23ef34d20b56b9cf7624b2c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:19 GMT
ADD file:5d2b35b45a0f23e2f2e93f9c311eb34a92e4591ea27979236d801e512d44cb85 in / 
# Tue, 11 Apr 2023 23:59:31 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:24:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8a09cd2374da8355612e7d4c91d55107a3f089816ae52b2c91b9e08e6a895ab1`  
		Last Modified: Wed, 12 Apr 2023 00:04:39 GMT  
		Size: 47.7 MB (47670407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d047361c12b2aeb253b1923b053dcc960101b3b3348af8f15f95f7fda2b89e4`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 8.7 MB (8713846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a462d218c24c21390b32ace449f4f47a57624b858dc05a37c31cb7f6e21c41`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 11.3 MB (11288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:5e0efa3054c24e10273c68601b3fccaaf0a0227b1fde44194bd37d41a14b472f
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
$ docker pull buildpack-deps@sha256:9ed3be818675099491b2a9c5066bbd63d5283caa5f3b77d978ea95ecb43f2d61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133896234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba56358263d5c537ab77ee622af1e53f4ab231c655f7637aa7739d9b469a80da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:35 GMT
ADD file:1cb6c660a2e3ea14b2a11bb8b80f53920c3da423a0ad7004391bfab4db4d0177 in / 
# Wed, 12 Apr 2023 00:19:36 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:48:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:49:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:49:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc556c281183180fae02d57fa6fb60ed0a99d9040936278743dc4022bfb0c686`  
		Last Modified: Wed, 12 Apr 2023 00:22:48 GMT  
		Size: 49.3 MB (49292938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8022b43d7c31d74c341d297cf10031ff0c51f596473a0c1945ee83a841094638`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 9.1 MB (9083160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db75f726ec67539c4823cb16851963ebe5838a853b0e769fd662020fad918781`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 11.4 MB (11422437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8a9e299258b84de99d6d739eb84b5b1632005f9c7723f2dd9e209fb1a8aaa3`  
		Last Modified: Wed, 12 Apr 2023 07:56:46 GMT  
		Size: 64.1 MB (64097699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:344b53de882fcda7c2d453195595144a3c69b6e842ee71d13d6da33ab28ecc50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129241091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5754c39ab542288953f32e05c79772f7f299ee5ef462be8bd98f34a5d5ae07f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:19 GMT
ADD file:df1103dce44baa95c92287ab5016f36d5cc45c6062116ebf5273f7e79a00915c in / 
# Wed, 12 Apr 2023 00:48:20 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:795c0ca2726dffdb0e5ef6ffa341d17ec672d5915011f1a93a05e8c95a4779ae`  
		Last Modified: Wed, 12 Apr 2023 00:50:12 GMT  
		Size: 48.1 MB (48110879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e70c1a23fdf0fd320a61a2506f0ca4a391a319de8403734e4af8d678a6081fc`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 8.5 MB (8523001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27111cd5fb1057675f2e0b269790dc264d344d6e4b7ad92ff941f90a496167b`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 11.1 MB (11065924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ed8d7f4b0f78246beda91a51ddbc4ab368fe6f04bb2432498c3f5a76cbc010`  
		Last Modified: Wed, 12 Apr 2023 01:20:30 GMT  
		Size: 61.5 MB (61541287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:83bc2ff04b8e6c4dccf1eeb1c113368f19ccdf7b850ad03505d94a5dbcb1ea9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123990303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd862b11f39b556183892c170beb4f43c718d63859ec32f1056de0082737529`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:09:37 GMT
ADD file:084e44d77ffdb8aad1f856ec10db87922bdba3a90e06f9f1cafcb6e4284c8ff7 in / 
# Thu, 23 Mar 2023 01:09:37 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:37:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b14dce67c2fdb37d2b0eacccff5119e226c45c2906f12d6ee93d8850400824b`  
		Last Modified: Thu, 23 Mar 2023 01:32:34 GMT  
		Size: 45.9 MB (45889194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395ab26b892c3659080680521b7e37b5cee24838f59696a77cfd944e93ccd158`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 8.2 MB (8168514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788f0ce3e6e5ae63843a828f2542045686f8131e60c22d54846351e88422de`  
		Last Modified: Thu, 23 Mar 2023 12:44:04 GMT  
		Size: 10.7 MB (10687642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9a3318c652dc50d1377b04d3c6d10a08df4155179df516ddbb594b1e7df246`  
		Last Modified: Thu, 23 Mar 2023 12:44:21 GMT  
		Size: 59.2 MB (59244953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:14fe92b486d2fa872ed5792948ef263bf382710d96156521bba91db6409d8adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133624598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13f0946fdc4f05c98259e0c4a796a7215b79fdfac56393722a52de699ef3ad2c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:27 GMT
ADD file:efed18ef2a003bff7e64e7049455216e51876402083581032c35085328e416f6 in / 
# Wed, 12 Apr 2023 00:39:28 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:04:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0f987ce91d920ae0a705ed6c9824f1bbbfa282defb8986614030eb8e2bc0b4e`  
		Last Modified: Wed, 12 Apr 2023 00:41:45 GMT  
		Size: 49.3 MB (49345365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6a618ee06e99ebfbb7809c1cc4902cb717d294243f3765f170fd1c8eaf94a`  
		Last Modified: Wed, 12 Apr 2023 01:12:23 GMT  
		Size: 8.9 MB (8915044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c3f19470d2fd9e1407a7ddcbac3c316a999a143865347f221db18517e0838`  
		Last Modified: Wed, 12 Apr 2023 01:12:24 GMT  
		Size: 11.4 MB (11389565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b373ae05bf678c385bace283c65197a2bbc2a334c528ed7b58a01d93131de585`  
		Last Modified: Wed, 12 Apr 2023 01:12:39 GMT  
		Size: 64.0 MB (63974624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1b7217dd58c62e94d4df1bd3fe5e75114d9fdb3da6a3d8338c1e2534008bffce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137369491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8865cd6ac62a089861253f45fe5c6131b992aa6d88dd85645089c3f5ada23`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:30 GMT
ADD file:7718865253a3489583d40f8c7a7beede0c20cebbab68bb3e97ad2e84082afcb7 in / 
# Wed, 12 Apr 2023 00:38:30 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:02:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:03:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4ce9e81f634822e5166ef3eef875a4140795ac18afe0391433d72c7865bf67b`  
		Last Modified: Wed, 12 Apr 2023 00:41:43 GMT  
		Size: 50.3 MB (50317977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e54183fe5cb0866f886a93c0d098d38e649286a2b516b64d9658dd40f5d74b`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 9.3 MB (9264042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76896a8c48193a86329dc809066c177aedc76d55811eb32ca7c80c1ab06f66f1`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 11.8 MB (11827045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba7e1ed0df9a2a8a6501d91360cea22ab988653bf057d73c44ecb41e49f6151`  
		Last Modified: Wed, 12 Apr 2023 01:13:56 GMT  
		Size: 66.0 MB (65960427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:febd8b1b579bb8f8c6e10e278729e85eedae1a13b46197fcaf699aee460de42a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131823277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f8ca8bc3fe142102f73eaa97cc8abc67f75fa29f8c4f921365762e6e5e75e17`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:15:54 GMT
ADD file:454bfcbdd9d738730885002e9124aea5e8eb4920ca5d3bf13bb9f4707023bd67 in / 
# Thu, 23 Mar 2023 05:15:59 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:03:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:05:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70edc5cd98f5a2e589d309248c77122dabf95f437c0448b99513b15ef209f244`  
		Last Modified: Thu, 23 Mar 2023 05:23:55 GMT  
		Size: 49.3 MB (49291654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74250ff8fd2374ebbb2086f535377d5246a78ee51939da5984dc42e7afe6d2f5`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 8.4 MB (8439840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c3b2ae326a6eb2a81faaff9322b317ad4788f4c53f6c3b6721724ed9f3d04`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 11.2 MB (11154181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce72fc6141c1bf4e5dcee62655f6469a6796ecc6186b5f6d227dd67b147c683`  
		Last Modified: Thu, 23 Mar 2023 07:31:48 GMT  
		Size: 62.9 MB (62937602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5be307306068d9b39637f16fe607ab070f354512a3b03fa1a34fa79afe382201
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144683760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503fa7c99f71ee01993b38f1cad0622c095add9381ddd3cdfa3854728a10d5e2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:18:49 GMT
ADD file:5e17f6075630657b8465309f99ecbfc57e325d159b54f58181b974526f2314a5 in / 
# Thu, 23 Mar 2023 01:18:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:10:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:11:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:60e68956630003599038e3cfe86d6dd09ee874e8c30d9ea29b8350e0d3fa8497`  
		Last Modified: Thu, 23 Mar 2023 01:23:06 GMT  
		Size: 53.3 MB (53290316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcdbd51144dbb4a208e40072c2caf491305afb997e9161481db00137eefec5e`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 9.7 MB (9661293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bed649f1a85d37347952942e0ee256bdf515769a40a1c23cf02e65c6c90e6b1`  
		Last Modified: Thu, 23 Mar 2023 13:23:20 GMT  
		Size: 12.2 MB (12168496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f138294734fe3a74e7b88ac5a9a4fe51653cff8b3ad0ba829039339f82a1a99`  
		Last Modified: Thu, 23 Mar 2023 13:23:46 GMT  
		Size: 69.6 MB (69563655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f1a6a91892b66c97ca28c0d4aa10b5706ce5d49d91fcfb33f33d04a191068ce7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130773785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1798d2a8c091800a97b7795b2e2f35680f165f0a95d7f44b12965f19623788f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:19 GMT
ADD file:5d2b35b45a0f23e2f2e93f9c311eb34a92e4591ea27979236d801e512d44cb85 in / 
# Tue, 11 Apr 2023 23:59:31 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:24:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:25:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a09cd2374da8355612e7d4c91d55107a3f089816ae52b2c91b9e08e6a895ab1`  
		Last Modified: Wed, 12 Apr 2023 00:04:39 GMT  
		Size: 47.7 MB (47670407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d047361c12b2aeb253b1923b053dcc960101b3b3348af8f15f95f7fda2b89e4`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 8.7 MB (8713846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a462d218c24c21390b32ace449f4f47a57624b858dc05a37c31cb7f6e21c41`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 11.3 MB (11288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628da1a495c0341f28b24cb228c4984d7d8a718059c95991d67739f4a4602e4b`  
		Last Modified: Wed, 12 Apr 2023 00:32:14 GMT  
		Size: 63.1 MB (63101451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:6fa31d2839b2176bb4d92e7cb1bf4f0acdac4ca440650d2d937bfd713779f3a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1cb95d972e0a2c28195432ae6f0b584389e01e1938354a98b61c2d0e4c79f44f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.0 MB (350981822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9133db89f5b5ae7caee0f8cca02226caaa3b22832a67d2a4bfc68f2ca38dfccf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:55 GMT
ADD file:0936f6fccda991ba27a7f73ca61c23a436b7ca417e504b66d5a68f2283e1e81d in / 
# Wed, 12 Apr 2023 00:20:55 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:54:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:54:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:55:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:003dca91ec623536e08abc4e1bb2849836a84c44f82e24b97fd5423162a4d46e`  
		Last Modified: Wed, 12 Apr 2023 00:25:13 GMT  
		Size: 49.3 MB (49287652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486f0b6179599c75a087e6850c42ef248d973e29a6898ed99c9bccdae08d2cd2`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 9.1 MB (9082764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f184ca8dda7ed83dd9d21d6c880d4e15976f35814156a0a67df81423067f4b8`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 11.4 MB (11422423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76159e5040abc54c8e269f5e87ba68551c98fa9a6a06c9d7af5eae5f9f3ee57b`  
		Last Modified: Wed, 12 Apr 2023 07:59:41 GMT  
		Size: 64.3 MB (64257071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108d0b8f8755100dc81501ff3e762f953171a4a1230223973781ad90f85c1a53`  
		Last Modified: Wed, 12 Apr 2023 08:00:14 GMT  
		Size: 216.9 MB (216931912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7c5689a7aafd87d157899f6caf4601d66e8e391aef6483970f37553b5a868314
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.5 MB (318503660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:321ba3c06205c499df306cc1b5cfded148321e0a03dea6b3028714995c1f7d03`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:48 GMT
ADD file:b02c911309a1b69d235b76dab369d523653c62374b0173ee9f1b65017607f9d6 in / 
# Wed, 12 Apr 2023 00:48:48 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:18:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:18:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:19:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8699c4859220eb7e4f2a5ae13e4dd5f9143cb7144e2a02a3eb381a79416524bf`  
		Last Modified: Wed, 12 Apr 2023 00:51:27 GMT  
		Size: 48.1 MB (48109671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b565bf44c40ab65f5193c4fbfd752809f50e95e2c4b2397728f42419979d7c`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 8.5 MB (8522810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8db076a21199a98e758a14876a91c9a890bb606e6d9d483862bcb73bc5cfbb`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 11.1 MB (11065853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466720607b58ed4036916fa9d7cb2e82a3ca95f0e5ec8e2ef908744cd3e409ec`  
		Last Modified: Wed, 12 Apr 2023 01:22:44 GMT  
		Size: 61.7 MB (61667229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df42d9b3dd685881fab45c09a19f6d1505f1612856e8b0acca62c90e5aa6457`  
		Last Modified: Wed, 12 Apr 2023 01:23:20 GMT  
		Size: 189.1 MB (189138097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:13bc1f7227e4eb190e2425e9ae9baaa9afa595247f7c48578dae477f5206c282
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.1 MB (299089852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82add4ff4f01d1f31c7d61d6b83e243c99fc38f0cb8fbe94fc118eaf5a75103`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:28:43 GMT
ADD file:628ac1300ca273dba23c7d617164bc6e664cdebb4106910020d7b3dcb39429c8 in / 
# Thu, 23 Mar 2023 01:28:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:42:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:42:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:42:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:43:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53d7f1f008e91cd29c47c933b404c16fc1d4cf64b8699ad1269e882f53ca6e2d`  
		Last Modified: Thu, 23 Mar 2023 01:34:10 GMT  
		Size: 45.9 MB (45911196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61016f9e9c2f44cda61da9f54267fbafe7fef3695caec3c87c6d5ae9eb452ae4`  
		Last Modified: Thu, 23 Mar 2023 12:46:05 GMT  
		Size: 8.2 MB (8168245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4226b16c6b7093dc765001b6e5615e8150c8d19be6c96ea1171e1ad13654f5`  
		Last Modified: Thu, 23 Mar 2023 12:46:04 GMT  
		Size: 10.7 MB (10704470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889e5e2259a7026a6a42309e4673ccd18c4288dce5b85e2039cb7238e36ce3fe`  
		Last Modified: Thu, 23 Mar 2023 12:46:22 GMT  
		Size: 59.4 MB (59373909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd2df18bf0523ee48067a579083ad967febe18f6eda98aa82f65c4fbb8ff974`  
		Last Modified: Thu, 23 Mar 2023 12:46:53 GMT  
		Size: 174.9 MB (174932032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ddc7753bdf44aa12263963bdb9942af3b69f4ed4dad7430d1a9eecabd6381d97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.1 MB (342096356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e722281a223374a931912368ece55c74201c7f46e39795b84006341333ddb0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:21 GMT
ADD file:2784bc6dba1e1dbea293e074ebf51fa7d89cb5545ea63ba2ed75b74d067387d4 in / 
# Wed, 12 Apr 2023 00:40:22 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:10:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:10:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:10:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43d214f7ab3ca35a0c9ed4d8cdf62b36248aba2fa1bbac4ecd64e82ba2520b70`  
		Last Modified: Wed, 12 Apr 2023 00:43:58 GMT  
		Size: 49.3 MB (49327656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d9e5d2b2df062d16ffea4a022a4c09ce904fb96ec3fa4712a1d936593ae2a`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 8.9 MB (8915031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd2b1a4cab3b4ac2bb4a7e9aaaa60ce806e3c49a8726f7baf5a10ba5e0e89fb`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 11.4 MB (11389544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff14914c0381e1889d1db49b1b39da80ae3a347cf1af048e2ae0eb42aec87a12`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 64.2 MB (64154048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f54a27824f720f86861a2776e1cc4e2f54563a9d0f0b56d1a6ec034866e3f8`  
		Last Modified: Wed, 12 Apr 2023 01:15:45 GMT  
		Size: 208.3 MB (208310077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:413efb8fbcbb35e21e9437afbee83ae1bdcf365d62cc1261952b77c46884fede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (352984444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09e361eb5030e9416d576bb6456af5b6f82090e0ffcde0ac62558e2c5fa198c1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:51 GMT
ADD file:31710a830769b5e1f2612e1cd05380f677714bf52f61a54adbc7424087fd1378 in / 
# Wed, 12 Apr 2023 00:39:52 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:11:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:13:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35e4af56b8bda58bf958814bc36c8e3a9a1d719c8582c0f33d7d69cc5b416211`  
		Last Modified: Wed, 12 Apr 2023 00:44:24 GMT  
		Size: 50.3 MB (50310899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145bb18c860aae65312434f79bce9d784a4824ef455202efca0f687a388037fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 9.3 MB (9263774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2063c41d1dff24f54b6a7d8edde21610fe37e02b35ed369be0ccf9f64cdc43fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 11.8 MB (11827096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3196dd70f259df7354dba37d732f79f68e602883ec8838b2cfcd0515de5c5c`  
		Last Modified: Wed, 12 Apr 2023 01:17:49 GMT  
		Size: 66.1 MB (66127351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc32f4359c6fe3187a1f8bab45e405139e65a8f45a4858a27e1059dd58842672`  
		Last Modified: Wed, 12 Apr 2023 01:18:36 GMT  
		Size: 215.5 MB (215455324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3862aaeea79e1c28e659f99f4d362b54d636ab87938c521b7e6c32cd660f4359
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.5 MB (321528438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d166a77be6f0012f9af9d61d3c7ad01ee0b80e1584627a75c08c07fee6b7e9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:18:32 GMT
ADD file:2d913f7b6c2e804834958b3d144bd7b5150a438e2aaa73cdf2f1be1c64d10100 in / 
# Thu, 23 Mar 2023 05:18:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:24:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:30:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c1a140184ad386a37a5446dba474a2a8498dff7ae8d2ccd2957aaf8dc1682e`  
		Last Modified: Thu, 23 Mar 2023 05:26:35 GMT  
		Size: 49.3 MB (49291603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaeb19ea7953e3c0a2cce0d76910d46a1fc5e289c90379ecb81b3e5ba2a0c16`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 8.4 MB (8439874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecc4eca24f781c1e786d1fc88cb24202f1248f85adc06cf1b375f5607ec2d93`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 11.2 MB (11170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3768b306fba92d6a836552b3ee3a1bb755cd0f7d6618ca028d0643fde06553`  
		Last Modified: Thu, 23 Mar 2023 07:37:53 GMT  
		Size: 63.1 MB (63099163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cde7245b1c56e104d5370eab7caa185d690ab7a9d05dd04502c112995eedf9c`  
		Last Modified: Thu, 23 Mar 2023 07:39:55 GMT  
		Size: 189.5 MB (189526884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1cd92695e70eee806ffc668ffc3613c1ae37e09e9905ff84a9ad42e7353a4a07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.8 MB (358843576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff6cf39c1a7a6027c3f5251567633ab1cfbf3af110fb104f2f31ece459b538e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:20:05 GMT
ADD file:3534cf3f10dae5b70c64865fd70cf5b9aa6ace6be9caa2d69518d6d59c4943fa in / 
# Thu, 23 Mar 2023 01:20:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:18:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:19:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:21:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8de2c12bac6cdfac096a845424e637222b157d221d8080dfc0e3cd14581716d5`  
		Last Modified: Thu, 23 Mar 2023 01:24:47 GMT  
		Size: 53.3 MB (53290173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ffcd14b130bc950e2e794bcf2e09ddffa8e18668803aa384fc8de743e9d8d2`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 9.7 MB (9661589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecca2a654e1b66be833e49110ac475ae4995f36d83ba12ad0396e8f4cf953872`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 12.2 MB (12185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5053cb00528479013fa5db3eb35bb36ff11628a7f8c9c6ae0310021f09a7005`  
		Last Modified: Thu, 23 Mar 2023 13:26:59 GMT  
		Size: 69.7 MB (69740333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb6e33785c280f1561e4dcdae27bfcb7e802b5b52d2ebf732730e9c11c4c717`  
		Last Modified: Thu, 23 Mar 2023 13:27:58 GMT  
		Size: 214.0 MB (213966262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:b9c02baf674d938d6af39d2f681786407b07e39dcc6c0ef663bbfa3027bb41f6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.0 MB (361040206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcff52053934b6b9001b1f614aafda9141bd8e31a4b2680e51f8d44353d4a4ed`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:05 GMT
ADD file:b8c0cf42f791d92283c2c47cf2ed446fb98a7cde685c9b923c89cadb86ddad31 in / 
# Wed, 12 Apr 2023 00:09:07 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:32:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:35:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:43:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6178d7c3b8603b1579d72ad9f5bda8fd22627feccccd498dad946eddfe96d27a`  
		Last Modified: Wed, 12 Apr 2023 00:12:25 GMT  
		Size: 45.5 MB (45494949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd056fe810f7c94134b5c26af6939949c18bfa4868dbc9f81ea8d7a25a0daf4c`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 8.1 MB (8117374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f8d5394c046224d62d5170fd151d4339e0f5131b1503bf3eafecefe1ec7a10`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 10.8 MB (10794055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0c6cc5fb9f28304c05335b3e21ed5e3cce359b94731f04cc903938689ebc19`  
		Last Modified: Wed, 12 Apr 2023 00:45:23 GMT  
		Size: 59.7 MB (59741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16f9d49dc3af209b4bcf7ce13172c2a5a76516c0d39580db79da7b27eaf387f`  
		Last Modified: Wed, 12 Apr 2023 00:50:51 GMT  
		Size: 236.9 MB (236892651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9287c8095d9220df2f988981ac641e97e22f861d9bd87aa2a19a9e6cf396a687
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.0 MB (319011191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:914264ef0379c6c6c2f67b9eb3fd0e99ffc0016a3f81cb006225180ad93d3a77`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:19 GMT
ADD file:0593fbca11f3d4a9b2b916ee99bb70651af04ea1275262f12e9b0e5c07e81f0e in / 
# Wed, 12 Apr 2023 00:01:29 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:28:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:28:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:29:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1844a6b5cc32e25703d3a6ac2115866157b1f856d7463d0dca8443fea51061f1`  
		Last Modified: Wed, 12 Apr 2023 00:05:31 GMT  
		Size: 47.7 MB (47665068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f306dc6c45f3e2637390b46a2dce7fb061bb8be6ae7c72c47bba97d84b99d256`  
		Last Modified: Wed, 12 Apr 2023 00:33:37 GMT  
		Size: 8.7 MB (8713548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676682574fe22f1cac8016a4f36ad54898c4313e0609a7e88e75e035e32444b`  
		Last Modified: Wed, 12 Apr 2023 00:33:36 GMT  
		Size: 11.3 MB (11288124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f9748f029581dd4821ad6e7d4da7ab4a31600128a2411dda2639c9b92fe58`  
		Last Modified: Wed, 12 Apr 2023 00:33:51 GMT  
		Size: 63.3 MB (63260422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81adcc7796eb9dd6b2ccee5b41b08f31d903a15caab787b2edc99367e1c15497`  
		Last Modified: Wed, 12 Apr 2023 00:34:19 GMT  
		Size: 188.1 MB (188084029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:f113f3ff3a042b006496b153fb9364e5d5aaab208637bec3fd6bf0ba65e447a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:162b0f4bf898e2f30f86c124dae307c51fcefaf8e30eba8f3d0538d5b88b1533
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69792839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895c4767319db895fdd9034df03472e20114f0f8c5ae8c9ce85f116db05635b8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:55 GMT
ADD file:0936f6fccda991ba27a7f73ca61c23a436b7ca417e504b66d5a68f2283e1e81d in / 
# Wed, 12 Apr 2023 00:20:55 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:54:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:54:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:003dca91ec623536e08abc4e1bb2849836a84c44f82e24b97fd5423162a4d46e`  
		Last Modified: Wed, 12 Apr 2023 00:25:13 GMT  
		Size: 49.3 MB (49287652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486f0b6179599c75a087e6850c42ef248d973e29a6898ed99c9bccdae08d2cd2`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 9.1 MB (9082764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f184ca8dda7ed83dd9d21d6c880d4e15976f35814156a0a67df81423067f4b8`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 11.4 MB (11422423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8b516bb4199218b93e0828691cca7924741a8012ef412cd89ec797180b9ad014
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67698334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9438faefdd9540401ef284f3ce81a1c9c2829d48e27358bfaecfb65aedfa6e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:48 GMT
ADD file:b02c911309a1b69d235b76dab369d523653c62374b0173ee9f1b65017607f9d6 in / 
# Wed, 12 Apr 2023 00:48:48 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:18:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8699c4859220eb7e4f2a5ae13e4dd5f9143cb7144e2a02a3eb381a79416524bf`  
		Last Modified: Wed, 12 Apr 2023 00:51:27 GMT  
		Size: 48.1 MB (48109671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b565bf44c40ab65f5193c4fbfd752809f50e95e2c4b2397728f42419979d7c`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 8.5 MB (8522810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8db076a21199a98e758a14876a91c9a890bb606e6d9d483862bcb73bc5cfbb`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 11.1 MB (11065853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f45638145f3049bdd8569f5e3e37f9012b169c009beecbf423abcfede1b90b6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64783911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfccb40ab0d880192527f3c9058b284e721f369d3a6a86d097ac545f40dc846c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:28:43 GMT
ADD file:628ac1300ca273dba23c7d617164bc6e664cdebb4106910020d7b3dcb39429c8 in / 
# Thu, 23 Mar 2023 01:28:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:42:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:42:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:53d7f1f008e91cd29c47c933b404c16fc1d4cf64b8699ad1269e882f53ca6e2d`  
		Last Modified: Thu, 23 Mar 2023 01:34:10 GMT  
		Size: 45.9 MB (45911196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61016f9e9c2f44cda61da9f54267fbafe7fef3695caec3c87c6d5ae9eb452ae4`  
		Last Modified: Thu, 23 Mar 2023 12:46:05 GMT  
		Size: 8.2 MB (8168245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4226b16c6b7093dc765001b6e5615e8150c8d19be6c96ea1171e1ad13654f5`  
		Last Modified: Thu, 23 Mar 2023 12:46:04 GMT  
		Size: 10.7 MB (10704470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c3e4535c3a32e860c9cdcb87e33d91d91a05de0caebac0e396b682b23449f890
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69632231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f59a19733f90d03e40a3a26aa25904ff3dd15a57aa3bc07c4723ab3a166147dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:21 GMT
ADD file:2784bc6dba1e1dbea293e074ebf51fa7d89cb5545ea63ba2ed75b74d067387d4 in / 
# Wed, 12 Apr 2023 00:40:22 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:10:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:10:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:43d214f7ab3ca35a0c9ed4d8cdf62b36248aba2fa1bbac4ecd64e82ba2520b70`  
		Last Modified: Wed, 12 Apr 2023 00:43:58 GMT  
		Size: 49.3 MB (49327656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d9e5d2b2df062d16ffea4a022a4c09ce904fb96ec3fa4712a1d936593ae2a`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 8.9 MB (8915031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd2b1a4cab3b4ac2bb4a7e9aaaa60ce806e3c49a8726f7baf5a10ba5e0e89fb`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 11.4 MB (11389544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7fd624c3066dfa1ca3da4f7665c730788104cdc2cb90f94fe839582a1a20bff9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71401769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10d2d9289ea8eef61411b36e3c5358bc3e57f93d19422a12cdce3b5d7d7e922d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:51 GMT
ADD file:31710a830769b5e1f2612e1cd05380f677714bf52f61a54adbc7424087fd1378 in / 
# Wed, 12 Apr 2023 00:39:52 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:35e4af56b8bda58bf958814bc36c8e3a9a1d719c8582c0f33d7d69cc5b416211`  
		Last Modified: Wed, 12 Apr 2023 00:44:24 GMT  
		Size: 50.3 MB (50310899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145bb18c860aae65312434f79bce9d784a4824ef455202efca0f687a388037fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 9.3 MB (9263774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2063c41d1dff24f54b6a7d8edde21610fe37e02b35ed369be0ccf9f64cdc43fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 11.8 MB (11827096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1cb13e8dab0a14d667e4d9b265c749ae59a611e6862763377f1c8e34e0112c01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68902391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54d7ab7b13f29c59bc95210628c83870c56bc3b074d787b15d305d64a13d17d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:18:32 GMT
ADD file:2d913f7b6c2e804834958b3d144bd7b5150a438e2aaa73cdf2f1be1c64d10100 in / 
# Thu, 23 Mar 2023 05:18:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:83c1a140184ad386a37a5446dba474a2a8498dff7ae8d2ccd2957aaf8dc1682e`  
		Last Modified: Thu, 23 Mar 2023 05:26:35 GMT  
		Size: 49.3 MB (49291603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaeb19ea7953e3c0a2cce0d76910d46a1fc5e289c90379ecb81b3e5ba2a0c16`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 8.4 MB (8439874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecc4eca24f781c1e786d1fc88cb24202f1248f85adc06cf1b375f5607ec2d93`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 11.2 MB (11170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:85bf0cae57000ef766ea7ed7d8f16d94925cfc5dfe0ffdef79a82c81cfdb0bd8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75136981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f95dec386d645db16ef52d1d12753c4acc5e8cd37261e08c733828e13efe122`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:20:05 GMT
ADD file:3534cf3f10dae5b70c64865fd70cf5b9aa6ace6be9caa2d69518d6d59c4943fa in / 
# Thu, 23 Mar 2023 01:20:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:18:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:19:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8de2c12bac6cdfac096a845424e637222b157d221d8080dfc0e3cd14581716d5`  
		Last Modified: Thu, 23 Mar 2023 01:24:47 GMT  
		Size: 53.3 MB (53290173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ffcd14b130bc950e2e794bcf2e09ddffa8e18668803aa384fc8de743e9d8d2`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 9.7 MB (9661589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecca2a654e1b66be833e49110ac475ae4995f36d83ba12ad0396e8f4cf953872`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 12.2 MB (12185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:b6ecdf5c65f021e05c80106a2cc8a598f2fb062039c62b358a2a42fc40f3d4d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64406378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc1ea8528f7edf3edcdff9fd62663fec45eaf492953562405ce7f8504695160`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:05 GMT
ADD file:b8c0cf42f791d92283c2c47cf2ed446fb98a7cde685c9b923c89cadb86ddad31 in / 
# Wed, 12 Apr 2023 00:09:07 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:32:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6178d7c3b8603b1579d72ad9f5bda8fd22627feccccd498dad946eddfe96d27a`  
		Last Modified: Wed, 12 Apr 2023 00:12:25 GMT  
		Size: 45.5 MB (45494949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd056fe810f7c94134b5c26af6939949c18bfa4868dbc9f81ea8d7a25a0daf4c`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 8.1 MB (8117374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f8d5394c046224d62d5170fd151d4339e0f5131b1503bf3eafecefe1ec7a10`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 10.8 MB (10794055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2a32ff0d5208b6ad040a9cb58b776824b3c95030e002745b9128549a0e88a98e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67666740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d98184dbb030d39270ec3b57dcd40af7dc1cb4c8755f6afe805779ab651c12`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:19 GMT
ADD file:0593fbca11f3d4a9b2b916ee99bb70651af04ea1275262f12e9b0e5c07e81f0e in / 
# Wed, 12 Apr 2023 00:01:29 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:28:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1844a6b5cc32e25703d3a6ac2115866157b1f856d7463d0dca8443fea51061f1`  
		Last Modified: Wed, 12 Apr 2023 00:05:31 GMT  
		Size: 47.7 MB (47665068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f306dc6c45f3e2637390b46a2dce7fb061bb8be6ae7c72c47bba97d84b99d256`  
		Last Modified: Wed, 12 Apr 2023 00:33:37 GMT  
		Size: 8.7 MB (8713548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676682574fe22f1cac8016a4f36ad54898c4313e0609a7e88e75e035e32444b`  
		Last Modified: Wed, 12 Apr 2023 00:33:36 GMT  
		Size: 11.3 MB (11288124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:b1ae960627b5c823f2a9f1b9a5985b38e09b4277cda102446472f1ddf77ccde3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d9f6278d7e0c871b5bcdc327298a29c7c00a8a0504891c4ad2631c374b75a01c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134049910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd617366d1cce33570b6dcf04f7eac2404f89e0bece798cb7e973cbd704f667`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:55 GMT
ADD file:0936f6fccda991ba27a7f73ca61c23a436b7ca417e504b66d5a68f2283e1e81d in / 
# Wed, 12 Apr 2023 00:20:55 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:54:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:54:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:003dca91ec623536e08abc4e1bb2849836a84c44f82e24b97fd5423162a4d46e`  
		Last Modified: Wed, 12 Apr 2023 00:25:13 GMT  
		Size: 49.3 MB (49287652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486f0b6179599c75a087e6850c42ef248d973e29a6898ed99c9bccdae08d2cd2`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 9.1 MB (9082764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f184ca8dda7ed83dd9d21d6c880d4e15976f35814156a0a67df81423067f4b8`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 11.4 MB (11422423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76159e5040abc54c8e269f5e87ba68551c98fa9a6a06c9d7af5eae5f9f3ee57b`  
		Last Modified: Wed, 12 Apr 2023 07:59:41 GMT  
		Size: 64.3 MB (64257071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c0b4a3eae58bd274c266cb60478e79df6446cb058ebcb7beec816064f9c69b75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129365563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b15a5f5bf525f6d5ed1af6bc9d3b44768864d1199c3f26e961d670e918851d7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:48 GMT
ADD file:b02c911309a1b69d235b76dab369d523653c62374b0173ee9f1b65017607f9d6 in / 
# Wed, 12 Apr 2023 00:48:48 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:18:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:18:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8699c4859220eb7e4f2a5ae13e4dd5f9143cb7144e2a02a3eb381a79416524bf`  
		Last Modified: Wed, 12 Apr 2023 00:51:27 GMT  
		Size: 48.1 MB (48109671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b565bf44c40ab65f5193c4fbfd752809f50e95e2c4b2397728f42419979d7c`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 8.5 MB (8522810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8db076a21199a98e758a14876a91c9a890bb606e6d9d483862bcb73bc5cfbb`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 11.1 MB (11065853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466720607b58ed4036916fa9d7cb2e82a3ca95f0e5ec8e2ef908744cd3e409ec`  
		Last Modified: Wed, 12 Apr 2023 01:22:44 GMT  
		Size: 61.7 MB (61667229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1bcd239105aa63dc35ccb13a3762579403f20339f19a8b5e4e3fa462e8efc5c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124157820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f8c81ddf581c824df2e636b5d3c3658ea69e1ee1d68768b20b0c899586cd2f8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:28:43 GMT
ADD file:628ac1300ca273dba23c7d617164bc6e664cdebb4106910020d7b3dcb39429c8 in / 
# Thu, 23 Mar 2023 01:28:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:42:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:42:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 12:42:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53d7f1f008e91cd29c47c933b404c16fc1d4cf64b8699ad1269e882f53ca6e2d`  
		Last Modified: Thu, 23 Mar 2023 01:34:10 GMT  
		Size: 45.9 MB (45911196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61016f9e9c2f44cda61da9f54267fbafe7fef3695caec3c87c6d5ae9eb452ae4`  
		Last Modified: Thu, 23 Mar 2023 12:46:05 GMT  
		Size: 8.2 MB (8168245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4226b16c6b7093dc765001b6e5615e8150c8d19be6c96ea1171e1ad13654f5`  
		Last Modified: Thu, 23 Mar 2023 12:46:04 GMT  
		Size: 10.7 MB (10704470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889e5e2259a7026a6a42309e4673ccd18c4288dce5b85e2039cb7238e36ce3fe`  
		Last Modified: Thu, 23 Mar 2023 12:46:22 GMT  
		Size: 59.4 MB (59373909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:909145f5f8b9a67acd7be2b62e379fe6c15950dee01727de50e4cc961c962502
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133786279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c7d9c27ae042d56e7ca69c21a7a5a690294d166c8196d78574264d9160d8957`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:21 GMT
ADD file:2784bc6dba1e1dbea293e074ebf51fa7d89cb5545ea63ba2ed75b74d067387d4 in / 
# Wed, 12 Apr 2023 00:40:22 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:10:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:10:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:10:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43d214f7ab3ca35a0c9ed4d8cdf62b36248aba2fa1bbac4ecd64e82ba2520b70`  
		Last Modified: Wed, 12 Apr 2023 00:43:58 GMT  
		Size: 49.3 MB (49327656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d9e5d2b2df062d16ffea4a022a4c09ce904fb96ec3fa4712a1d936593ae2a`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 8.9 MB (8915031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd2b1a4cab3b4ac2bb4a7e9aaaa60ce806e3c49a8726f7baf5a10ba5e0e89fb`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 11.4 MB (11389544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff14914c0381e1889d1db49b1b39da80ae3a347cf1af048e2ae0eb42aec87a12`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 64.2 MB (64154048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8e5134589fb0e6d388a1a4741142104956636747431cf809398cd58520b6da78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137529120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acc693ca7c37b5ced8d79a021265f81c4cecbc277909bb33bb103fd1302a0b37`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:51 GMT
ADD file:31710a830769b5e1f2612e1cd05380f677714bf52f61a54adbc7424087fd1378 in / 
# Wed, 12 Apr 2023 00:39:52 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:11:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35e4af56b8bda58bf958814bc36c8e3a9a1d719c8582c0f33d7d69cc5b416211`  
		Last Modified: Wed, 12 Apr 2023 00:44:24 GMT  
		Size: 50.3 MB (50310899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145bb18c860aae65312434f79bce9d784a4824ef455202efca0f687a388037fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 9.3 MB (9263774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2063c41d1dff24f54b6a7d8edde21610fe37e02b35ed369be0ccf9f64cdc43fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 11.8 MB (11827096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3196dd70f259df7354dba37d732f79f68e602883ec8838b2cfcd0515de5c5c`  
		Last Modified: Wed, 12 Apr 2023 01:17:49 GMT  
		Size: 66.1 MB (66127351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1fe2cb894be2bc55a95b04e66763ccec91305b7c7ac438bca7d21d751c7809b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (132001554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e553975cc4545e2dfa4c801fc4f1bfe90378add106afcf9e70883c34024f725c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:18:32 GMT
ADD file:2d913f7b6c2e804834958b3d144bd7b5150a438e2aaa73cdf2f1be1c64d10100 in / 
# Thu, 23 Mar 2023 05:18:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:24:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c1a140184ad386a37a5446dba474a2a8498dff7ae8d2ccd2957aaf8dc1682e`  
		Last Modified: Thu, 23 Mar 2023 05:26:35 GMT  
		Size: 49.3 MB (49291603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaeb19ea7953e3c0a2cce0d76910d46a1fc5e289c90379ecb81b3e5ba2a0c16`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 8.4 MB (8439874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecc4eca24f781c1e786d1fc88cb24202f1248f85adc06cf1b375f5607ec2d93`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 11.2 MB (11170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3768b306fba92d6a836552b3ee3a1bb755cd0f7d6618ca028d0643fde06553`  
		Last Modified: Thu, 23 Mar 2023 07:37:53 GMT  
		Size: 63.1 MB (63099163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cb552cfa8fffc38c06c010861606d8318ff8a2aafec75e73f34a9cf665dfbcc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144877314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5972c8f16c43d5fbd1f3bb72c145ccaef4bbf62a487929661df73dadb607568`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:20:05 GMT
ADD file:3534cf3f10dae5b70c64865fd70cf5b9aa6ace6be9caa2d69518d6d59c4943fa in / 
# Thu, 23 Mar 2023 01:20:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:18:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:19:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8de2c12bac6cdfac096a845424e637222b157d221d8080dfc0e3cd14581716d5`  
		Last Modified: Thu, 23 Mar 2023 01:24:47 GMT  
		Size: 53.3 MB (53290173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ffcd14b130bc950e2e794bcf2e09ddffa8e18668803aa384fc8de743e9d8d2`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 9.7 MB (9661589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecca2a654e1b66be833e49110ac475ae4995f36d83ba12ad0396e8f4cf953872`  
		Last Modified: Thu, 23 Mar 2023 13:26:33 GMT  
		Size: 12.2 MB (12185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5053cb00528479013fa5db3eb35bb36ff11628a7f8c9c6ae0310021f09a7005`  
		Last Modified: Thu, 23 Mar 2023 13:26:59 GMT  
		Size: 69.7 MB (69740333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:bcd300a4e07d706f2fd9f306c4c32864622137e94ae3c3c4670ea905ee0beff3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124147555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:397d717b57a8049a3da1ad949d9ed38c1e6d2518bf8f6c629c18545c03f04445`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:05 GMT
ADD file:b8c0cf42f791d92283c2c47cf2ed446fb98a7cde685c9b923c89cadb86ddad31 in / 
# Wed, 12 Apr 2023 00:09:07 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:32:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:35:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6178d7c3b8603b1579d72ad9f5bda8fd22627feccccd498dad946eddfe96d27a`  
		Last Modified: Wed, 12 Apr 2023 00:12:25 GMT  
		Size: 45.5 MB (45494949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd056fe810f7c94134b5c26af6939949c18bfa4868dbc9f81ea8d7a25a0daf4c`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 8.1 MB (8117374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f8d5394c046224d62d5170fd151d4339e0f5131b1503bf3eafecefe1ec7a10`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 10.8 MB (10794055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0c6cc5fb9f28304c05335b3e21ed5e3cce359b94731f04cc903938689ebc19`  
		Last Modified: Wed, 12 Apr 2023 00:45:23 GMT  
		Size: 59.7 MB (59741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ab7bb732a3d488865f2b887c55fbefc2e0041d528429e377f1f5ee84b43bda25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130927162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dba9e0d63f399d18f4d3f0cd3f58b4eee0e1d16c71d855c9f9b0bd4e250d67b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:19 GMT
ADD file:0593fbca11f3d4a9b2b916ee99bb70651af04ea1275262f12e9b0e5c07e81f0e in / 
# Wed, 12 Apr 2023 00:01:29 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:28:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:28:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1844a6b5cc32e25703d3a6ac2115866157b1f856d7463d0dca8443fea51061f1`  
		Last Modified: Wed, 12 Apr 2023 00:05:31 GMT  
		Size: 47.7 MB (47665068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f306dc6c45f3e2637390b46a2dce7fb061bb8be6ae7c72c47bba97d84b99d256`  
		Last Modified: Wed, 12 Apr 2023 00:33:37 GMT  
		Size: 8.7 MB (8713548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676682574fe22f1cac8016a4f36ad54898c4313e0609a7e88e75e035e32444b`  
		Last Modified: Wed, 12 Apr 2023 00:33:36 GMT  
		Size: 11.3 MB (11288124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f9748f029581dd4821ad6e7d4da7ab4a31600128a2411dda2639c9b92fe58`  
		Last Modified: Wed, 12 Apr 2023 00:33:51 GMT  
		Size: 63.3 MB (63260422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
