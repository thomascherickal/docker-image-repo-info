## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:a5f3a4642a7bcb6745331f5a940933739ff186ea15b09cbaa1e275c12034508e
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
$ docker pull buildpack-deps@sha256:3c0807515e128baced0d30bb957832be1e298498ab4ae27e19a9790933a98442
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221261333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb3fc72df6ea346e4d81aac88ec7ea1d73ce5a1b4c228bd00daffd981222f849`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:02:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:06:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1404df7fbdef68bea55f7c051dbdb1aac1e564886ca277d1f8b1d0bf3fbe8e4`  
		Last Modified: Fri, 01 Oct 2021 03:17:56 GMT  
		Size: 6.6 MB (6643379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964552afca366bca79302ab79366a0528db0710e3db41a0a5c40e90d1b936c20`  
		Last Modified: Fri, 01 Oct 2021 03:17:55 GMT  
		Size: 3.0 MB (3022502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f547fe5b8db9e7e53004a6ebd2656feef7a91d529f9cb21c95b3bc8b108e19`  
		Last Modified: Fri, 01 Oct 2021 03:18:13 GMT  
		Size: 45.5 MB (45477448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d3bc1c26143d890a32399b1baeb259de8bf2f6b5f65036e6dbaca6547f8f`  
		Last Modified: Fri, 01 Oct 2021 03:18:43 GMT  
		Size: 139.4 MB (139412929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2a0a9aedb9391d38f4ff60c2ab26a5f465a326d22176710fc4e5ac81946a09fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189464780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b350369fb87f1ca87b97cdefe796eaffdef079642accdd4e21ca189c118148a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:11:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:11:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:12:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3861a2b4b4379b2bb53b663f814026fd5aa82ec17aba9f350a9597ab5273a6`  
		Last Modified: Tue, 31 Aug 2021 03:33:18 GMT  
		Size: 5.7 MB (5717193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb3fa3c4abd05090e6fe2924b1f9dace9c46f49394e0d3c3fb897ce110a718`  
		Last Modified: Tue, 31 Aug 2021 03:33:15 GMT  
		Size: 2.6 MB (2584566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b133473bb2c65d282eb3de44eb03d1d1132609ed4b032096b6e8d19c0ab159f`  
		Last Modified: Tue, 31 Aug 2021 03:33:59 GMT  
		Size: 40.7 MB (40671642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51d4df10b3dbd2670cfa2e40aa12cda1a31890469777cee489197ac586c3c29`  
		Last Modified: Tue, 31 Aug 2021 03:35:23 GMT  
		Size: 118.2 MB (118184900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bb8ee9051e7d4b54ae564f9b794edcb3d43512f0da2f32ffa6fff0b346fcc4ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205821969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b433afcd80444e75da56050c2f2fb8a3fcac5258832102e7dde4be0707285e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:15:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:15:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:16:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ae8f73d2b97ae6f304518bd244cd1e218386861b11878333a3e1704cd06fc4`  
		Last Modified: Fri, 01 Oct 2021 03:24:20 GMT  
		Size: 6.1 MB (6085031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc43f166dad077ef896c5d7e305f3a19ff7f4c0245159dede3adee91cf2fb17`  
		Last Modified: Fri, 01 Oct 2021 03:24:19 GMT  
		Size: 2.8 MB (2783140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a133bda1a844b0b9e9ac0284af4779d5ec158f5693b56511a1f27a5cbc8f541`  
		Last Modified: Fri, 01 Oct 2021 03:24:38 GMT  
		Size: 43.3 MB (43269968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba35ad1221e5859d39cb2b5e83e0f09f32a679b01ad0cf9bd7d43f755fce8ca`  
		Last Modified: Fri, 01 Oct 2021 03:25:08 GMT  
		Size: 130.0 MB (129956354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9f10a9ee18f6be60bfe5500c424c0125ad8e8b34ef076b08278d9a12cf826537
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.6 MB (218560267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419b39771048169c84a707f522a0987ffe42bf3349a0ab49e3abac9277252716`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:14:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 04:15:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:18:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89515178f4a354382498077df201d0c7296621351f651bf1d7bda94f1d499466`  
		Last Modified: Fri, 01 Oct 2021 04:21:07 GMT  
		Size: 6.9 MB (6932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99224216777e769a2c151c0c091ec4cda2a5d5f541c203e203683c71b6cb4a9f`  
		Last Modified: Fri, 01 Oct 2021 04:21:06 GMT  
		Size: 3.3 MB (3252987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8565053f61bc235064ba9f6560e2464bd101da6ba901ae2152a5198bac7f4e3`  
		Last Modified: Fri, 01 Oct 2021 04:21:29 GMT  
		Size: 47.1 MB (47065713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0502655b09b53ef4e834ca20300b20d019082bfbe8caad5e33e24676ce7aa8`  
		Last Modified: Fri, 01 Oct 2021 04:22:13 GMT  
		Size: 134.2 MB (134150425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:be35398927073fda01415ea00d7b65e109547bfb420e6ee2fe10eaea460312f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246214005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc7badbbabd3507ddd585d388bf12121101dc802cc082d1f326ffa3fd83edb8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:24:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:24:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:27:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:37:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164a2b27f3d3e3338d0cad4aa8917def23b4e4125d8bd35fd92d28d391bd7193`  
		Last Modified: Tue, 31 Aug 2021 05:04:40 GMT  
		Size: 7.1 MB (7059170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c419c8f7c4b804d1eb861ec26eda86aed2a9e66ffe649c93fe1a1729410d58`  
		Last Modified: Tue, 31 Aug 2021 05:04:32 GMT  
		Size: 3.7 MB (3719596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938b10a4ce464230361253a72401f6202439a4d63ec35d261d6ff9149f4649bf`  
		Last Modified: Tue, 31 Aug 2021 05:06:57 GMT  
		Size: 53.7 MB (53715779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d558be345f86c0280cd8bdfeb4b49282bb6a8c0db05c4992c7dc33a0d667803`  
		Last Modified: Tue, 31 Aug 2021 05:11:31 GMT  
		Size: 151.3 MB (151281702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5936655630734b659a06da22719a5788844863d57670778cb9d6bc1f79007ddb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.6 MB (205618219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ec7d1aadb3df4675c40b4a20c77c55defab1ae414d0cc9570efce58c897ac6a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:33:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:33:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:33:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:34:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f1e9a656ce747f09402ff405b881ebbce2041d0228e2373aac2dbfe9a23fd8`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 6.3 MB (6334289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe96b416a4fa4b5de3ab17b5e2b2b85bde2482559e7592284278d282da0c067`  
		Last Modified: Fri, 01 Oct 2021 02:41:21 GMT  
		Size: 3.0 MB (2974970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6a10244fc86eb56eba2d1e8554fe9b23b582e56b7728fcb21fee59a9313d52`  
		Last Modified: Fri, 01 Oct 2021 02:41:34 GMT  
		Size: 45.0 MB (45016989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8108fe4f05569dd68d228c1be27552ed405fc79994a5cb6f78b8c142ff1ed6da`  
		Last Modified: Fri, 01 Oct 2021 02:41:57 GMT  
		Size: 125.9 MB (125929053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
