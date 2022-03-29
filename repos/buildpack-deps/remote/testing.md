## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:c78a0630463db6925d452bc45911e2eb04bcedf775394b967a5c8eddba239a99
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
$ docker pull buildpack-deps@sha256:ea308a00b1b14aeb3d6fbad5a23a2c3a6fe5734e00a3b74cccd6badff84ffe1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.0 MB (333014978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d4459214da150d35a084bc2957baeeb6cdf1acd266263f7576731c384c39f9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:21:48 GMT
ADD file:084dc3db6641669bf09de94b7a32f3180ca32152a22a677961428ad78324f10c in / 
# Tue, 29 Mar 2022 00:21:48 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:28:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:28:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:28:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6673186ed4ed62930866783fb71f9386d0ece250e264d269d06e238753c30392`  
		Last Modified: Tue, 29 Mar 2022 00:26:08 GMT  
		Size: 55.6 MB (55584323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df04644801f7943b709f58330bcc6bb7f022f170144d520e3ed86de27038730`  
		Last Modified: Tue, 29 Mar 2022 17:36:58 GMT  
		Size: 5.3 MB (5268987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faed9fc4a14be51a64a07e3c2c778a51e2c2d8fbf4f7f4e4502991884520e0a5`  
		Last Modified: Tue, 29 Mar 2022 17:36:58 GMT  
		Size: 10.9 MB (10923809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1774237b19b51c64e2dec4de20d289c9fa3ea436c5c9ebca3c443d811e7ddf0a`  
		Last Modified: Tue, 29 Mar 2022 17:37:17 GMT  
		Size: 57.2 MB (57189052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3156bf80798d30be1ef0f7ad8315b4a6ce5313c937647b769cc5143f3b8cdff9`  
		Last Modified: Tue, 29 Mar 2022 17:37:51 GMT  
		Size: 204.0 MB (204048807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7e5308e1944fc1787dfd450bacba7bbe9859856f745a6e7aaa0ceddd6582b423
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.9 MB (303917448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4962b715d6e6bda7ec5550500040d73d5b3745a205d6f23532db0d1f089452`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:07 GMT
ADD file:6b5b5c095508b777a2c8b2633d97d6143bfab0320bed58e8e335179bfd681fc9 in / 
# Tue, 29 Mar 2022 00:49:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:38:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:38:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:39:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:42:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b209f6efb315c2c09d16e50d6077a10a401191c741a83c3c6c0767fe202d69d`  
		Last Modified: Tue, 29 Mar 2022 01:03:30 GMT  
		Size: 53.0 MB (52995524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc9d490149e4bcb11fe298e2c5a923c08cc31f08662f9f7637aca6473309b73`  
		Last Modified: Tue, 29 Mar 2022 08:02:54 GMT  
		Size: 5.2 MB (5163931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1132e128b11ccea17e38c248a34ec3142776903dcca038a3e7789c9e8f52f6a1`  
		Last Modified: Tue, 29 Mar 2022 08:02:56 GMT  
		Size: 10.6 MB (10597029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bea4cefcae02c237fe7371ca4d568c1f51b28d10f874dfcdd78ad48b4b5234f`  
		Last Modified: Tue, 29 Mar 2022 08:03:39 GMT  
		Size: 54.8 MB (54809370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5598b39f93060be7cdb0eb78efa2a5db7f9bb86aaee7fe02bb691c1b74c8938b`  
		Last Modified: Tue, 29 Mar 2022 08:05:28 GMT  
		Size: 180.4 MB (180351594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3057c536c7c6f68c195471d1f40f37b857d336191dbeb3b5b7fc48e7283edd80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294548530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c14b81fb84e8c247b2f7829800640a92be07e0c24c2aec452bd0333aae527c5a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 09:29:27 GMT
ADD file:819f7eacc6077672fc50aade09ce96ce0ef1e2b4d9bd84e706ea22d90d73799a in / 
# Thu, 17 Mar 2022 09:29:28 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 02:48:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 02:49:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 02:50:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 02:51:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7fca9c92eb5afd37d0b08a4fba4dd30ea576686d945af655ae46133854768127`  
		Last Modified: Thu, 17 Mar 2022 09:44:45 GMT  
		Size: 50.8 MB (50761706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5383ea443f2740a52246a5eee4a417a2b1244a1f912208d4c96428520670a4`  
		Last Modified: Sat, 19 Mar 2022 03:26:13 GMT  
		Size: 5.0 MB (5030714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d3f50feb52a7829302a09f9e4f362e90c5b18f7be314c43c43c6b1cbb89dea`  
		Last Modified: Sat, 19 Mar 2022 03:26:14 GMT  
		Size: 10.5 MB (10475768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66566945e25367a4d188cff5f444e5c148cf8c32c44b9a8b417c7c6950ce026`  
		Last Modified: Sat, 19 Mar 2022 03:27:01 GMT  
		Size: 52.8 MB (52827968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f449907892961828b09d71a6087b74860f8462bc407f9f83ee68955421731`  
		Last Modified: Sat, 19 Mar 2022 03:28:50 GMT  
		Size: 175.5 MB (175452374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:dc10872e9df18781834b0c42b03fe79668b23406008810d1e90621c64908d34c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.7 MB (326706748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4a83c9cea35cc589e8ead2e17e227e9f428a2cb832afc7d20ce0fa18a6fd4c0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:18 GMT
ADD file:c8087b65b6b61e4854699fe41f5bd7f307c0e0710204b586e85fd8176523d9bb in / 
# Thu, 17 Mar 2022 03:21:19 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:08:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:08:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 22:09:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:10:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:906df7cbb9fee5eb5d79c51ae55b6a857335ddd1b44645e3a59b3a50862f4317`  
		Last Modified: Thu, 17 Mar 2022 03:27:23 GMT  
		Size: 54.7 MB (54668239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bee854a2c1d4d436485263d8648a3eb5c0a4cdc26326102c680903b409889d`  
		Last Modified: Thu, 17 Mar 2022 22:19:48 GMT  
		Size: 5.3 MB (5256412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f88519bd8fe148fde1d5a9917fbea41afdd523e19fcecf2dc8f2f39c86cfbe`  
		Last Modified: Thu, 17 Mar 2022 22:19:49 GMT  
		Size: 10.7 MB (10676785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679d36783a2b174a0e8ee03bc292d3fdd5d57461299a881aa3561e5313ff763f`  
		Last Modified: Thu, 17 Mar 2022 22:20:09 GMT  
		Size: 57.2 MB (57222374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffb92c1d1edb0bb67024b345c9e4455169845b0e4807004f036901c1a23c815`  
		Last Modified: Thu, 17 Mar 2022 22:20:45 GMT  
		Size: 198.9 MB (198882938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8851d1e8a77483566b82195c9eaffceea6b155944274e3e51755a7776a38983f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.1 MB (336094169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d22e95f6da9cb5a3ef8107bf0dca8187b7f438b41ea53d8c835986af951337`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:20 GMT
ADD file:828aa883b729cb9e3bbc9efef043626425a2803461bd7b07862d746e2df08c10 in / 
# Tue, 29 Mar 2022 00:41:21 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:53:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:55:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e0acfe1e9e31a265994eee72788e1a0b4b33edc5c9d6fc978fd65d87aa94b53`  
		Last Modified: Tue, 29 Mar 2022 00:47:47 GMT  
		Size: 56.6 MB (56628219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e1b01718568970f8976ea798ed333d8acb22b4cdc57a341b078bb0a7e4e4dc`  
		Last Modified: Tue, 29 Mar 2022 18:13:41 GMT  
		Size: 5.4 MB (5400088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296971f2bacc0edb451554653b20751f9adfa0cbce82cb5e06a78c72076b036a`  
		Last Modified: Tue, 29 Mar 2022 18:13:41 GMT  
		Size: 11.1 MB (11103529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556f03b11aedb9bbc81a6111cf72e7c011c9682d79ce42ad6dba4bac5f1a2340`  
		Last Modified: Tue, 29 Mar 2022 18:14:03 GMT  
		Size: 58.6 MB (58613121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c72142fbc612ab497e789e0cf317e15155ad755a807c55a5e0c33308079666`  
		Last Modified: Tue, 29 Mar 2022 18:14:42 GMT  
		Size: 204.3 MB (204349212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4b96719aa342c4bfd8465cef5960ac34e4b1ef74915e068e1f157ce0adc065d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313279863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94cb436aa3e4b96d1b765561aadd9908d0b900046f7c6612823f0e3d0b33198a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:40:39 GMT
ADD file:88e75745fdbfd0784c1c18134a0a52a5534df18201a6f49555a5c618b4531804 in / 
# Tue, 29 Mar 2022 07:40:44 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:16:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:17:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 08:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:26:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bdc3f4c024aea887030bcf477ee808da6aa3e6683fb111845d94ab4f2480ff24`  
		Last Modified: Tue, 29 Mar 2022 07:50:58 GMT  
		Size: 54.2 MB (54240334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e94f68f0d96094b4bd1aa9ba6f4465ec7d6879ed28f910b949ffb165eef3fe`  
		Last Modified: Tue, 29 Mar 2022 08:54:21 GMT  
		Size: 5.2 MB (5221857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd581c56a027feec68bb7a881cac731bca045297cd76398414512c34351a063d`  
		Last Modified: Tue, 29 Mar 2022 08:54:24 GMT  
		Size: 10.7 MB (10672471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3631eb84b5e85d4e37526f1ae6b1259a7a43e8e02c45f72f851783117629e90a`  
		Last Modified: Tue, 29 Mar 2022 08:55:13 GMT  
		Size: 56.0 MB (55951132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365030772f8d919db49c949fdcb31ab34f90afe192c43a10bf522b2eab07e743`  
		Last Modified: Tue, 29 Mar 2022 08:57:20 GMT  
		Size: 187.2 MB (187194069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:70a287c3d178338b504a3651dfa532860d3a3a1a99f6e9e420bfa69553a225d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.8 MB (347787569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da1b34af902135a39f779c4a5b5782bff7e73e161cc6177a746b2d63d300c5c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 11:16:03 GMT
ADD file:f36cb09b5dc4cc09d85cfa372e4eab4761ae2e6db21140cd04ae6ac162780fa9 in / 
# Thu, 17 Mar 2022 11:16:14 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 05:28:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 05:29:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 05:30:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 05:38:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:829e07eac0f4532ec122618377e35dc25b8df14f3a8c8760107a868520ea7977`  
		Last Modified: Thu, 17 Mar 2022 11:26:42 GMT  
		Size: 60.2 MB (60181798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6b3254a8b049acdfea0695e77b1a65674284fb016e967d686cd004440b01c8`  
		Last Modified: Sat, 19 Mar 2022 06:36:37 GMT  
		Size: 5.5 MB (5538587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4496ff18aa5cb8cfce7705eb961453fcba1af247cee4d0ead60d54b6fdebda`  
		Last Modified: Sat, 19 Mar 2022 06:36:38 GMT  
		Size: 12.0 MB (11998277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9c5aeb5958db68933e2187c1ff6579c1f3c96b4e0fe8c7d451d5628430942b`  
		Last Modified: Sat, 19 Mar 2022 06:37:35 GMT  
		Size: 61.9 MB (61919466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcefa4029a54f0a3400cb6545cd8733c731d6c2f28baaeb0f7287435a6b89cd`  
		Last Modified: Sat, 19 Mar 2022 06:39:14 GMT  
		Size: 208.1 MB (208149441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ee52198958ed6b43a532c277c17fe850360a88e61b71d69a48eeb2059133ca25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.4 MB (306360438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02c4c96fd2d6a2a4c551ea765ad85ceced07b67b7b77234aa6c73b02d09d0a33`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:02 GMT
ADD file:82d5e48a017e9f867dce69500059071538b25dc5395a355bb79bfed992fb8cab in / 
# Thu, 17 Mar 2022 03:06:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:19:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:19:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 18:19:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:20:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91cc6fa8b00e7facc9855a15de9dbb6211a8692978d893a028e487ca7988379b`  
		Last Modified: Thu, 17 Mar 2022 03:11:59 GMT  
		Size: 54.0 MB (54000921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2c6272c85978c4b20b105a7a33a11881628bc38840c72128a526cdc6b709ab`  
		Last Modified: Thu, 17 Mar 2022 18:28:20 GMT  
		Size: 5.3 MB (5250449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900da87743fe44ae1fee0a700fae42c07e9ade18d95f98fbace40ab318fb4846`  
		Last Modified: Thu, 17 Mar 2022 18:28:20 GMT  
		Size: 10.8 MB (10803619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895f1b87cddc9e80df0130457e34d2b02b2e3a3700aab72bc40ee7ce09612250`  
		Last Modified: Thu, 17 Mar 2022 18:28:33 GMT  
		Size: 56.6 MB (56560505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d85dff32c741be680f86736f73847c567fc4f53dc0eb1cb045e3938bf1ed87`  
		Last Modified: Thu, 17 Mar 2022 18:28:59 GMT  
		Size: 179.7 MB (179744944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
