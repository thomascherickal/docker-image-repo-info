## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:d5f56a7f29a22f17db3a0a4e9bea5d9dae254d4940c7623df31fdb256475db73
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
$ docker pull buildpack-deps@sha256:2d4112f0a0fe6644dbc470ce26d2b46fa9d98048840705bf39e7385f43454bf8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.3 MB (328263587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c9c8cd4e6ee4affbe4c12a5a146baa1a5e65842700a331d474882114d4dd64`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:28 GMT
ADD file:49aaad883f9932e76df5604c9353bdbc51cd2c74b986b57b2dbb4f3aeaa46404 in / 
# Tue, 09 Jun 2020 01:22:28 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:54:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:54:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:55:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:55:58 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:516091449b2853b301713d61c7a73bfbe7ae63ace598e76e1d5e9da246f88b37`  
		Last Modified: Tue, 09 Jun 2020 01:27:16 GMT  
		Size: 51.5 MB (51526780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3385de445fd2842a13718698d3fa721fdd723aaede5f9cc079f9bc763e815830`  
		Last Modified: Tue, 09 Jun 2020 02:01:38 GMT  
		Size: 7.9 MB (7920994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd8a6c64c26854ad6d393a2096bb413e86391dc5861cc5a961eb2c55eaa1f63`  
		Last Modified: Tue, 09 Jun 2020 02:01:40 GMT  
		Size: 10.6 MB (10579754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fdc4632caaecd4275038ef75a4d7591fe4f368589453a583a1ee078a8ea6b5`  
		Last Modified: Tue, 09 Jun 2020 02:01:55 GMT  
		Size: 59.3 MB (59345488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0adac4777207eceebd46561aa9743b88b91637394ea5e743f1ee87fdee73f0`  
		Last Modified: Tue, 09 Jun 2020 02:02:29 GMT  
		Size: 198.9 MB (198890571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fa2de73b09b456e870fe489a3be9791f0d77f09050fbe64ae69ac0e76a0278f2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.6 MB (299588561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc107311ef12681f4bdff5a663221bd607a69b49f8913b6a6f6f469ca8ff2db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:54:09 GMT
ADD file:333f6925c41655ef86c1c55aa4628d69f324c5f263e27174c329a670a7408728 in / 
# Tue, 09 Jun 2020 00:54:11 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:40:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:49:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e514d65a1f93d9b21040cfb52628de87401493f0b2eb92f1a22c9d381f15df3b`  
		Last Modified: Tue, 09 Jun 2020 01:01:40 GMT  
		Size: 49.5 MB (49505780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da95254689f8f0bf61ba2fb5802bcfd31293fb3a56d7c3ee6b7653d100b6e62f`  
		Last Modified: Tue, 09 Jun 2020 02:00:49 GMT  
		Size: 7.5 MB (7500859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e156bd6d1d602264fe07ee2e4da6116f3627a0cdcb05d3f8452ab7e6a15fc5`  
		Last Modified: Tue, 09 Jun 2020 02:00:50 GMT  
		Size: 10.3 MB (10265113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64920f1a1e404f43b9ad025af513da62eb1e49466c92adafed377f2c5543974`  
		Last Modified: Tue, 09 Jun 2020 02:01:18 GMT  
		Size: 56.9 MB (56882678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e193e5c27d3058d3eb2eb9740840f3ebdf9b298b137108bfd48fc5c6e3b211c`  
		Last Modified: Tue, 09 Jun 2020 02:02:19 GMT  
		Size: 175.4 MB (175434131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f7b8c9a742a53abb5a1c9ce72a50445c2f3768ee643b1da0ec45186828e8e0ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.8 MB (293805077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeafa8f74d2f205fb5b6208540c76c84fd8fd43e66400221ad65ffe902c56ad9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:04:25 GMT
ADD file:f137ab200a6655933430876a9a0f3c675ed39dbf4a73be4750579b0c66812888 in / 
# Tue, 09 Jun 2020 01:04:32 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:58:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:59:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:59:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:369ddd165e2326d11cacb52bac2afd8d2277bc9506399fb693a5a5eb336716ee`  
		Last Modified: Tue, 09 Jun 2020 01:12:30 GMT  
		Size: 47.3 MB (47326325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ada3ce7a1b468f31af8a1aa9f083d4521fbeedd0d46757dc5d1f97c49ebf17`  
		Last Modified: Tue, 09 Jun 2020 02:13:48 GMT  
		Size: 7.2 MB (7243269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab399397acddc3f7ce3a847871519a272a15f91ee26bd786a485bf8a41dc870`  
		Last Modified: Tue, 09 Jun 2020 02:13:50 GMT  
		Size: 9.9 MB (9916653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfd7032d9f8bf51476a074156f4ebd7aa42e52d8e07b6e899f787d2eb56a14b`  
		Last Modified: Tue, 09 Jun 2020 02:14:15 GMT  
		Size: 54.4 MB (54429079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761692937defcf312878f98836fcce81ed37ef47411ce26721d05a3be9fc6929`  
		Last Modified: Tue, 09 Jun 2020 02:15:05 GMT  
		Size: 174.9 MB (174889751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4a6d9c2a2433330cab26b185b67b92fb61d15d82ae8d53e48c1ef684311e1b69
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.2 MB (320194018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:404dc58c41658b141104b5cf52433511ece9e8e2f5ca6730701be3b02bccb5b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:53:03 GMT
ADD file:56e3fbb5c1d0a4c301b36e4f85f596b26f32562da8ed0a704496f1e3ca5c676a in / 
# Tue, 09 Jun 2020 01:53:06 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:35:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:35:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:36:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:38:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f925f2558464755f2d5e30c33f6f9072851b0da5fb44204c52fcecdfb3bfbb44`  
		Last Modified: Tue, 09 Jun 2020 01:59:06 GMT  
		Size: 50.5 MB (50491571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b751eeb6110560d41a2af99cdea392104b87433a0ba6fd41a17872f77369f134`  
		Last Modified: Tue, 09 Jun 2020 02:48:52 GMT  
		Size: 7.8 MB (7795590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284f1451ccb4e8af4e45ad26e876fb36dc52c07dd21d5c4b226f8ac6a9407fba`  
		Last Modified: Tue, 09 Jun 2020 02:48:51 GMT  
		Size: 10.6 MB (10588456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac4f07de830aebf1a95a75c20d01a9d7b137067dcc03270e4b2817c78bdb0bb`  
		Last Modified: Tue, 09 Jun 2020 02:49:16 GMT  
		Size: 59.5 MB (59468248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2ef7d7ca7ec4ca944107ba51219a4ad9618d4231a1a1d68a0529084cf9bd76`  
		Last Modified: Tue, 09 Jun 2020 02:50:08 GMT  
		Size: 191.9 MB (191850153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b528bcddd995123deff89c1193c06f89641958a2547bd3a35edf11ff929bdc6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338321839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f281c9da2e0f6177e5dbde7692e3aec81f3269291b17e3affd35544cd71d692`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:41:24 GMT
ADD file:e46d18aaa3cf0eb6320c1b26b025ee8fbec78b2c4e4b3f5d4343393f1cbc769b in / 
# Tue, 09 Jun 2020 01:41:24 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:23:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:24:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:24:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:26:08 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c73d5896f1a36fe56b17fa2ffd2771c0b97b78e1b086e696cfa14b05618bbeee`  
		Last Modified: Tue, 09 Jun 2020 01:47:08 GMT  
		Size: 52.6 MB (52644936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf148f44d6df7cce1b2964667971df2c24df9d24505794d9324b303eff4da0b`  
		Last Modified: Tue, 09 Jun 2020 02:35:07 GMT  
		Size: 8.1 MB (8099472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa8c598f01778284c7219a5d6e3853bc2247c68a8e1ce0851af567867177c31`  
		Last Modified: Tue, 09 Jun 2020 02:35:07 GMT  
		Size: 11.0 MB (10960005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c50a355d1547fd485f5847386487c1b5c9e1b423bb328cfa13d40d4ccf5709d`  
		Last Modified: Tue, 09 Jun 2020 02:35:36 GMT  
		Size: 61.5 MB (61481714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da16fae9376ad69103ad5ad184b5c9092db29e6260a29e137fce4a9fa391fb14`  
		Last Modified: Tue, 09 Jun 2020 02:36:53 GMT  
		Size: 205.1 MB (205135712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:68da9c2ca1a71cdfaf8e2ce46a1ffc48749ea9f2e851f502a396dd40a7f7915d
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.8 MB (311843452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:282e4144a06a5c5b69030dfe20a744da71b6f081fa14ab38706d2756d3e6f273`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:11:18 GMT
ADD file:2c0e5d72dc26223a4df660e91acd4c8c70d1b0ee1139c92fb9cb3f041d81bdc2 in / 
# Tue, 09 Jun 2020 01:11:19 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:57:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:00:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:78e0a34f3ecd34b89d20cdb0b915427acd1691184f4f7649f816759737ddb842`  
		Last Modified: Tue, 09 Jun 2020 01:20:19 GMT  
		Size: 50.3 MB (50264875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff174bb9582ec89056fe600d1820b6c6e7445d74e52537dfea39a4dd2b4324e`  
		Last Modified: Tue, 09 Jun 2020 02:14:03 GMT  
		Size: 7.4 MB (7447530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a44807d6533dba987e8712d4b69466283e5bbe760298ac86ccbe1ed4ea542e2`  
		Last Modified: Tue, 09 Jun 2020 02:14:05 GMT  
		Size: 10.6 MB (10598855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46849a421d1ddb3755126f8b58c93389f656c6533dd46480416ce5fe6af98d6`  
		Last Modified: Tue, 09 Jun 2020 02:15:04 GMT  
		Size: 58.3 MB (58255965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a1c2305900b714d831f6e7eb3c142aa2d551e99840444f8ce45d7b6f4359cb`  
		Last Modified: Tue, 09 Jun 2020 02:17:30 GMT  
		Size: 185.3 MB (185276227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:596294dd7d3c8909a19bc67a3ab43642e2f957ead48716d7669c76708f5dbb80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.8 MB (348753748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edd71f8b2da39a89ebb4ac1c9f3418e06dc082436a8e9f63c3ac5e94b270a00`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:28:26 GMT
ADD file:7e16c349b13e97e4784ee396bb36ab2d3a069714388b0803f18ceb8d526be36a in / 
# Wed, 13 May 2020 22:28:35 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:55:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:56:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:57:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:07:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2aad5ee0ac7c9bdb0530f0a2f94bcadce58437453bcbdc7a2f20b5366c22799`  
		Last Modified: Wed, 13 May 2020 22:59:47 GMT  
		Size: 55.1 MB (55111830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bb4a67eb9efabb0bee7a8a6ff0c8c5d8b09a6992b8574669e941eb06ffe22d`  
		Last Modified: Thu, 14 May 2020 00:33:24 GMT  
		Size: 8.4 MB (8356775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba850bd6d1e4314d0d2953223c98e2452ff03935b42d421bbd2d54ca027da5f4`  
		Last Modified: Thu, 14 May 2020 00:33:24 GMT  
		Size: 11.2 MB (11176751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dc99aced2c3410b9c7fc622fe0d8acdcfb87cde0748b3dcf4eb683bbaabc75`  
		Last Modified: Thu, 14 May 2020 00:34:44 GMT  
		Size: 61.0 MB (61049801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bfb8ac6c8c068a55886224be2e4a5c5de176a66acdafe3ed54871b23e022290`  
		Last Modified: Thu, 14 May 2020 00:37:25 GMT  
		Size: 213.1 MB (213058591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ff4b3c197ddc556fe292837a50957e19018ed9cc460e57e25be7703cc6981ca0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308931231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15905a448775abf626e3fd2a6175269c903cd0db374575a09844068e5c7c2f6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:43:14 GMT
ADD file:f1ebbcfe99a36749cfce4bf2c38aff7e5a06ff0eee49c1c44970cb518d59c6c1 in / 
# Tue, 09 Jun 2020 01:43:17 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:11:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:11:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:12:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:68d68a3a62e23bc275e3488ccf04bd3d9cf392e7f00f7ac29a6f1d74be8ec63f`  
		Last Modified: Tue, 09 Jun 2020 01:47:06 GMT  
		Size: 50.2 MB (50155657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69552bf02d312240efc0fa7fe7d03054f5a709076df8a08878cd0782b3cac8b`  
		Last Modified: Tue, 09 Jun 2020 02:18:53 GMT  
		Size: 7.6 MB (7589963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77d73b4136a153380a7e5348a698053b0ee98f961fe50d20e65ca30de8da8d`  
		Last Modified: Tue, 09 Jun 2020 02:18:53 GMT  
		Size: 10.5 MB (10456030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6895be31368f26dc7d04d4c9a689adae6dddc460d56bca91594be43fed86789a`  
		Last Modified: Tue, 09 Jun 2020 02:19:08 GMT  
		Size: 58.5 MB (58518718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b63231c042b7591f737076426c99a73956b0c1b342b55eccd574840f37ed84`  
		Last Modified: Tue, 09 Jun 2020 02:19:34 GMT  
		Size: 182.2 MB (182210863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
