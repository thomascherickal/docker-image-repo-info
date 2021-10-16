## `buildpack-deps:impish`

```console
$ docker pull buildpack-deps@sha256:9ff9def4dab166bfffe6c8270b3e6d84bdf7c57a0bd0824683d2ec0b46ea1eb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4a714ef064211342ecb2b7c0d3f842fde01ce29545314ac8b7855739d233a20c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.7 MB (406696151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c02f6289dca6ecbd27c029252f3b42c320ed52aea0148373aa8419ab493a958`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:58 GMT
ADD file:41d75787395224d025bcc0f7feca7c56fd4c1adea7cce667e2472fad282054fc in / 
# Sat, 16 Oct 2021 00:37:59 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:48:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:49:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:52:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3910f09893e52b84e55ef361892610a5a78e9df154e23da9bd7e317a4f3518d5`  
		Last Modified: Sat, 16 Oct 2021 00:38:57 GMT  
		Size: 30.4 MB (30391190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344f3e1ad647088394470484ad047b920daf1cfde567fb1b99b7526177300185`  
		Last Modified: Sat, 16 Oct 2021 01:55:21 GMT  
		Size: 3.7 MB (3697350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e70db9e5b826e9fac9ce0f806fa2b5875a56ccc8ea33a2e7eeafab2210f485`  
		Last Modified: Sat, 16 Oct 2021 01:55:21 GMT  
		Size: 3.6 MB (3551747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937a666ce0307a7646dc581c64fdaca960f0cff83dc954c43ba2c4fc7500eec4`  
		Last Modified: Sat, 16 Oct 2021 01:55:37 GMT  
		Size: 38.1 MB (38080022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0c62b19511dd9a0074eb6d6eae137e7a9487dff6812c464d5d77b3308b8cdd`  
		Last Modified: Sat, 16 Oct 2021 01:56:28 GMT  
		Size: 331.0 MB (330975842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f6678c935da21dcc51c2272f514ae95e68946b6e94206470cfa7e0d3c84f3f33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.1 MB (371066555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f07948a9b90cd3d03abd58a6ebacbaa26c4f20e9a3ce2cd987bd465f4ed3965`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:27:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:28:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:30:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf1a9d4fbdb8bcdea8da245690e0e7b0d7f42cd7b7480dd3f9866881a1da2c`  
		Last Modified: Sat, 02 Oct 2021 22:43:19 GMT  
		Size: 3.4 MB (3448048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfa76bdfd39c414c299c1e02cf75c9b579b3aa69ca8e1abf9eb876765fcc9ab`  
		Last Modified: Sat, 02 Oct 2021 22:43:18 GMT  
		Size: 3.7 MB (3742516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360154fa07ad953713f7e71f7feffabf9f868fa69562aeb598e60ebd881ede16`  
		Last Modified: Sat, 02 Oct 2021 22:43:59 GMT  
		Size: 40.3 MB (40285193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb0c2a0ca1287f5644704ab6ae1dbfd650eeae5b8ce48ee335e46a1a2bd068`  
		Last Modified: Sat, 02 Oct 2021 22:46:58 GMT  
		Size: 296.7 MB (296673806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:173282a68ed3c7d434e0a049630d7ee47e5ff9b0937c87e24de80c41032b44f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.8 MB (399753642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c681f790e2c9ad75fe348a46f94492c9e4e2a4cf1c6e08b36b18048884d41020`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:20:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:20:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:21:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e1bb6cc21d9aa99ea2365d91ca737ff33423cf8eef3ac6d444f9264ecf62c`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.7 MB (3680866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44384e90f77381715996a06f1aef553b1ffe6e32cd9f467350b914746ba678eb`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.5 MB (3533741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc1cb90f475d191407aa41ee7d90ffd845371c604e65fedf778556ba48612f`  
		Last Modified: Fri, 01 Oct 2021 03:27:51 GMT  
		Size: 38.0 MB (38028253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fd4f9a27c5ce4d91f6bfc6770ad8a8b894911d0d94e7e683e9c34844be1c22`  
		Last Modified: Fri, 01 Oct 2021 03:28:51 GMT  
		Size: 325.5 MB (325462804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d8fd1b555823e2eadce71afdfb43b7af92657b0d2af4bea0909c0089b9a49d8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.3 MB (414285096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d50be5ea3b04e32763f9ff630d4dffdefa8edd27b6ffd6f3f26f4863dde311`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:08 GMT
ADD file:2882612be3480d0a26c565cfff723f6f7c913ecc1e3b982def388f5c29ad10e6 in / 
# Sat, 16 Oct 2021 00:37:12 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:18:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:19:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:20:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:26:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cfd5cbebb9f6bac4f6c4e8b0ed1450129f245085d7131094975207c3091fb66`  
		Last Modified: Sat, 16 Oct 2021 00:39:02 GMT  
		Size: 36.2 MB (36177739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5e42bcc4ae69e168604f5e12739b0b1eb5c7801c5bbba53b80248a3522d3b2`  
		Last Modified: Sat, 16 Oct 2021 01:31:20 GMT  
		Size: 4.1 MB (4149852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbf4430060475cdfccdf811046cc128f1e962010f7015eb473cd56a44a181a8`  
		Last Modified: Sat, 16 Oct 2021 01:31:20 GMT  
		Size: 4.2 MB (4241545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb8938471f6dddbd4f944bff6ddb03f309c6bcae0ae55bb812677543460af16`  
		Last Modified: Sat, 16 Oct 2021 01:31:39 GMT  
		Size: 42.7 MB (42707246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1c0b96742c2d6080e849496d6ddf7e2b24df3e3f80c814bf8b05b6ad73d4fc`  
		Last Modified: Sat, 16 Oct 2021 01:32:45 GMT  
		Size: 327.0 MB (327008714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:d057cfbb20718beaf889f2d3f424053e69ca9a34f66d17986e2a5b084f4ef940
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266333139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef7a6fb984d6ea8571ca1e96c2b1829df424f5ae30cb6889b5ce991dec009db`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:17:48 GMT
ADD file:8cf59b4b38ccab14d48f2740546784966d4b20690dc57f9018241a62adac259e in / 
# Sat, 16 Oct 2021 00:17:50 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:02:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:03:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:06:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:12:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:19a9653dc9c1bf288e8c03d2027a0edd6609e7bc4c852b05e2ba35e947868701`  
		Last Modified: Sat, 16 Oct 2021 00:31:12 GMT  
		Size: 27.2 MB (27208455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e415d53d305cea0edcb8861ea11f8c974a195af5e0bbab60d58e5e787c69b09`  
		Last Modified: Sat, 16 Oct 2021 01:31:29 GMT  
		Size: 3.5 MB (3494237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c502225d86b92683284985a96ecaca6eec34631b1832346308e6c7a4edb2378e`  
		Last Modified: Sat, 16 Oct 2021 01:31:28 GMT  
		Size: 3.8 MB (3803241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cecdd79d1cc72b4c2d810dc407d5914a021c62c026514835acc2f18ecd221e5`  
		Last Modified: Sat, 16 Oct 2021 01:33:24 GMT  
		Size: 40.8 MB (40762991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e03719fabfbd1fdcdd0925fd8aa8947f5d943b1410c59b9ba5ea8a05a6ef24c`  
		Last Modified: Sat, 16 Oct 2021 01:39:34 GMT  
		Size: 191.1 MB (191064215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:289c4e33490a29a0c4d1e91ff90ba687e49e4d9bfce3cffb5ac1bbcbf8eb91af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.9 MB (367897006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e42552a4cc5f56b542c98c8f021e4f0397b5897c83e276e4edaa0e79d5471db`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:42:02 GMT
ADD file:e3ac42c4b4650e7d57adf242fb9b7137898397121142c4fd47afb661024e0b00 in / 
# Sat, 16 Oct 2021 00:42:03 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:11:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:11:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:12:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7101024e2e65688584ff7a7aa5f503fe9e8165ebcc5fb924b1304bbdd0d4256e`  
		Last Modified: Sat, 16 Oct 2021 00:43:14 GMT  
		Size: 30.5 MB (30527974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c893f3d07db208a09670ca2a61f5af4e83488249bea3ec02f9de57eb0e6c1f`  
		Last Modified: Sat, 16 Oct 2021 01:15:57 GMT  
		Size: 3.8 MB (3771530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3328cbd7261ef1a0a50687cdd7d7c486ab672569fbd2f169f94fdb4d20618a`  
		Last Modified: Sat, 16 Oct 2021 01:15:57 GMT  
		Size: 4.0 MB (3962629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba43f37a0fd565fd1fbb24c6e2586d0d7a7bad8eda0d92d2407d12fa7ee680a`  
		Last Modified: Sat, 16 Oct 2021 01:16:10 GMT  
		Size: 38.3 MB (38324342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d6471533ad95df35c90efa28ac34a550430001d0c9a7c71ffb036ea4bfa034`  
		Last Modified: Sat, 16 Oct 2021 01:16:49 GMT  
		Size: 291.3 MB (291310531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
