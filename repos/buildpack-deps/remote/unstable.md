## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:233d45c7498fed302d5bba195b5e6831e019f87b44af16cbce869219c1610803
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull buildpack-deps@sha256:2eb2bab3e32bb6deafa893d5954b99f7f65804b142fe45f4a36210f6c9208c94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321918912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ac348d6fb0595a4c5a3e16c00b64aca01ff3772f8c3f9b5d1ba3b73abdb48f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:22:23 GMT
ADD file:66b4753e4d225919cb5470c007009d4dbea725cab1d3ad1cd3c0ac3b35192aa5 in / 
# Tue, 09 Feb 2021 02:22:23 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:37:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:37:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:39:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9e6a013db8a50441790405f039006e736170b55104d06c80015cacba6d5b0f4`  
		Last Modified: Tue, 09 Feb 2021 02:28:28 GMT  
		Size: 54.8 MB (54793268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082f6b01c7a4634e4f6d0de548009681557bbaedac26abf3e20b536a7b5e5923`  
		Last Modified: Tue, 09 Feb 2021 04:47:21 GMT  
		Size: 5.1 MB (5144121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4f1dd261e5a91095fe68ed97b0d837c7dd575a8940fc745f7be6b907a906dd`  
		Last Modified: Tue, 09 Feb 2021 04:47:22 GMT  
		Size: 11.5 MB (11526140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd0a197c751f04bd540044db906f495e302beececb29f7508ec957c91579227`  
		Last Modified: Tue, 09 Feb 2021 04:47:39 GMT  
		Size: 54.2 MB (54164369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e7ee8cf9fae0d5dbed45a53f0837548dda3b83a5cb222016c0eec0b60cf799`  
		Last Modified: Tue, 09 Feb 2021 04:48:21 GMT  
		Size: 196.3 MB (196291014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b326e3864329a97619f51d3ac94f82b8c1dad4eee989d716b64b5a0fad0c0fd3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.0 MB (295035951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8159f8cb691627f3510cd979f365376276ac7378db3b62c4296519c4082f6ef0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:53:02 GMT
ADD file:8a666bde5248b085708640c42b93c850be2265e6a4db5b59c48543ddc8ad0148 in / 
# Tue, 09 Feb 2021 02:53:03 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:29:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:30:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:33:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b915a09886212577bb3e4444d6bdc576b17746fa48c0239c56c968d81127e7e`  
		Last Modified: Tue, 09 Feb 2021 03:01:34 GMT  
		Size: 52.3 MB (52324134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c594f7d69077392315310232b92354eaa9652361ef5e54825e4aade3a67e2851`  
		Last Modified: Tue, 09 Feb 2021 03:41:51 GMT  
		Size: 5.1 MB (5053985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195684c55108e3d23d6b03082fa8140c8859a738918fed4410211cbac9dd2ee6`  
		Last Modified: Tue, 09 Feb 2021 03:41:52 GMT  
		Size: 11.2 MB (11214925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4c9349b2c21a4df7a32b0def6cda8f6f44a4972a38016b41392e9a816ae16f`  
		Last Modified: Tue, 09 Feb 2021 03:42:16 GMT  
		Size: 51.9 MB (51916841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac5a4b1fa14ffa1118c684852826477563f26374829b473a6787fdf2a59fad8`  
		Last Modified: Tue, 09 Feb 2021 03:43:10 GMT  
		Size: 174.5 MB (174526066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:030518e554179d4e1c51c0bcef07b66cc63047ea5071a756485e7580afc1dac3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.4 MB (282449232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1d68d65f4c1c25eaa4479421d8c22ee8b43594be44220241ca677fd2cb6748`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 03:03:31 GMT
ADD file:37f3b4ac2683802bd4615102851fc9dcbc409a3964e047866697c24a568fc90f in / 
# Tue, 09 Feb 2021 03:03:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:29:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:29:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:30:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:31:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b8fd51bd157e6a71bf72bc04c009bb65c4766fc14c9fa5e95c0bf36f393f7ab4`  
		Last Modified: Tue, 09 Feb 2021 03:12:11 GMT  
		Size: 50.0 MB (49982731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d61fff78cf158b64e5f26e7f3c7e3d2e7eeb167059b0e914b1d2626b5c9f1e2`  
		Last Modified: Tue, 09 Feb 2021 04:41:09 GMT  
		Size: 4.9 MB (4914542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5d61b00c2332b32afcd6a8b313f6eee25aac2d20a654993899c9bad1c8191f`  
		Last Modified: Tue, 09 Feb 2021 04:41:10 GMT  
		Size: 10.8 MB (10835940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033fa227e4af9dd28e4a17a31e9b4f944cdad2c7b21ccd6cb0d2cf03326f7f51`  
		Last Modified: Tue, 09 Feb 2021 04:41:35 GMT  
		Size: 49.9 MB (49935532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4df489f496e108be42b6ff8806739598054f4983d1ba115a0603e8fb1777f5`  
		Last Modified: Tue, 09 Feb 2021 04:42:27 GMT  
		Size: 166.8 MB (166780487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:eb82a81b0b11b9f95784cd8d0a366a2165bc36c7c463714b58c4d02e794ec5b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313619184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7efd7b54d5c7b6da3aff3802e25b399d9a6ed379b1cc7204854e6742419bc4e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:06 GMT
ADD file:988aaab917b0b86b69a5ec0bc1b562df25e15f11cbd3997c0eb79c065697d66b in / 
# Tue, 09 Feb 2021 02:42:10 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:46:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:47:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:47:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:49:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16d849c3d9b47a494d04ea09283a62946c42f5ebec529d6b0f5c094929bc8e48`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 53.5 MB (53467842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1a97402a658df9ec658bfe4c46ed0b39e10960a7656f1762b77630edbff325`  
		Last Modified: Tue, 09 Feb 2021 04:58:49 GMT  
		Size: 5.1 MB (5132244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d6b3647e20b39d65d6536d94dd338a68c8214241b59de7f6643aff0bd2a98e`  
		Last Modified: Tue, 09 Feb 2021 04:58:50 GMT  
		Size: 11.5 MB (11531779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f75f6d750154f0418976cd6a34689ec5a962d9938abeb8f4d05ba354a30d72`  
		Last Modified: Tue, 09 Feb 2021 04:59:13 GMT  
		Size: 54.3 MB (54279457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9e96330fa904c7e6f126864c75d918d788769e214a7eb6138b9dc4b3ed3623`  
		Last Modified: Tue, 09 Feb 2021 05:00:04 GMT  
		Size: 189.2 MB (189207862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:65d937b357533e7724c939967f09e82d73b46a0f4be66fb3f020c2157cb38ef4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.7 MB (327727704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bccc862964946b5959cf0eee78e1a8da97c2c377e06b2fdfbe92d8cb72977cc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:17 GMT
ADD file:d3470c47b61c2df201e9fe51e9dd198c152bae2eba84df9bbfcb591bfb29502a in / 
# Tue, 09 Feb 2021 02:41:18 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:12:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:12:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:13:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:14:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:14213d5e86eb4e1e7c43e3524429378786d8674960445945ce050c587b83884f`  
		Last Modified: Tue, 09 Feb 2021 02:48:13 GMT  
		Size: 55.8 MB (55792012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2cbabcd8ca39fd619ad8a109f0fe5eea442c6afefd108f3d2a80a49be04524`  
		Last Modified: Tue, 09 Feb 2021 03:22:39 GMT  
		Size: 5.3 MB (5271392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cacdc0d9d1ac9a69c2a336a43253fbfd3737321bf5e32c6f9ee54465cb2087`  
		Last Modified: Tue, 09 Feb 2021 03:22:40 GMT  
		Size: 11.9 MB (11932342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f68738ae071787fe3613a10b142f8364d3bb9250f4e045082d605a217ca3a1`  
		Last Modified: Tue, 09 Feb 2021 03:23:12 GMT  
		Size: 55.5 MB (55510870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94f8f0f0209d88af48a9eefc480e170087c7bcd7a514e5a48f5f2fd0634130`  
		Last Modified: Tue, 09 Feb 2021 03:24:37 GMT  
		Size: 199.2 MB (199221088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:fbdcec9f9052c434fdea22e2ecb82b6bef71098801f973468390e1c5bef7736c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.1 MB (300075892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f72301874d2ca47c1b77b3acca033d9e110f400a179f591d916e965147f65a1f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:52 GMT
ADD file:1bed7e8245b9fdc9b6216dfe7c7a97a236870647ca9e7641f98c8b2f5f165612 in / 
# Tue, 09 Feb 2021 03:09:53 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:09:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:09:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:10:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:12:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d37dfb54bbee12f1ddd54773820dc4abe1d8525601798200ea891af443d2dcdd`  
		Last Modified: Tue, 09 Feb 2021 03:16:42 GMT  
		Size: 53.0 MB (53038778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c585817c61fcb4aec261a19daa3690feb2d437834958b786381a615e14144fcd`  
		Last Modified: Tue, 09 Feb 2021 04:19:59 GMT  
		Size: 5.1 MB (5107065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340d3cf0ba9b4e31b7d87e5818d6489e6e7ad7ad78a8a6c448eb31c1288899fc`  
		Last Modified: Tue, 09 Feb 2021 04:20:02 GMT  
		Size: 10.7 MB (10652706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08842a18c95c3b172cd4cebae5320ad3d89b5857435661dd88a438a58c526106`  
		Last Modified: Tue, 09 Feb 2021 04:20:52 GMT  
		Size: 52.9 MB (52904169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3497cde79cfe7c7e4c2f81ccf9973b85908f3181b79b9553a9e58ad6c21ddd93`  
		Last Modified: Tue, 09 Feb 2021 04:23:00 GMT  
		Size: 178.4 MB (178373174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f1b7a7a30d8e8a4811aa8dca514bc0b441aee226158cd92a9328805d47f5893b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338472361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e36634baf7e275da80546e3bcde8cf98b9282fd9f8b3ec417cefff7d57c5ca9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:40 GMT
ADD file:f289d6dea557bc0563fd9221c4857a56c56bb52d981a3ec90ade2f1b76980794 in / 
# Tue, 12 Jan 2021 00:25:56 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:22:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 02:25:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:35:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:594e638823d3ce0bbedac4d1aebea00f91d28a98d7b98ca680fd90e4c0fc8850`  
		Last Modified: Tue, 12 Jan 2021 00:34:46 GMT  
		Size: 61.0 MB (61048727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a59148553af7496dfbc29a5704e94338ac15ab898a646dcbab32076a5f00f3`  
		Last Modified: Tue, 12 Jan 2021 02:40:41 GMT  
		Size: 5.4 MB (5400394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45a065f7b5587bec16714bce093a4075fb92b291238fee1bae7d383a16a4052`  
		Last Modified: Tue, 12 Jan 2021 02:40:42 GMT  
		Size: 11.4 MB (11422811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d08d3752bb8f3109a9dc34906d86a1d6f92b178e9b8153717c78ad56a98e568`  
		Last Modified: Tue, 12 Jan 2021 02:41:08 GMT  
		Size: 58.3 MB (58333533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d650daa9329014f04bd0efe42ae67b05ba9177040921ee9a637b9415f8bc44`  
		Last Modified: Tue, 12 Jan 2021 02:42:02 GMT  
		Size: 202.3 MB (202266896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e9bb23dd4b6434c08f5b32d4aea924887a101509c425f14ec47b2703f8d19b5b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296096847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d943de156aa71c7ec4df6ec4a6be9bd26496af6742e8e50c39287fc872d8ee0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:21 GMT
ADD file:6b632451421e7f0411db1927a48466a6b3bc2f7e10a53b00a06799fbec279bdd in / 
# Tue, 09 Feb 2021 02:42:24 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:07:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:07:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:07:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:08:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd2606d37926391a1e8153ffefee2aaccae04bd432c37c97187880ba3ed01ea`  
		Last Modified: Tue, 09 Feb 2021 02:45:45 GMT  
		Size: 53.1 MB (53060083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd34d7430306d4b5f56a7983d33fdce7c2f86209989ddeacc68e07134aef96e`  
		Last Modified: Tue, 09 Feb 2021 03:12:40 GMT  
		Size: 5.1 MB (5127742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b9a7cd753b983b2730894814680d1c0b77e08d7affc85900856bd036f96806`  
		Last Modified: Tue, 09 Feb 2021 03:12:41 GMT  
		Size: 11.4 MB (11412927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceafff3a3e377a78f87f033989c6a1e6a8359c5afc3075ebb1d31d46a46a2cb`  
		Last Modified: Tue, 09 Feb 2021 03:12:56 GMT  
		Size: 53.6 MB (53647058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6c69cefbf0e740400b18a407e7d0017b945a36c5aff89b14e1c09a11643b85`  
		Last Modified: Tue, 09 Feb 2021 03:13:23 GMT  
		Size: 172.8 MB (172849037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
