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
