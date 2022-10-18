<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neurodebian`

-	[`neurodebian:bionic`](#neurodebianbionic)
-	[`neurodebian:bionic-non-free`](#neurodebianbionic-non-free)
-	[`neurodebian:bookworm`](#neurodebianbookworm)
-	[`neurodebian:bookworm-non-free`](#neurodebianbookworm-non-free)
-	[`neurodebian:bullseye`](#neurodebianbullseye)
-	[`neurodebian:bullseye-non-free`](#neurodebianbullseye-non-free)
-	[`neurodebian:buster`](#neurodebianbuster)
-	[`neurodebian:buster-non-free`](#neurodebianbuster-non-free)
-	[`neurodebian:focal`](#neurodebianfocal)
-	[`neurodebian:focal-non-free`](#neurodebianfocal-non-free)
-	[`neurodebian:jammy`](#neurodebianjammy)
-	[`neurodebian:jammy-non-free`](#neurodebianjammy-non-free)
-	[`neurodebian:latest`](#neurodebianlatest)
-	[`neurodebian:nd`](#neurodebiannd)
-	[`neurodebian:nd-non-free`](#neurodebiannd-non-free)
-	[`neurodebian:nd100`](#neurodebiannd100)
-	[`neurodebian:nd100-non-free`](#neurodebiannd100-non-free)
-	[`neurodebian:nd110`](#neurodebiannd110)
-	[`neurodebian:nd110-non-free`](#neurodebiannd110-non-free)
-	[`neurodebian:nd120`](#neurodebiannd120)
-	[`neurodebian:nd120-non-free`](#neurodebiannd120-non-free)
-	[`neurodebian:nd16.04`](#neurodebiannd1604)
-	[`neurodebian:nd16.04-non-free`](#neurodebiannd1604-non-free)
-	[`neurodebian:nd18.04`](#neurodebiannd1804)
-	[`neurodebian:nd18.04-non-free`](#neurodebiannd1804-non-free)
-	[`neurodebian:nd20.04`](#neurodebiannd2004)
-	[`neurodebian:nd20.04-non-free`](#neurodebiannd2004-non-free)
-	[`neurodebian:nd22.04`](#neurodebiannd2204)
-	[`neurodebian:nd22.04-non-free`](#neurodebiannd2204-non-free)
-	[`neurodebian:non-free`](#neurodebiannon-free)
-	[`neurodebian:sid`](#neurodebiansid)
-	[`neurodebian:sid-non-free`](#neurodebiansid-non-free)
-	[`neurodebian:xenial`](#neurodebianxenial)
-	[`neurodebian:xenial-non-free`](#neurodebianxenial-non-free)

## `neurodebian:bionic`

```console
$ docker pull neurodebian@sha256:4beab2d9de10f5c74669b7aad7fe9c38a0ca77109ce16e33e2cf46a6bdbe1fe8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:a4563092987a9094f629e918b696638826ac17270d6e4b4844c943cbacdf8c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31769449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6c5a3eb19316317ceea7d7dd57d8206854e2c096749ec0163c48ffcf59d4b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:35:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:35:52 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:35:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:35:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b326536d9135ba21a7d81e94b00d7908a0e98db7443d55decaace2cadae22f`  
		Last Modified: Wed, 05 Oct 2022 04:39:47 GMT  
		Size: 4.8 MB (4815599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfeae315539086179fc071cd4f1866e8c8d38765cf68e5832d07bdb7388fdc8`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7ceb3ac42fa70ccfe5e470e0efc92d4b1c90e54fcdaf9a451bacc6107bd91f`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca5b1ce88f0b3604342d8ec51ae31e8d9af4dde0b98e0e039eebd8ede5a78fa`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 240.1 KB (240089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:3106ed7f09960a95ba5d9da7894ddd0272aed0a27baaf35acde7b4387ec53d87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28107422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a836588eaf2b8b33d9904fa7774955073c4c6f56baa00c908b948876ad437cbf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:56:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:56:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:56:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:56:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415982c552b3097dc0f0e3fdab4c2932671fee8d829436501ccb051e6eb83500`  
		Last Modified: Wed, 05 Oct 2022 04:01:19 GMT  
		Size: 4.3 MB (4263811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521f05b326e0e79919ca42ac9a0c47cb9f1caeffc488a7c889282f7fdc7783ab`  
		Last Modified: Wed, 05 Oct 2022 04:01:18 GMT  
		Size: 1.6 KB (1639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea2e867535975d3209819774df2886ba41c121200bbe2c7d447a1e76754391`  
		Last Modified: Wed, 05 Oct 2022 04:01:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53cf70e35b0e254b43fe67021ea0499f47207b931b8d33c35d44b684e86ce1d`  
		Last Modified: Wed, 05 Oct 2022 04:01:18 GMT  
		Size: 107.1 KB (107134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bionic-non-free`

```console
$ docker pull neurodebian@sha256:121585e3ab450a44b229835895f4517a1e4ea0a29a5661aa743f1cab99064509
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:241e8b93af0e677ab1c024ab6e004344c3591193a9be7ae6ce029c5bae66f2d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31769706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4758b5a325ceebffec9976a3a336b62594cea44d24465903f9db4e780d72c4f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:35:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:35:52 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:35:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:35:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:36:06 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b326536d9135ba21a7d81e94b00d7908a0e98db7443d55decaace2cadae22f`  
		Last Modified: Wed, 05 Oct 2022 04:39:47 GMT  
		Size: 4.8 MB (4815599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfeae315539086179fc071cd4f1866e8c8d38765cf68e5832d07bdb7388fdc8`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7ceb3ac42fa70ccfe5e470e0efc92d4b1c90e54fcdaf9a451bacc6107bd91f`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca5b1ce88f0b3604342d8ec51ae31e8d9af4dde0b98e0e039eebd8ede5a78fa`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 240.1 KB (240089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38536dc9dd91716f882e2f305d71c20ccff6acb2ec0a5193f51ee490b91e06d`  
		Last Modified: Wed, 05 Oct 2022 04:39:55 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:960a7526392894300331ed782ff021b9064ebce94cfe42e5045859e17125fced
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28107677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c978717a3a838e157a52e5cd1a4b004a4483d7a2c137f26dd49b70bbdf2772a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:56:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:56:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:56:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:56:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:57:03 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415982c552b3097dc0f0e3fdab4c2932671fee8d829436501ccb051e6eb83500`  
		Last Modified: Wed, 05 Oct 2022 04:01:19 GMT  
		Size: 4.3 MB (4263811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521f05b326e0e79919ca42ac9a0c47cb9f1caeffc488a7c889282f7fdc7783ab`  
		Last Modified: Wed, 05 Oct 2022 04:01:18 GMT  
		Size: 1.6 KB (1639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea2e867535975d3209819774df2886ba41c121200bbe2c7d447a1e76754391`  
		Last Modified: Wed, 05 Oct 2022 04:01:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53cf70e35b0e254b43fe67021ea0499f47207b931b8d33c35d44b684e86ce1d`  
		Last Modified: Wed, 05 Oct 2022 04:01:18 GMT  
		Size: 107.1 KB (107134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62049f0f865fe4debb6e085c8399238bd0435ae872e5fcdbd8a784dcfaf45f5b`  
		Last Modified: Wed, 05 Oct 2022 04:01:29 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm`

```console
$ docker pull neurodebian@sha256:79ed50d7fea07cb407771e5be79af216bb69c992b9535d126ad02e9d298536cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm` - linux; amd64

```console
$ docker pull neurodebian@sha256:80e495f56a8237c8cfa8e2e3b3dd9e54a505a4f883d316a4240a21b7041aecb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65014055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a3ff4e52f917a5a8d864f577fa58cbf9cfc295b40f922b27828012fb5cf890`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:36 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2316c52551cab9cc0ad9166bc77e216033702e8aaabffc0abcfb89f136d8c76`  
		Last Modified: Wed, 05 Oct 2022 04:41:29 GMT  
		Size: 11.8 MB (11764299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe69058d31d6cd9481204bc8bf1336732437d0660a1d75e5f65767c22a94bb9`  
		Last Modified: Wed, 05 Oct 2022 04:41:27 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87205a6c66a4f8e9f0acef27904269125540931696cbeef7b33f8df121ac2edd`  
		Last Modified: Wed, 05 Oct 2022 04:41:27 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8368ed01254e7fabcaccc37943c9d4b1b860ee0375ed75e45c834a9c52ade31`  
		Last Modified: Wed, 05 Oct 2022 04:41:28 GMT  
		Size: 285.3 KB (285329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:04b205e6757ccaee181d6b9df9a36655883160250f742d021117a3a1b1cfff4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64610344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a08ab62e18104657885408c27ceefaa2eab492b53f852b8affb14b0c2faa55`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:00 GMT
ADD file:269c8bec4871d84b9133706a2f391209619d53c0bfa56121c740757cf5798fcb in / 
# Tue, 04 Oct 2022 23:44:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:59:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:59:23 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2debf9e7f23054c81a936da9b01c5db9f72a55d4810f7bf0e5641bd1748d90b7`  
		Last Modified: Tue, 04 Oct 2022 23:49:11 GMT  
		Size: 53.0 MB (52980389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0ef51f5528c6564ff374a45d9cb4c4c6eaf535c3565cbb4ba763bc55b22343`  
		Last Modified: Wed, 05 Oct 2022 04:03:24 GMT  
		Size: 11.5 MB (11531064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469c79e490be5fc87427c713b2cff0a58e2d249f09613ea11f6d6a02ed9e62f7`  
		Last Modified: Wed, 05 Oct 2022 04:03:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a22ac0a033238596c38df2f9af0747aa62ed9470c2a82f61ed8978d6ccc5f`  
		Last Modified: Wed, 05 Oct 2022 04:03:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bc59e065b02635051c28a8a2b68751fbdc3486f83ce39b848da35674d67b13`  
		Last Modified: Wed, 05 Oct 2022 04:03:23 GMT  
		Size: 96.9 KB (96904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; 386

```console
$ docker pull neurodebian@sha256:73316bae3c4e7a4271e81a96da0a8a0cb7c42d32b91c42c8d4ba42585d386780
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66022618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:618ae15fc21beb4669f25359429e3e4605519f66976d8c64d6879fa894af89e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:38:57 GMT
ADD file:2a0c743e373aeed6462c2f3ae8a138fb0e240e935ad7ca5bf008aa3efd3673a0 in / 
# Tue, 04 Oct 2022 23:38:58 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68776dad61a299b8e65d1a6a02e376b8ed2e9b241bd753bf6c35d497055ecdf`  
		Last Modified: Tue, 04 Oct 2022 23:44:23 GMT  
		Size: 53.9 MB (53932827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b23a7101cec8d64ddc2337801957f17d5366b0725dfb359c4a75a69d6a5e59b`  
		Last Modified: Wed, 05 Oct 2022 02:17:53 GMT  
		Size: 12.0 MB (11990988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bc6ea3e1edb50b087a2d132755dd424f332df905fd3ca53fc106283fa89192`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f7492185dc14c52e2b31a59607eac615a02bb456adcdd05c611ea2b460da27`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156209dfa890bcc23c8e351f1f08baad61399ccb713ea04a5f81e3d9a8d3760a`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 96.8 KB (96816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm-non-free`

```console
$ docker pull neurodebian@sha256:e824689fd765e6636fd053b8640c6c796089ca812aedeae435886e5b5368b67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:bd5355676c5af8e531fbb1f95cb73c50e8aded59a5bbd628ba410ab609d423a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65014415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54479f492559d1e663f6669b2c7233f7cdea30f616c8fcdfe326d874ebec17a7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:36 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:42 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2316c52551cab9cc0ad9166bc77e216033702e8aaabffc0abcfb89f136d8c76`  
		Last Modified: Wed, 05 Oct 2022 04:41:29 GMT  
		Size: 11.8 MB (11764299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe69058d31d6cd9481204bc8bf1336732437d0660a1d75e5f65767c22a94bb9`  
		Last Modified: Wed, 05 Oct 2022 04:41:27 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87205a6c66a4f8e9f0acef27904269125540931696cbeef7b33f8df121ac2edd`  
		Last Modified: Wed, 05 Oct 2022 04:41:27 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8368ed01254e7fabcaccc37943c9d4b1b860ee0375ed75e45c834a9c52ade31`  
		Last Modified: Wed, 05 Oct 2022 04:41:28 GMT  
		Size: 285.3 KB (285329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca0c4df391b41681b1f4c8259b14ac54ae55eaca35fa4729063e3b06d85119`  
		Last Modified: Wed, 05 Oct 2022 04:41:37 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:9fb15b3ee57c8ecf0c6fad7fbc5ce41d2124d2363d6d2532d4c74192ed6f5e4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64610704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a146677dea1903a8763fe0202bdc02ac58275e1db107f7d1a45d48d360d56b1a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:00 GMT
ADD file:269c8bec4871d84b9133706a2f391209619d53c0bfa56121c740757cf5798fcb in / 
# Tue, 04 Oct 2022 23:44:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:59:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:59:23 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:30 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:2debf9e7f23054c81a936da9b01c5db9f72a55d4810f7bf0e5641bd1748d90b7`  
		Last Modified: Tue, 04 Oct 2022 23:49:11 GMT  
		Size: 53.0 MB (52980389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0ef51f5528c6564ff374a45d9cb4c4c6eaf535c3565cbb4ba763bc55b22343`  
		Last Modified: Wed, 05 Oct 2022 04:03:24 GMT  
		Size: 11.5 MB (11531064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469c79e490be5fc87427c713b2cff0a58e2d249f09613ea11f6d6a02ed9e62f7`  
		Last Modified: Wed, 05 Oct 2022 04:03:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a22ac0a033238596c38df2f9af0747aa62ed9470c2a82f61ed8978d6ccc5f`  
		Last Modified: Wed, 05 Oct 2022 04:03:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bc59e065b02635051c28a8a2b68751fbdc3486f83ce39b848da35674d67b13`  
		Last Modified: Wed, 05 Oct 2022 04:03:23 GMT  
		Size: 96.9 KB (96904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86addfd21f29a2b3cc2f2d4caa2e71233a7f3263674e19b65321fcf5e03cc560`  
		Last Modified: Wed, 05 Oct 2022 04:03:36 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:a0419b3921c4500ce8017f99b534dd4c66e6641fdd63cf8d17d36a607b17dead
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66022979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee04776b466810c25260cd640d93dd96840d94e5bf91857e004aa6b5f454b5c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:38:57 GMT
ADD file:2a0c743e373aeed6462c2f3ae8a138fb0e240e935ad7ca5bf008aa3efd3673a0 in / 
# Tue, 04 Oct 2022 23:38:58 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:50 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c68776dad61a299b8e65d1a6a02e376b8ed2e9b241bd753bf6c35d497055ecdf`  
		Last Modified: Tue, 04 Oct 2022 23:44:23 GMT  
		Size: 53.9 MB (53932827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b23a7101cec8d64ddc2337801957f17d5366b0725dfb359c4a75a69d6a5e59b`  
		Last Modified: Wed, 05 Oct 2022 02:17:53 GMT  
		Size: 12.0 MB (11990988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bc6ea3e1edb50b087a2d132755dd424f332df905fd3ca53fc106283fa89192`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f7492185dc14c52e2b31a59607eac615a02bb456adcdd05c611ea2b460da27`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156209dfa890bcc23c8e351f1f08baad61399ccb713ea04a5f81e3d9a8d3760a`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 96.8 KB (96816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e038e92cc95c6ee9d08edbfccb0fd01d6cc3153d445b6ea5717491f57216b426`  
		Last Modified: Wed, 05 Oct 2022 02:18:04 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:2661841f96cd443d306b51d0d63a018642c1d31667dbb10df5e6160a7188cbf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:64f51985744c09f1eece661c9b0fae45e93716af39ca647cccd567a2271bc25d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66670584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98be26081cb0e38c2b3c1b3be93c7fd4165d11982e16c058f60bdbc9f906ef85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:05 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:06 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:07 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59519a823826166b6d39d758ec5014bd2a5a294b254600d211895dd9c5a866a`  
		Last Modified: Wed, 05 Oct 2022 04:41:04 GMT  
		Size: 11.3 MB (11310722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ec2e5570ce1fabd90c3f195db1c2491485e03dfbaa959a752acc6de8c4641`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f97d5eff53b93eef2dcda043176e5b2ad126bb890a82dd2f405b0f9fe26f5c7`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3860fd5292dee9ad38ed40b5bab9706f31cf24d1663060f1cda46eb7d4856cc8`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 311.6 KB (311600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:549507692b43319c3085c66c184331a3690843651c9856f1f1a451b2822abb7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64912635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3771988b0944a19a09d4efadebfc7d8a9cfbb1195dbd0f65a981d082e17e6c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:54 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32748b0f6967d6d3a663ec439e7a0b631ffe7f6e19fe0a854fa9f60cfbd8013`  
		Last Modified: Wed, 05 Oct 2022 04:02:54 GMT  
		Size: 11.1 MB (11104845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2cd3f4776c95e95f8cf2fe1866ba88b1f93d61bd9cf77c2b0454c13231a54`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74195093fe58a8f1f862fdb46f29db25a349b6d544a17872538f43ed9f69314`  
		Last Modified: Wed, 05 Oct 2022 04:02:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bb772dba620ade3ee2ee0b39ede83b9e4e52271a3c735aea72ebe200c60d9a`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 105.2 KB (105178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; 386

```console
$ docker pull neurodebian@sha256:faad9fd73720614aa3571453130adab314a1337233c23716ea029d9c8f2f5262
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67630593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82bebd1ae720b0a3624a349c8605a9c423db494f38f028eddfdfc8e500ab3db9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1913722e4098b05a88200af242b3e4de75036431d863b1330ca708cec7d52fda`  
		Last Modified: Wed, 05 Oct 2022 02:17:23 GMT  
		Size: 11.5 MB (11499735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16eddaf2626ebe571c30e863702e069074b6e5a9a22488db55e5d6dfdb41fdf8`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b6358b663dae0a2653ca7146baf655ba0e0e1b765ac7cc2914cdcc4390ea7b`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2069c1e6d4aa4c4d2b785d1396e8487db0a8e83ff092b0fae2d0454a2d6b9a2`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 105.1 KB (105067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:f0db759e1632d1225899599cce0dfb1562c8d3b39e20cddd98cdbf6055681840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:429703f7e0fee449ecf50ab4cc0361f089ca009722e969ee67d2cd0359c2b297
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66670946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95b57e27da6390014efb505383ed7bcf2053334cc51e76b3a2dbef13db3e7ebb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:05 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:06 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:07 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59519a823826166b6d39d758ec5014bd2a5a294b254600d211895dd9c5a866a`  
		Last Modified: Wed, 05 Oct 2022 04:41:04 GMT  
		Size: 11.3 MB (11310722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ec2e5570ce1fabd90c3f195db1c2491485e03dfbaa959a752acc6de8c4641`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f97d5eff53b93eef2dcda043176e5b2ad126bb890a82dd2f405b0f9fe26f5c7`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3860fd5292dee9ad38ed40b5bab9706f31cf24d1663060f1cda46eb7d4856cc8`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 311.6 KB (311600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3f2699fcf96f4273335b294c96598796754d1f07e7247bae8bdee5bc4a2e84`  
		Last Modified: Wed, 05 Oct 2022 04:41:16 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:6f6e001cebd2e7dc0a6dcdfac69f62ae40db3ad5a27873ceb5dcbdaa656bad5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64912994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a33532c39658d75d58079d13e51642f56eeac73e1fa42bd67e5e54408cd59f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:54 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:05 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32748b0f6967d6d3a663ec439e7a0b631ffe7f6e19fe0a854fa9f60cfbd8013`  
		Last Modified: Wed, 05 Oct 2022 04:02:54 GMT  
		Size: 11.1 MB (11104845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2cd3f4776c95e95f8cf2fe1866ba88b1f93d61bd9cf77c2b0454c13231a54`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74195093fe58a8f1f862fdb46f29db25a349b6d544a17872538f43ed9f69314`  
		Last Modified: Wed, 05 Oct 2022 04:02:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bb772dba620ade3ee2ee0b39ede83b9e4e52271a3c735aea72ebe200c60d9a`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 105.2 KB (105178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe1986c4b98c09310059dfffefb45f157872b7f5c09d1d2d4c4a68e3acfb272`  
		Last Modified: Wed, 05 Oct 2022 04:03:08 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:49bec358473d52c6911c4c6deae5298035893c9faf0b40a00f42e315e067caa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67630953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d31e9115c7ef837ee295344dd83e413d4164b55f4a4b8fb32836479f79316ebf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1913722e4098b05a88200af242b3e4de75036431d863b1330ca708cec7d52fda`  
		Last Modified: Wed, 05 Oct 2022 02:17:23 GMT  
		Size: 11.5 MB (11499735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16eddaf2626ebe571c30e863702e069074b6e5a9a22488db55e5d6dfdb41fdf8`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b6358b663dae0a2653ca7146baf655ba0e0e1b765ac7cc2914cdcc4390ea7b`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2069c1e6d4aa4c4d2b785d1396e8487db0a8e83ff092b0fae2d0454a2d6b9a2`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 105.1 KB (105067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fcc7395aa5a726c6a498dace0389db7c1a51fa808ba67dfecf838c90d83dd7`  
		Last Modified: Wed, 05 Oct 2022 02:17:37 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:704d61176624378d00d12746b1e028e1973852c3ff9789f09201f41b177e535b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:bac54f40a6dd681e8e608373b4938df13f0b3b3344aa9d33b50c60e2205b54be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61247541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:689b0d51aee9386015685a93d96881629b22b1ae333beb6d77c361cc6b7bc78c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:37:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:37:47 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:37:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a98ad9d5bfe5c93cdc5dd566aa7c846123d6b674612d8c22ce6c4506a1c72d`  
		Last Modified: Wed, 05 Oct 2022 04:40:45 GMT  
		Size: 10.5 MB (10501516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a8bc5b640eb70d850ea36e9b51ae7b8fc76946e82ae1bb0642d47f0e0eb73`  
		Last Modified: Wed, 05 Oct 2022 04:40:44 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f286e51e987b82a169deb249e7d1398676dca1955e72e0976dc9302cfe8b7a`  
		Last Modified: Wed, 05 Oct 2022 04:40:43 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0eb25a875218ed1b804497338449bbaeb2129f8647aec7695c8ef06e71cad`  
		Last Modified: Wed, 05 Oct 2022 04:40:44 GMT  
		Size: 302.9 KB (302910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:2dc6d3c83993dc6a49fc286f9a1d6110258197edb1d3cacabec8b12d88d4becf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59636797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b50a8e93e8303cee10538cc56493e6e180c31a069561b078b566065bc62aca2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:28 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d154496b8ab72771340bbbfcb90129abefba06a0df134e694e436c32723ecf`  
		Last Modified: Wed, 05 Oct 2022 04:02:31 GMT  
		Size: 10.3 MB (10297436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef89a9a6d8113e10f9e579ee92783e306a5fa8bfe2acfa01e2d78d7fd818107f`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23704a18d02fdbc4131c6f7adfaaec3730093c5504d02a143c4a78f637028721`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d322400769bb470d58b21b11c9f6e84fb73d5e8603c40127b4804943ec7f7ec2`  
		Last Modified: Wed, 05 Oct 2022 04:02:30 GMT  
		Size: 108.5 KB (108492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; 386

```console
$ docker pull neurodebian@sha256:1fd4cf8b2a55d0059c7adddd50e16ea9c0b91e97458079defd08db84607e50a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61982452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4611172bd93ea6abd33eb27f96eeb688a884c754e831b30d565524925f180742`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:52 GMT
ADD file:887aa5460e148ba204780ebe976e5627d5f4d0a07faf22b86afe146998d75d79 in / 
# Tue, 04 Oct 2022 23:39:53 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:14:43 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:14:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:14:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:14:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:98d78922e3457a6697f2cdbddaab27dbb47e2e0beedb1a4348c56102c850b343`  
		Last Modified: Tue, 04 Oct 2022 23:45:58 GMT  
		Size: 51.2 MB (51202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a1c4ae5a735b6da355e52d679127188fc0385520109eb7c93e31b0fd3a7c5`  
		Last Modified: Wed, 05 Oct 2022 02:17:01 GMT  
		Size: 10.7 MB (10669155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127af1b441210177fdedbe41dc0aaf6ca644be580c15ae7a5cae51e8ff1bffce`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8999f6b03a0580644ff4a8ada4dec6b0d39eec0f624022a1b96f832f8fd28a21`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5c07173b4dcb13dbcc2b4c04cdbb7546fb67e2b14f21eea7653356ac3845ba`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 108.5 KB (108467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:1b8e6b396dd099b61e36a2b19d6900f814d81510c418f42a1d5cebf15aefd42a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:a2e3e436f3774637fecc2d35630111123e5ae75ba23ba63e83d57401b729b454
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61247897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d329a9df499d0dc0b3386b4766c5be22661ce5105b8fcf90606746add3e6bfec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:37:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:37:47 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:37:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:56 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a98ad9d5bfe5c93cdc5dd566aa7c846123d6b674612d8c22ce6c4506a1c72d`  
		Last Modified: Wed, 05 Oct 2022 04:40:45 GMT  
		Size: 10.5 MB (10501516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a8bc5b640eb70d850ea36e9b51ae7b8fc76946e82ae1bb0642d47f0e0eb73`  
		Last Modified: Wed, 05 Oct 2022 04:40:44 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f286e51e987b82a169deb249e7d1398676dca1955e72e0976dc9302cfe8b7a`  
		Last Modified: Wed, 05 Oct 2022 04:40:43 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0eb25a875218ed1b804497338449bbaeb2129f8647aec7695c8ef06e71cad`  
		Last Modified: Wed, 05 Oct 2022 04:40:44 GMT  
		Size: 302.9 KB (302910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534645635d433d322d0e0a9f9eb06a9ea23d56fd282b1576d7af7234e822cba0`  
		Last Modified: Wed, 05 Oct 2022 04:40:54 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:ae50d50c11c32068f7b0f868f8975041e8cc6381108233aa6926e8f2b4dbb863
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59637153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e1ca9d0cf271394b943e6c4dbc574cc3b61dbe9eed4fa82dbd4e4feaf92085c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:28 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:40 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d154496b8ab72771340bbbfcb90129abefba06a0df134e694e436c32723ecf`  
		Last Modified: Wed, 05 Oct 2022 04:02:31 GMT  
		Size: 10.3 MB (10297436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef89a9a6d8113e10f9e579ee92783e306a5fa8bfe2acfa01e2d78d7fd818107f`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23704a18d02fdbc4131c6f7adfaaec3730093c5504d02a143c4a78f637028721`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d322400769bb470d58b21b11c9f6e84fb73d5e8603c40127b4804943ec7f7ec2`  
		Last Modified: Wed, 05 Oct 2022 04:02:30 GMT  
		Size: 108.5 KB (108492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ebd81db9bac845b1da95a5029d74042c0045701de4248a1c4a035311b28efe`  
		Last Modified: Wed, 05 Oct 2022 04:02:41 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:fa77adad3506f7d86dae7b6965fe84a271c03357bb0d6a0a88cfcf84d9c5aec1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61982810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d524cf15f421c47fa01d99d0e92e1d401e54ffefa9ea0aec36d56ddd527a0e09`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:52 GMT
ADD file:887aa5460e148ba204780ebe976e5627d5f4d0a07faf22b86afe146998d75d79 in / 
# Tue, 04 Oct 2022 23:39:53 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:14:43 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:14:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:14:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:14:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:14:56 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:98d78922e3457a6697f2cdbddaab27dbb47e2e0beedb1a4348c56102c850b343`  
		Last Modified: Tue, 04 Oct 2022 23:45:58 GMT  
		Size: 51.2 MB (51202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a1c4ae5a735b6da355e52d679127188fc0385520109eb7c93e31b0fd3a7c5`  
		Last Modified: Wed, 05 Oct 2022 02:17:01 GMT  
		Size: 10.7 MB (10669155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127af1b441210177fdedbe41dc0aaf6ca644be580c15ae7a5cae51e8ff1bffce`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8999f6b03a0580644ff4a8ada4dec6b0d39eec0f624022a1b96f832f8fd28a21`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5c07173b4dcb13dbcc2b4c04cdbb7546fb67e2b14f21eea7653356ac3845ba`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 108.5 KB (108467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a0b36a65a1c2c95edc9bf80ee22743a8f9009433ee1c689bb97051f7899e85`  
		Last Modified: Wed, 05 Oct 2022 02:17:11 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal`

```console
$ docker pull neurodebian@sha256:c18c560f176eb46041715e6e82c11c58f8486836253dff54e820a6bbf72ca516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:7340e4a1d02b24f61c7891075156bc3aed757461b976e131fef72f65107c6477
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34303966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a497bfc7b1befd51e04e6c0d289e77563686c379b8b7dcec430b35816b5aed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:36:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:36:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:36:41 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:36:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6bd0f856bb7acc90ab4443dc259de1333cfda3d76a258b4ecffe0ba0423001`  
		Last Modified: Wed, 05 Oct 2022 04:40:05 GMT  
		Size: 5.5 MB (5488926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec95545cadde7556963cca6dbe9a7a582e532a753fe098f534873a5d44509c58`  
		Last Modified: Wed, 05 Oct 2022 04:40:04 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7103e2fd0a7a94665abf1b872037f51b8beb8142d737d76f5a9571a588df541b`  
		Last Modified: Wed, 05 Oct 2022 04:40:04 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e953560506e2981b9ab4b287853ba7c1e73ba4d90133660ee56b3dca93e904e`  
		Last Modified: Wed, 05 Oct 2022 04:40:05 GMT  
		Size: 238.6 KB (238576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:focal` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:9e19d92f322c13a32357ac60ed6dcd8bce328e15b35f44191da77e8b3822b9ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32618571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3105a115921035dc455c661504a462e1ca355aab8d920f6110d266e0fba37cac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:57:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:57:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:57:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:57:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3730a2cad9cb25a3678d78ba877c9bf0d220929e8f45f9bbff1817122e6f531`  
		Last Modified: Wed, 05 Oct 2022 04:01:41 GMT  
		Size: 5.3 MB (5320766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164c55950381db4d1b78a1b3a2b3f0d3f7bf4de0f4580eccbc1603928ed5b79`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518ae94eca7b012d8ed2f54bc625bd18bf6427860578d187cd9ee1a0a4860106`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2eae91864849c904d629b133ab443a99218e0b47f94c7eeffb491c93da3f31`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 104.2 KB (104194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal-non-free`

```console
$ docker pull neurodebian@sha256:360743995ac767035d3bd9990b6ef5eb7811fde37db655a229750a7770beab3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:focal-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:9a3d5e4551c0fde8c789e14f04f63ab2ca9daa7547a9bd25709b76e498c71fa5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34304221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4f6e86c5d058250cdb24ce593bf8d238019b88676c0ba86fc9a1574c38d71da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:36:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:36:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:36:41 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:36:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:36:49 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6bd0f856bb7acc90ab4443dc259de1333cfda3d76a258b4ecffe0ba0423001`  
		Last Modified: Wed, 05 Oct 2022 04:40:05 GMT  
		Size: 5.5 MB (5488926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec95545cadde7556963cca6dbe9a7a582e532a753fe098f534873a5d44509c58`  
		Last Modified: Wed, 05 Oct 2022 04:40:04 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7103e2fd0a7a94665abf1b872037f51b8beb8142d737d76f5a9571a588df541b`  
		Last Modified: Wed, 05 Oct 2022 04:40:04 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e953560506e2981b9ab4b287853ba7c1e73ba4d90133660ee56b3dca93e904e`  
		Last Modified: Wed, 05 Oct 2022 04:40:05 GMT  
		Size: 238.6 KB (238576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe62b2f572b42f89995db5d09adc8f81e9e2f77b2f8d99f052ba95cc9c82fc2`  
		Last Modified: Wed, 05 Oct 2022 04:40:14 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:focal-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:4c5340a833188322de86f6f98165eeb9dd0fec61c2bb1d7e1e72acc3b7530d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32618828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a76552309ba47602f9c6033627eb38098234d4aff78a0731d208ce33feaa2535`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:57:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:57:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:57:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:57:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:57:35 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3730a2cad9cb25a3678d78ba877c9bf0d220929e8f45f9bbff1817122e6f531`  
		Last Modified: Wed, 05 Oct 2022 04:01:41 GMT  
		Size: 5.3 MB (5320766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164c55950381db4d1b78a1b3a2b3f0d3f7bf4de0f4580eccbc1603928ed5b79`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518ae94eca7b012d8ed2f54bc625bd18bf6427860578d187cd9ee1a0a4860106`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2eae91864849c904d629b133ab443a99218e0b47f94c7eeffb491c93da3f31`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 104.2 KB (104194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92cce2f79bfc53f2bbb7601d0755d5b4bff78cd90ab4898e0a1b36ebda80904`  
		Last Modified: Wed, 05 Oct 2022 04:01:52 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:jammy`

```console
$ docker pull neurodebian@sha256:1f56af1fef4b30426331394c4163f22eaa7a8fc2e51485308c5ffb25ef26e855
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy` - linux; amd64

```console
$ docker pull neurodebian@sha256:68570c859f56a40662fdd5ad693da8340bc814ff1062e465bfd702f06c511aa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34454380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab7a779e9e317fab6b650b30df728b9a6bff2ecfe4c130df9f31e8ddea298ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:37:23 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:24 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:37:25 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:37:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f38da8d95f17de727ff64759972dbf1e6d887efe5f254506a23fd70ba3065b7`  
		Last Modified: Wed, 05 Oct 2022 04:40:26 GMT  
		Size: 3.8 MB (3765865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c10071d6f704357ec6b4fc90149ab1f0266bd2f859745ad5887b496563d5e88`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e117899982ab9f8600b6861f1440be605a7212c3ae586161375e0ed0b14fd34`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7957a4d09ef4cfcc2e4f9e8d9d980498ae723c0f2e087b7dd10975d4c6c3be`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 257.6 KB (257574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:e2fe15575f83678f39332da0326ecda80016d1dbcd9554b03b310060ec8f57bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32092294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeeffd42f7fc03ffc04e736fdcd562ad468ac2023453bc007b5cf158b1460a25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:57:59 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:00 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:01 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:08 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a74d96cddd31a9b0dcb858a34c9e4f2c2d1730679299ce66a44111af946c220`  
		Last Modified: Wed, 05 Oct 2022 04:02:08 GMT  
		Size: 3.6 MB (3593367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cab1a661086a3dc4eddc2627f2548445bd3185053ba7c024f9f03c9069e039`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c5bdf963687c93eca41e724d30263052cb0477c9b631dc4d14432142488855`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30638b5977520e4c36f1e8c72edd304b0be8f000dc6c349287ae1832ebb83b27`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 114.7 KB (114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:jammy-non-free`

```console
$ docker pull neurodebian@sha256:1668a100744dfe2a1dd0686735fd552f6de3c5d69427e6f5c1e581a15f215e69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:41e63dc24b0f7238288c4579f5cc7f6f7ed3b28bf31ff384ebf5206969dc4c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34454637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da2fb771ff149985fb315d4b17c331aba072267e0e64e8e23081387d09c9303`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:37:23 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:24 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:37:25 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:37:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:36 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f38da8d95f17de727ff64759972dbf1e6d887efe5f254506a23fd70ba3065b7`  
		Last Modified: Wed, 05 Oct 2022 04:40:26 GMT  
		Size: 3.8 MB (3765865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c10071d6f704357ec6b4fc90149ab1f0266bd2f859745ad5887b496563d5e88`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e117899982ab9f8600b6861f1440be605a7212c3ae586161375e0ed0b14fd34`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7957a4d09ef4cfcc2e4f9e8d9d980498ae723c0f2e087b7dd10975d4c6c3be`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 257.6 KB (257574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be700f0ad8ff547a7babb253a538c948ca0a27f3961a6505219a5df4d6e425cc`  
		Last Modified: Wed, 05 Oct 2022 04:40:34 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:836593c6bc4045f774a159231de968402fb6cb74c71b0a7831ea7166640fe03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32092550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50c75f4d5587a358e178e8aae43b140ef11fa08b92df691c11f3739ffea93ad0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:57:59 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:00 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:01 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:08 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a74d96cddd31a9b0dcb858a34c9e4f2c2d1730679299ce66a44111af946c220`  
		Last Modified: Wed, 05 Oct 2022 04:02:08 GMT  
		Size: 3.6 MB (3593367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cab1a661086a3dc4eddc2627f2548445bd3185053ba7c024f9f03c9069e039`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c5bdf963687c93eca41e724d30263052cb0477c9b631dc4d14432142488855`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30638b5977520e4c36f1e8c72edd304b0be8f000dc6c349287ae1832ebb83b27`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 114.7 KB (114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d97faa1fa50fd30713bd4d7d1f5eda0123ce7a0b310dcac4ca92093e8040296`  
		Last Modified: Wed, 05 Oct 2022 04:02:18 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:2661841f96cd443d306b51d0d63a018642c1d31667dbb10df5e6160a7188cbf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:64f51985744c09f1eece661c9b0fae45e93716af39ca647cccd567a2271bc25d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66670584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98be26081cb0e38c2b3c1b3be93c7fd4165d11982e16c058f60bdbc9f906ef85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:05 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:06 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:07 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59519a823826166b6d39d758ec5014bd2a5a294b254600d211895dd9c5a866a`  
		Last Modified: Wed, 05 Oct 2022 04:41:04 GMT  
		Size: 11.3 MB (11310722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ec2e5570ce1fabd90c3f195db1c2491485e03dfbaa959a752acc6de8c4641`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f97d5eff53b93eef2dcda043176e5b2ad126bb890a82dd2f405b0f9fe26f5c7`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3860fd5292dee9ad38ed40b5bab9706f31cf24d1663060f1cda46eb7d4856cc8`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 311.6 KB (311600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:549507692b43319c3085c66c184331a3690843651c9856f1f1a451b2822abb7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64912635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3771988b0944a19a09d4efadebfc7d8a9cfbb1195dbd0f65a981d082e17e6c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:54 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32748b0f6967d6d3a663ec439e7a0b631ffe7f6e19fe0a854fa9f60cfbd8013`  
		Last Modified: Wed, 05 Oct 2022 04:02:54 GMT  
		Size: 11.1 MB (11104845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2cd3f4776c95e95f8cf2fe1866ba88b1f93d61bd9cf77c2b0454c13231a54`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74195093fe58a8f1f862fdb46f29db25a349b6d544a17872538f43ed9f69314`  
		Last Modified: Wed, 05 Oct 2022 04:02:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bb772dba620ade3ee2ee0b39ede83b9e4e52271a3c735aea72ebe200c60d9a`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 105.2 KB (105178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; 386

```console
$ docker pull neurodebian@sha256:faad9fd73720614aa3571453130adab314a1337233c23716ea029d9c8f2f5262
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67630593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82bebd1ae720b0a3624a349c8605a9c423db494f38f028eddfdfc8e500ab3db9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1913722e4098b05a88200af242b3e4de75036431d863b1330ca708cec7d52fda`  
		Last Modified: Wed, 05 Oct 2022 02:17:23 GMT  
		Size: 11.5 MB (11499735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16eddaf2626ebe571c30e863702e069074b6e5a9a22488db55e5d6dfdb41fdf8`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b6358b663dae0a2653ca7146baf655ba0e0e1b765ac7cc2914cdcc4390ea7b`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2069c1e6d4aa4c4d2b785d1396e8487db0a8e83ff092b0fae2d0454a2d6b9a2`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 105.1 KB (105067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:0ab19f9f980c6751be623ec2b81ff301f97899d29bdee08dd10aa725ad5960a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:e6909af965ce64be8f6b1c0f32bb6cfd9e6c57b84ebb544b4a32fdbe56a2dc76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64736983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e431e3a9fc2aae9fc0a48164bcff057e00b97976b328292ef893731c9d07ccf4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:54 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c974a6c61f45043e129e219d4381fa099db2e7a173f61912a8982e579a6fe4c`  
		Last Modified: Wed, 05 Oct 2022 04:41:48 GMT  
		Size: 11.8 MB (11764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722be9facb8de2d4f538cbaa389186d6bbd281727551826bf6df7c7e4792928`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cb23dd2e6424a119cad9e202ce4f86217edd6a42e57c86cf5af490f2086ef2`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0d634f74a911a7f3b806dda7044fdbba550ec77c0a9b1d02e6c4d91b97bfc7`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 285.7 KB (285728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:606fe2624ff9d573725a337157db984416d1c306f5902bfb084818a3486d5f5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64331879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcca08c9aa4f00502bf9002fe0c8d93d67c00042c3e9b5de049a083af432b0d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:47 GMT
ADD file:28797d8b43689eae5ccab5b01e88b732a5fca655590a0c9f066d6f0a4d880a95 in / 
# Tue, 04 Oct 2022 23:45:48 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:59:44 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:59:49 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6499ab100dbfb0305e0d96b62f7ad515906275ab30864ac686f0af8ff2fdd114`  
		Last Modified: Tue, 04 Oct 2022 23:52:17 GMT  
		Size: 52.7 MB (52699991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df1adfecab1461b8bd99768350d329ebd6e7b7f5e62880f44688fa052d81ee5`  
		Last Modified: Wed, 05 Oct 2022 04:03:49 GMT  
		Size: 11.5 MB (11532459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211df1c3633aa1661947564b9ed3696aa1124f6f50b0f8f3b5955b1375b7edc9`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae2e7a8e83e699919e6d0b01c2018d0aa2bab3c68163dd11674788e3045521d`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c48121c4388703126d8476e2c0db10a4f0e3fe3b6cf4b0c6c837990718ec487`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 97.4 KB (97449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; 386

```console
$ docker pull neurodebian@sha256:723fcb4319dc470a62adb2c3765720692d48d6ac68a243dbbb4b078135f63508
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65738969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288db7a1ad4289391574ac79c607ffdc110abea480167360cec2bd805154eefd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:40:48 GMT
ADD file:ea6d247c762f6294c87144d1a4308c30669e9e732bd8ff9ef892c71d14563165 in / 
# Tue, 04 Oct 2022 23:40:49 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:16:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:16:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:16:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:16:10 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a0d07a7940ebb4ded014cd2eaedc6b9aa8767ff5afeee7b1b09fce7cbd7a31e`  
		Last Modified: Tue, 04 Oct 2022 23:47:29 GMT  
		Size: 53.6 MB (53647464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ef37d1ca044b99973bac8a03dd842b017b7e1459194239fd83e9dd188597c`  
		Last Modified: Wed, 05 Oct 2022 02:18:16 GMT  
		Size: 12.0 MB (11992190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7bb9a78d2d85b84ec9ffbfb13e408d286021108c33addfecf65bcc2993839`  
		Last Modified: Wed, 05 Oct 2022 02:18:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994eb0042ba9c275a2f107edab9fd532d71c9a01c5addf5d4966600e9bac59b3`  
		Last Modified: Wed, 05 Oct 2022 02:18:14 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d19a641e13b51478bf8e07a69c870d20f5b6988a813cb8082a4e0636567fa19`  
		Last Modified: Wed, 05 Oct 2022 02:18:15 GMT  
		Size: 97.3 KB (97327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:f98a8c574d13705de4d08216b4585180142412d7251b6c34faf53a1ad5d1ea1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:307e1ad9ad2e2ab3c6aa952f25e895043099dbcc0f7d4339d18d0fd481268348
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64737377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32ea95e69fcf6ee1d5ee097e66f41450ef87e137e8a039a2a89b95a06ed804f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:54 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:39:04 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c974a6c61f45043e129e219d4381fa099db2e7a173f61912a8982e579a6fe4c`  
		Last Modified: Wed, 05 Oct 2022 04:41:48 GMT  
		Size: 11.8 MB (11764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722be9facb8de2d4f538cbaa389186d6bbd281727551826bf6df7c7e4792928`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cb23dd2e6424a119cad9e202ce4f86217edd6a42e57c86cf5af490f2086ef2`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0d634f74a911a7f3b806dda7044fdbba550ec77c0a9b1d02e6c4d91b97bfc7`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 285.7 KB (285728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96912c6f77059af0f7694c93d65d843d899967826d2ba9fa69d481f27864ddc0`  
		Last Modified: Wed, 05 Oct 2022 04:41:57 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:47635762f344317598dce2e4bb4b293c55808ffcf013957b1e17246722503bd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64332274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60878ab35485605801fe9972a19002148644695e6ace672c1675fc53331a90da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:47 GMT
ADD file:28797d8b43689eae5ccab5b01e88b732a5fca655590a0c9f066d6f0a4d880a95 in / 
# Tue, 04 Oct 2022 23:45:48 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:59:44 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:59:49 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:55 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6499ab100dbfb0305e0d96b62f7ad515906275ab30864ac686f0af8ff2fdd114`  
		Last Modified: Tue, 04 Oct 2022 23:52:17 GMT  
		Size: 52.7 MB (52699991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df1adfecab1461b8bd99768350d329ebd6e7b7f5e62880f44688fa052d81ee5`  
		Last Modified: Wed, 05 Oct 2022 04:03:49 GMT  
		Size: 11.5 MB (11532459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211df1c3633aa1661947564b9ed3696aa1124f6f50b0f8f3b5955b1375b7edc9`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae2e7a8e83e699919e6d0b01c2018d0aa2bab3c68163dd11674788e3045521d`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c48121c4388703126d8476e2c0db10a4f0e3fe3b6cf4b0c6c837990718ec487`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 97.4 KB (97449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a122987277c618f99d8e9797c12f5554f3e292599645081a8d40ceb2a5e6f6`  
		Last Modified: Wed, 05 Oct 2022 04:04:00 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:a425770283cda772573807278c0b8b6f038f76ca2dd620354fe49d4ae381080e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65739361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b0b187a067e370c9357a6f1f6a7eefc3e0ed25daf17f316e3b9b537ba736c3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:40:48 GMT
ADD file:ea6d247c762f6294c87144d1a4308c30669e9e732bd8ff9ef892c71d14563165 in / 
# Tue, 04 Oct 2022 23:40:49 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:16:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:16:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:16:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:16:10 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:16:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:8a0d07a7940ebb4ded014cd2eaedc6b9aa8767ff5afeee7b1b09fce7cbd7a31e`  
		Last Modified: Tue, 04 Oct 2022 23:47:29 GMT  
		Size: 53.6 MB (53647464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ef37d1ca044b99973bac8a03dd842b017b7e1459194239fd83e9dd188597c`  
		Last Modified: Wed, 05 Oct 2022 02:18:16 GMT  
		Size: 12.0 MB (11992190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7bb9a78d2d85b84ec9ffbfb13e408d286021108c33addfecf65bcc2993839`  
		Last Modified: Wed, 05 Oct 2022 02:18:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994eb0042ba9c275a2f107edab9fd532d71c9a01c5addf5d4966600e9bac59b3`  
		Last Modified: Wed, 05 Oct 2022 02:18:14 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d19a641e13b51478bf8e07a69c870d20f5b6988a813cb8082a4e0636567fa19`  
		Last Modified: Wed, 05 Oct 2022 02:18:15 GMT  
		Size: 97.3 KB (97327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db70b4bbb814cec277b2bbd389ec555efbbf4fb63b356046e21eca8518708d`  
		Last Modified: Wed, 05 Oct 2022 02:18:26 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100`

```console
$ docker pull neurodebian@sha256:704d61176624378d00d12746b1e028e1973852c3ff9789f09201f41b177e535b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100` - linux; amd64

```console
$ docker pull neurodebian@sha256:bac54f40a6dd681e8e608373b4938df13f0b3b3344aa9d33b50c60e2205b54be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61247541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:689b0d51aee9386015685a93d96881629b22b1ae333beb6d77c361cc6b7bc78c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:37:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:37:47 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:37:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a98ad9d5bfe5c93cdc5dd566aa7c846123d6b674612d8c22ce6c4506a1c72d`  
		Last Modified: Wed, 05 Oct 2022 04:40:45 GMT  
		Size: 10.5 MB (10501516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a8bc5b640eb70d850ea36e9b51ae7b8fc76946e82ae1bb0642d47f0e0eb73`  
		Last Modified: Wed, 05 Oct 2022 04:40:44 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f286e51e987b82a169deb249e7d1398676dca1955e72e0976dc9302cfe8b7a`  
		Last Modified: Wed, 05 Oct 2022 04:40:43 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0eb25a875218ed1b804497338449bbaeb2129f8647aec7695c8ef06e71cad`  
		Last Modified: Wed, 05 Oct 2022 04:40:44 GMT  
		Size: 302.9 KB (302910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:2dc6d3c83993dc6a49fc286f9a1d6110258197edb1d3cacabec8b12d88d4becf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59636797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b50a8e93e8303cee10538cc56493e6e180c31a069561b078b566065bc62aca2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:28 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d154496b8ab72771340bbbfcb90129abefba06a0df134e694e436c32723ecf`  
		Last Modified: Wed, 05 Oct 2022 04:02:31 GMT  
		Size: 10.3 MB (10297436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef89a9a6d8113e10f9e579ee92783e306a5fa8bfe2acfa01e2d78d7fd818107f`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23704a18d02fdbc4131c6f7adfaaec3730093c5504d02a143c4a78f637028721`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d322400769bb470d58b21b11c9f6e84fb73d5e8603c40127b4804943ec7f7ec2`  
		Last Modified: Wed, 05 Oct 2022 04:02:30 GMT  
		Size: 108.5 KB (108492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100` - linux; 386

```console
$ docker pull neurodebian@sha256:1fd4cf8b2a55d0059c7adddd50e16ea9c0b91e97458079defd08db84607e50a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61982452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4611172bd93ea6abd33eb27f96eeb688a884c754e831b30d565524925f180742`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:52 GMT
ADD file:887aa5460e148ba204780ebe976e5627d5f4d0a07faf22b86afe146998d75d79 in / 
# Tue, 04 Oct 2022 23:39:53 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:14:43 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:14:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:14:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:14:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:98d78922e3457a6697f2cdbddaab27dbb47e2e0beedb1a4348c56102c850b343`  
		Last Modified: Tue, 04 Oct 2022 23:45:58 GMT  
		Size: 51.2 MB (51202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a1c4ae5a735b6da355e52d679127188fc0385520109eb7c93e31b0fd3a7c5`  
		Last Modified: Wed, 05 Oct 2022 02:17:01 GMT  
		Size: 10.7 MB (10669155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127af1b441210177fdedbe41dc0aaf6ca644be580c15ae7a5cae51e8ff1bffce`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8999f6b03a0580644ff4a8ada4dec6b0d39eec0f624022a1b96f832f8fd28a21`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5c07173b4dcb13dbcc2b4c04cdbb7546fb67e2b14f21eea7653356ac3845ba`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 108.5 KB (108467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:1b8e6b396dd099b61e36a2b19d6900f814d81510c418f42a1d5cebf15aefd42a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:a2e3e436f3774637fecc2d35630111123e5ae75ba23ba63e83d57401b729b454
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61247897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d329a9df499d0dc0b3386b4766c5be22661ce5105b8fcf90606746add3e6bfec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:37:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:37:47 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:37:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:56 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a98ad9d5bfe5c93cdc5dd566aa7c846123d6b674612d8c22ce6c4506a1c72d`  
		Last Modified: Wed, 05 Oct 2022 04:40:45 GMT  
		Size: 10.5 MB (10501516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a8bc5b640eb70d850ea36e9b51ae7b8fc76946e82ae1bb0642d47f0e0eb73`  
		Last Modified: Wed, 05 Oct 2022 04:40:44 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f286e51e987b82a169deb249e7d1398676dca1955e72e0976dc9302cfe8b7a`  
		Last Modified: Wed, 05 Oct 2022 04:40:43 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0eb25a875218ed1b804497338449bbaeb2129f8647aec7695c8ef06e71cad`  
		Last Modified: Wed, 05 Oct 2022 04:40:44 GMT  
		Size: 302.9 KB (302910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534645635d433d322d0e0a9f9eb06a9ea23d56fd282b1576d7af7234e822cba0`  
		Last Modified: Wed, 05 Oct 2022 04:40:54 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:ae50d50c11c32068f7b0f868f8975041e8cc6381108233aa6926e8f2b4dbb863
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59637153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e1ca9d0cf271394b943e6c4dbc574cc3b61dbe9eed4fa82dbd4e4feaf92085c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:28 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:40 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d154496b8ab72771340bbbfcb90129abefba06a0df134e694e436c32723ecf`  
		Last Modified: Wed, 05 Oct 2022 04:02:31 GMT  
		Size: 10.3 MB (10297436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef89a9a6d8113e10f9e579ee92783e306a5fa8bfe2acfa01e2d78d7fd818107f`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23704a18d02fdbc4131c6f7adfaaec3730093c5504d02a143c4a78f637028721`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d322400769bb470d58b21b11c9f6e84fb73d5e8603c40127b4804943ec7f7ec2`  
		Last Modified: Wed, 05 Oct 2022 04:02:30 GMT  
		Size: 108.5 KB (108492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ebd81db9bac845b1da95a5029d74042c0045701de4248a1c4a035311b28efe`  
		Last Modified: Wed, 05 Oct 2022 04:02:41 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:fa77adad3506f7d86dae7b6965fe84a271c03357bb0d6a0a88cfcf84d9c5aec1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61982810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d524cf15f421c47fa01d99d0e92e1d401e54ffefa9ea0aec36d56ddd527a0e09`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:52 GMT
ADD file:887aa5460e148ba204780ebe976e5627d5f4d0a07faf22b86afe146998d75d79 in / 
# Tue, 04 Oct 2022 23:39:53 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:14:43 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:14:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:14:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:14:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:14:56 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:98d78922e3457a6697f2cdbddaab27dbb47e2e0beedb1a4348c56102c850b343`  
		Last Modified: Tue, 04 Oct 2022 23:45:58 GMT  
		Size: 51.2 MB (51202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a1c4ae5a735b6da355e52d679127188fc0385520109eb7c93e31b0fd3a7c5`  
		Last Modified: Wed, 05 Oct 2022 02:17:01 GMT  
		Size: 10.7 MB (10669155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127af1b441210177fdedbe41dc0aaf6ca644be580c15ae7a5cae51e8ff1bffce`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8999f6b03a0580644ff4a8ada4dec6b0d39eec0f624022a1b96f832f8fd28a21`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5c07173b4dcb13dbcc2b4c04cdbb7546fb67e2b14f21eea7653356ac3845ba`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 108.5 KB (108467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a0b36a65a1c2c95edc9bf80ee22743a8f9009433ee1c689bb97051f7899e85`  
		Last Modified: Wed, 05 Oct 2022 02:17:11 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110`

```console
$ docker pull neurodebian@sha256:2661841f96cd443d306b51d0d63a018642c1d31667dbb10df5e6160a7188cbf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110` - linux; amd64

```console
$ docker pull neurodebian@sha256:64f51985744c09f1eece661c9b0fae45e93716af39ca647cccd567a2271bc25d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66670584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98be26081cb0e38c2b3c1b3be93c7fd4165d11982e16c058f60bdbc9f906ef85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:05 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:06 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:07 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59519a823826166b6d39d758ec5014bd2a5a294b254600d211895dd9c5a866a`  
		Last Modified: Wed, 05 Oct 2022 04:41:04 GMT  
		Size: 11.3 MB (11310722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ec2e5570ce1fabd90c3f195db1c2491485e03dfbaa959a752acc6de8c4641`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f97d5eff53b93eef2dcda043176e5b2ad126bb890a82dd2f405b0f9fe26f5c7`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3860fd5292dee9ad38ed40b5bab9706f31cf24d1663060f1cda46eb7d4856cc8`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 311.6 KB (311600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:549507692b43319c3085c66c184331a3690843651c9856f1f1a451b2822abb7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64912635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3771988b0944a19a09d4efadebfc7d8a9cfbb1195dbd0f65a981d082e17e6c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:54 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32748b0f6967d6d3a663ec439e7a0b631ffe7f6e19fe0a854fa9f60cfbd8013`  
		Last Modified: Wed, 05 Oct 2022 04:02:54 GMT  
		Size: 11.1 MB (11104845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2cd3f4776c95e95f8cf2fe1866ba88b1f93d61bd9cf77c2b0454c13231a54`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74195093fe58a8f1f862fdb46f29db25a349b6d544a17872538f43ed9f69314`  
		Last Modified: Wed, 05 Oct 2022 04:02:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bb772dba620ade3ee2ee0b39ede83b9e4e52271a3c735aea72ebe200c60d9a`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 105.2 KB (105178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110` - linux; 386

```console
$ docker pull neurodebian@sha256:faad9fd73720614aa3571453130adab314a1337233c23716ea029d9c8f2f5262
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67630593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82bebd1ae720b0a3624a349c8605a9c423db494f38f028eddfdfc8e500ab3db9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1913722e4098b05a88200af242b3e4de75036431d863b1330ca708cec7d52fda`  
		Last Modified: Wed, 05 Oct 2022 02:17:23 GMT  
		Size: 11.5 MB (11499735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16eddaf2626ebe571c30e863702e069074b6e5a9a22488db55e5d6dfdb41fdf8`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b6358b663dae0a2653ca7146baf655ba0e0e1b765ac7cc2914cdcc4390ea7b`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2069c1e6d4aa4c4d2b785d1396e8487db0a8e83ff092b0fae2d0454a2d6b9a2`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 105.1 KB (105067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:f0db759e1632d1225899599cce0dfb1562c8d3b39e20cddd98cdbf6055681840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:429703f7e0fee449ecf50ab4cc0361f089ca009722e969ee67d2cd0359c2b297
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66670946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95b57e27da6390014efb505383ed7bcf2053334cc51e76b3a2dbef13db3e7ebb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:05 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:06 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:07 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59519a823826166b6d39d758ec5014bd2a5a294b254600d211895dd9c5a866a`  
		Last Modified: Wed, 05 Oct 2022 04:41:04 GMT  
		Size: 11.3 MB (11310722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ec2e5570ce1fabd90c3f195db1c2491485e03dfbaa959a752acc6de8c4641`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f97d5eff53b93eef2dcda043176e5b2ad126bb890a82dd2f405b0f9fe26f5c7`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3860fd5292dee9ad38ed40b5bab9706f31cf24d1663060f1cda46eb7d4856cc8`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 311.6 KB (311600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3f2699fcf96f4273335b294c96598796754d1f07e7247bae8bdee5bc4a2e84`  
		Last Modified: Wed, 05 Oct 2022 04:41:16 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:6f6e001cebd2e7dc0a6dcdfac69f62ae40db3ad5a27873ceb5dcbdaa656bad5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64912994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a33532c39658d75d58079d13e51642f56eeac73e1fa42bd67e5e54408cd59f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:54 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:05 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32748b0f6967d6d3a663ec439e7a0b631ffe7f6e19fe0a854fa9f60cfbd8013`  
		Last Modified: Wed, 05 Oct 2022 04:02:54 GMT  
		Size: 11.1 MB (11104845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2cd3f4776c95e95f8cf2fe1866ba88b1f93d61bd9cf77c2b0454c13231a54`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74195093fe58a8f1f862fdb46f29db25a349b6d544a17872538f43ed9f69314`  
		Last Modified: Wed, 05 Oct 2022 04:02:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bb772dba620ade3ee2ee0b39ede83b9e4e52271a3c735aea72ebe200c60d9a`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 105.2 KB (105178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe1986c4b98c09310059dfffefb45f157872b7f5c09d1d2d4c4a68e3acfb272`  
		Last Modified: Wed, 05 Oct 2022 04:03:08 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:49bec358473d52c6911c4c6deae5298035893c9faf0b40a00f42e315e067caa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67630953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d31e9115c7ef837ee295344dd83e413d4164b55f4a4b8fb32836479f79316ebf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1913722e4098b05a88200af242b3e4de75036431d863b1330ca708cec7d52fda`  
		Last Modified: Wed, 05 Oct 2022 02:17:23 GMT  
		Size: 11.5 MB (11499735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16eddaf2626ebe571c30e863702e069074b6e5a9a22488db55e5d6dfdb41fdf8`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b6358b663dae0a2653ca7146baf655ba0e0e1b765ac7cc2914cdcc4390ea7b`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2069c1e6d4aa4c4d2b785d1396e8487db0a8e83ff092b0fae2d0454a2d6b9a2`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 105.1 KB (105067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fcc7395aa5a726c6a498dace0389db7c1a51fa808ba67dfecf838c90d83dd7`  
		Last Modified: Wed, 05 Oct 2022 02:17:37 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120`

```console
$ docker pull neurodebian@sha256:79ed50d7fea07cb407771e5be79af216bb69c992b9535d126ad02e9d298536cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120` - linux; amd64

```console
$ docker pull neurodebian@sha256:80e495f56a8237c8cfa8e2e3b3dd9e54a505a4f883d316a4240a21b7041aecb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65014055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a3ff4e52f917a5a8d864f577fa58cbf9cfc295b40f922b27828012fb5cf890`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:36 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2316c52551cab9cc0ad9166bc77e216033702e8aaabffc0abcfb89f136d8c76`  
		Last Modified: Wed, 05 Oct 2022 04:41:29 GMT  
		Size: 11.8 MB (11764299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe69058d31d6cd9481204bc8bf1336732437d0660a1d75e5f65767c22a94bb9`  
		Last Modified: Wed, 05 Oct 2022 04:41:27 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87205a6c66a4f8e9f0acef27904269125540931696cbeef7b33f8df121ac2edd`  
		Last Modified: Wed, 05 Oct 2022 04:41:27 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8368ed01254e7fabcaccc37943c9d4b1b860ee0375ed75e45c834a9c52ade31`  
		Last Modified: Wed, 05 Oct 2022 04:41:28 GMT  
		Size: 285.3 KB (285329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:04b205e6757ccaee181d6b9df9a36655883160250f742d021117a3a1b1cfff4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64610344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a08ab62e18104657885408c27ceefaa2eab492b53f852b8affb14b0c2faa55`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:00 GMT
ADD file:269c8bec4871d84b9133706a2f391209619d53c0bfa56121c740757cf5798fcb in / 
# Tue, 04 Oct 2022 23:44:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:59:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:59:23 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2debf9e7f23054c81a936da9b01c5db9f72a55d4810f7bf0e5641bd1748d90b7`  
		Last Modified: Tue, 04 Oct 2022 23:49:11 GMT  
		Size: 53.0 MB (52980389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0ef51f5528c6564ff374a45d9cb4c4c6eaf535c3565cbb4ba763bc55b22343`  
		Last Modified: Wed, 05 Oct 2022 04:03:24 GMT  
		Size: 11.5 MB (11531064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469c79e490be5fc87427c713b2cff0a58e2d249f09613ea11f6d6a02ed9e62f7`  
		Last Modified: Wed, 05 Oct 2022 04:03:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a22ac0a033238596c38df2f9af0747aa62ed9470c2a82f61ed8978d6ccc5f`  
		Last Modified: Wed, 05 Oct 2022 04:03:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bc59e065b02635051c28a8a2b68751fbdc3486f83ce39b848da35674d67b13`  
		Last Modified: Wed, 05 Oct 2022 04:03:23 GMT  
		Size: 96.9 KB (96904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120` - linux; 386

```console
$ docker pull neurodebian@sha256:73316bae3c4e7a4271e81a96da0a8a0cb7c42d32b91c42c8d4ba42585d386780
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66022618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:618ae15fc21beb4669f25359429e3e4605519f66976d8c64d6879fa894af89e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:38:57 GMT
ADD file:2a0c743e373aeed6462c2f3ae8a138fb0e240e935ad7ca5bf008aa3efd3673a0 in / 
# Tue, 04 Oct 2022 23:38:58 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68776dad61a299b8e65d1a6a02e376b8ed2e9b241bd753bf6c35d497055ecdf`  
		Last Modified: Tue, 04 Oct 2022 23:44:23 GMT  
		Size: 53.9 MB (53932827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b23a7101cec8d64ddc2337801957f17d5366b0725dfb359c4a75a69d6a5e59b`  
		Last Modified: Wed, 05 Oct 2022 02:17:53 GMT  
		Size: 12.0 MB (11990988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bc6ea3e1edb50b087a2d132755dd424f332df905fd3ca53fc106283fa89192`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f7492185dc14c52e2b31a59607eac615a02bb456adcdd05c611ea2b460da27`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156209dfa890bcc23c8e351f1f08baad61399ccb713ea04a5f81e3d9a8d3760a`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 96.8 KB (96816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:e824689fd765e6636fd053b8640c6c796089ca812aedeae435886e5b5368b67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:bd5355676c5af8e531fbb1f95cb73c50e8aded59a5bbd628ba410ab609d423a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65014415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54479f492559d1e663f6669b2c7233f7cdea30f616c8fcdfe326d874ebec17a7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:36 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:42 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2316c52551cab9cc0ad9166bc77e216033702e8aaabffc0abcfb89f136d8c76`  
		Last Modified: Wed, 05 Oct 2022 04:41:29 GMT  
		Size: 11.8 MB (11764299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe69058d31d6cd9481204bc8bf1336732437d0660a1d75e5f65767c22a94bb9`  
		Last Modified: Wed, 05 Oct 2022 04:41:27 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87205a6c66a4f8e9f0acef27904269125540931696cbeef7b33f8df121ac2edd`  
		Last Modified: Wed, 05 Oct 2022 04:41:27 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8368ed01254e7fabcaccc37943c9d4b1b860ee0375ed75e45c834a9c52ade31`  
		Last Modified: Wed, 05 Oct 2022 04:41:28 GMT  
		Size: 285.3 KB (285329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca0c4df391b41681b1f4c8259b14ac54ae55eaca35fa4729063e3b06d85119`  
		Last Modified: Wed, 05 Oct 2022 04:41:37 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:9fb15b3ee57c8ecf0c6fad7fbc5ce41d2124d2363d6d2532d4c74192ed6f5e4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64610704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a146677dea1903a8763fe0202bdc02ac58275e1db107f7d1a45d48d360d56b1a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:00 GMT
ADD file:269c8bec4871d84b9133706a2f391209619d53c0bfa56121c740757cf5798fcb in / 
# Tue, 04 Oct 2022 23:44:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:17 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:59:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:59:23 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:30 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:2debf9e7f23054c81a936da9b01c5db9f72a55d4810f7bf0e5641bd1748d90b7`  
		Last Modified: Tue, 04 Oct 2022 23:49:11 GMT  
		Size: 53.0 MB (52980389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0ef51f5528c6564ff374a45d9cb4c4c6eaf535c3565cbb4ba763bc55b22343`  
		Last Modified: Wed, 05 Oct 2022 04:03:24 GMT  
		Size: 11.5 MB (11531064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469c79e490be5fc87427c713b2cff0a58e2d249f09613ea11f6d6a02ed9e62f7`  
		Last Modified: Wed, 05 Oct 2022 04:03:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a22ac0a033238596c38df2f9af0747aa62ed9470c2a82f61ed8978d6ccc5f`  
		Last Modified: Wed, 05 Oct 2022 04:03:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bc59e065b02635051c28a8a2b68751fbdc3486f83ce39b848da35674d67b13`  
		Last Modified: Wed, 05 Oct 2022 04:03:23 GMT  
		Size: 96.9 KB (96904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86addfd21f29a2b3cc2f2d4caa2e71233a7f3263674e19b65321fcf5e03cc560`  
		Last Modified: Wed, 05 Oct 2022 04:03:36 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:a0419b3921c4500ce8017f99b534dd4c66e6641fdd63cf8d17d36a607b17dead
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66022979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee04776b466810c25260cd640d93dd96840d94e5bf91857e004aa6b5f454b5c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:38:57 GMT
ADD file:2a0c743e373aeed6462c2f3ae8a138fb0e240e935ad7ca5bf008aa3efd3673a0 in / 
# Tue, 04 Oct 2022 23:38:58 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:50 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c68776dad61a299b8e65d1a6a02e376b8ed2e9b241bd753bf6c35d497055ecdf`  
		Last Modified: Tue, 04 Oct 2022 23:44:23 GMT  
		Size: 53.9 MB (53932827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b23a7101cec8d64ddc2337801957f17d5366b0725dfb359c4a75a69d6a5e59b`  
		Last Modified: Wed, 05 Oct 2022 02:17:53 GMT  
		Size: 12.0 MB (11990988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bc6ea3e1edb50b087a2d132755dd424f332df905fd3ca53fc106283fa89192`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f7492185dc14c52e2b31a59607eac615a02bb456adcdd05c611ea2b460da27`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156209dfa890bcc23c8e351f1f08baad61399ccb713ea04a5f81e3d9a8d3760a`  
		Last Modified: Wed, 05 Oct 2022 02:17:51 GMT  
		Size: 96.8 KB (96816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e038e92cc95c6ee9d08edbfccb0fd01d6cc3153d445b6ea5717491f57216b426`  
		Last Modified: Wed, 05 Oct 2022 02:18:04 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd16.04`

```console
$ docker pull neurodebian@sha256:c179df88528644a2b2b5df8f22b96dcab0bff5c4d61f7ac2ec80d06a648262db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd16.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:d80e83bfcc000dd04b02c778a1297c7ad2540cb555ab96c90ec154c6a4f0f495
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60902017c278b0db41b17f8f1de27469127d1ea4898b2469f52647585af6120`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:57:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Mar 2022 17:27:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 16 Mar 2022 17:27:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 16 Mar 2022 17:27:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84732b274efc4bdfc5e30a12f05cbd1a9936e3ed5e8952879d6ee935df35eb79`  
		Last Modified: Tue, 31 Aug 2021 04:00:24 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3505bfdde8eb1415423d95064ff6b92c835526022feb1d95009ab5ec04c115`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3fae1c80c2541f9a1f6a2df3ea6faa8f5c9797dda86103383518675981d44`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a78747ad8c43a648a10d04a1c586defca6040cc6c5a4acf404d3962d361631a`  
		Last Modified: Wed, 16 Mar 2022 17:35:35 GMT  
		Size: 227.0 KB (226984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd16.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:0b3d5b0cf4235e5ee1e5a25a0e659b44dd6601d4e870e3ca8bead4d37b9cd648
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41341574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed5da098fa1d015a6450f26d7b085d457c2b01a8b427f2d30849343a381e4ca7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Tue, 19 Jul 2022 19:54:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:54:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 19:54:18 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 21:48:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2aeaf3b81eb7fe1658089024c39952f34ea97c9eaff622b60582fbcd51d8f13`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 3.1 KB (3129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3469adcab4ca9a0392e6f6a8101969d54921e20ad79c2f70df00b7a84f6777e0`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d8dd7eaecc8c7cb61334bd81c2c47c8779b4b04668561f1b1caefd019a4b5`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 97.5 KB (97452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd16.04-non-free`

```console
$ docker pull neurodebian@sha256:a9b79b3f807f716014321b46bafc911ed4b0df804d137f9e5cbef226c5173a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd16.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:855db2a2543daaf4e085777944831f96ea7a6212d2231da7614dcb717c8a6df4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c4860f282209b4ea6a5dfd24af70a0307b7664484b8a5bb97070973e934e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:57:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Mar 2022 17:27:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 16 Mar 2022 17:27:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 16 Mar 2022 17:27:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:53:37 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84732b274efc4bdfc5e30a12f05cbd1a9936e3ed5e8952879d6ee935df35eb79`  
		Last Modified: Tue, 31 Aug 2021 04:00:24 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3505bfdde8eb1415423d95064ff6b92c835526022feb1d95009ab5ec04c115`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3fae1c80c2541f9a1f6a2df3ea6faa8f5c9797dda86103383518675981d44`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a78747ad8c43a648a10d04a1c586defca6040cc6c5a4acf404d3962d361631a`  
		Last Modified: Wed, 16 Mar 2022 17:35:35 GMT  
		Size: 227.0 KB (226984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb28ad0e4efee889c9e9363676830fcc3b2a6b15e7dbd41af4f1c4241f7c5ba`  
		Last Modified: Tue, 19 Jul 2022 19:56:32 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd16.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:020707ea4d325b1a95493865742e9fee81f8252f97090141fced8bc788725e39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41341831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d824467043c6d70fbe5679704bf4275178249cffe0b0408e0802cd9f9ddd1d5c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Tue, 19 Jul 2022 19:54:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:54:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 19:54:18 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 21:48:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 21:48:10 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2aeaf3b81eb7fe1658089024c39952f34ea97c9eaff622b60582fbcd51d8f13`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 3.1 KB (3129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3469adcab4ca9a0392e6f6a8101969d54921e20ad79c2f70df00b7a84f6777e0`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d8dd7eaecc8c7cb61334bd81c2c47c8779b4b04668561f1b1caefd019a4b5`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 97.5 KB (97452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c2010d9b79b1282b1d8f21875e4010b844f2a3c31af5ab9a1a7c039c85bac`  
		Last Modified: Tue, 19 Jul 2022 21:51:38 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04`

```console
$ docker pull neurodebian@sha256:4beab2d9de10f5c74669b7aad7fe9c38a0ca77109ce16e33e2cf46a6bdbe1fe8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd18.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:a4563092987a9094f629e918b696638826ac17270d6e4b4844c943cbacdf8c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31769449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6c5a3eb19316317ceea7d7dd57d8206854e2c096749ec0163c48ffcf59d4b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:35:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:35:52 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:35:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:35:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b326536d9135ba21a7d81e94b00d7908a0e98db7443d55decaace2cadae22f`  
		Last Modified: Wed, 05 Oct 2022 04:39:47 GMT  
		Size: 4.8 MB (4815599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfeae315539086179fc071cd4f1866e8c8d38765cf68e5832d07bdb7388fdc8`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7ceb3ac42fa70ccfe5e470e0efc92d4b1c90e54fcdaf9a451bacc6107bd91f`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca5b1ce88f0b3604342d8ec51ae31e8d9af4dde0b98e0e039eebd8ede5a78fa`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 240.1 KB (240089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd18.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:3106ed7f09960a95ba5d9da7894ddd0272aed0a27baaf35acde7b4387ec53d87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28107422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a836588eaf2b8b33d9904fa7774955073c4c6f56baa00c908b948876ad437cbf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:56:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:56:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:56:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:56:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415982c552b3097dc0f0e3fdab4c2932671fee8d829436501ccb051e6eb83500`  
		Last Modified: Wed, 05 Oct 2022 04:01:19 GMT  
		Size: 4.3 MB (4263811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521f05b326e0e79919ca42ac9a0c47cb9f1caeffc488a7c889282f7fdc7783ab`  
		Last Modified: Wed, 05 Oct 2022 04:01:18 GMT  
		Size: 1.6 KB (1639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea2e867535975d3209819774df2886ba41c121200bbe2c7d447a1e76754391`  
		Last Modified: Wed, 05 Oct 2022 04:01:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53cf70e35b0e254b43fe67021ea0499f47207b931b8d33c35d44b684e86ce1d`  
		Last Modified: Wed, 05 Oct 2022 04:01:18 GMT  
		Size: 107.1 KB (107134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04-non-free`

```console
$ docker pull neurodebian@sha256:121585e3ab450a44b229835895f4517a1e4ea0a29a5661aa743f1cab99064509
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd18.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:241e8b93af0e677ab1c024ab6e004344c3591193a9be7ae6ce029c5bae66f2d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31769706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4758b5a325ceebffec9976a3a336b62594cea44d24465903f9db4e780d72c4f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:35:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:35:52 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:35:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:35:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:36:06 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b326536d9135ba21a7d81e94b00d7908a0e98db7443d55decaace2cadae22f`  
		Last Modified: Wed, 05 Oct 2022 04:39:47 GMT  
		Size: 4.8 MB (4815599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfeae315539086179fc071cd4f1866e8c8d38765cf68e5832d07bdb7388fdc8`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7ceb3ac42fa70ccfe5e470e0efc92d4b1c90e54fcdaf9a451bacc6107bd91f`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca5b1ce88f0b3604342d8ec51ae31e8d9af4dde0b98e0e039eebd8ede5a78fa`  
		Last Modified: Wed, 05 Oct 2022 04:39:46 GMT  
		Size: 240.1 KB (240089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38536dc9dd91716f882e2f305d71c20ccff6acb2ec0a5193f51ee490b91e06d`  
		Last Modified: Wed, 05 Oct 2022 04:39:55 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd18.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:960a7526392894300331ed782ff021b9064ebce94cfe42e5045859e17125fced
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28107677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c978717a3a838e157a52e5cd1a4b004a4483d7a2c137f26dd49b70bbdf2772a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:56:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:56:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:56:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:56:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:57:03 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415982c552b3097dc0f0e3fdab4c2932671fee8d829436501ccb051e6eb83500`  
		Last Modified: Wed, 05 Oct 2022 04:01:19 GMT  
		Size: 4.3 MB (4263811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521f05b326e0e79919ca42ac9a0c47cb9f1caeffc488a7c889282f7fdc7783ab`  
		Last Modified: Wed, 05 Oct 2022 04:01:18 GMT  
		Size: 1.6 KB (1639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea2e867535975d3209819774df2886ba41c121200bbe2c7d447a1e76754391`  
		Last Modified: Wed, 05 Oct 2022 04:01:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53cf70e35b0e254b43fe67021ea0499f47207b931b8d33c35d44b684e86ce1d`  
		Last Modified: Wed, 05 Oct 2022 04:01:18 GMT  
		Size: 107.1 KB (107134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62049f0f865fe4debb6e085c8399238bd0435ae872e5fcdbd8a784dcfaf45f5b`  
		Last Modified: Wed, 05 Oct 2022 04:01:29 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04`

```console
$ docker pull neurodebian@sha256:c18c560f176eb46041715e6e82c11c58f8486836253dff54e820a6bbf72ca516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd20.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:7340e4a1d02b24f61c7891075156bc3aed757461b976e131fef72f65107c6477
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34303966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a497bfc7b1befd51e04e6c0d289e77563686c379b8b7dcec430b35816b5aed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:36:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:36:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:36:41 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:36:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6bd0f856bb7acc90ab4443dc259de1333cfda3d76a258b4ecffe0ba0423001`  
		Last Modified: Wed, 05 Oct 2022 04:40:05 GMT  
		Size: 5.5 MB (5488926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec95545cadde7556963cca6dbe9a7a582e532a753fe098f534873a5d44509c58`  
		Last Modified: Wed, 05 Oct 2022 04:40:04 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7103e2fd0a7a94665abf1b872037f51b8beb8142d737d76f5a9571a588df541b`  
		Last Modified: Wed, 05 Oct 2022 04:40:04 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e953560506e2981b9ab4b287853ba7c1e73ba4d90133660ee56b3dca93e904e`  
		Last Modified: Wed, 05 Oct 2022 04:40:05 GMT  
		Size: 238.6 KB (238576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd20.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:9e19d92f322c13a32357ac60ed6dcd8bce328e15b35f44191da77e8b3822b9ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32618571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3105a115921035dc455c661504a462e1ca355aab8d920f6110d266e0fba37cac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:57:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:57:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:57:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:57:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3730a2cad9cb25a3678d78ba877c9bf0d220929e8f45f9bbff1817122e6f531`  
		Last Modified: Wed, 05 Oct 2022 04:01:41 GMT  
		Size: 5.3 MB (5320766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164c55950381db4d1b78a1b3a2b3f0d3f7bf4de0f4580eccbc1603928ed5b79`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518ae94eca7b012d8ed2f54bc625bd18bf6427860578d187cd9ee1a0a4860106`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2eae91864849c904d629b133ab443a99218e0b47f94c7eeffb491c93da3f31`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 104.2 KB (104194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04-non-free`

```console
$ docker pull neurodebian@sha256:360743995ac767035d3bd9990b6ef5eb7811fde37db655a229750a7770beab3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd20.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:9a3d5e4551c0fde8c789e14f04f63ab2ca9daa7547a9bd25709b76e498c71fa5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34304221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4f6e86c5d058250cdb24ce593bf8d238019b88676c0ba86fc9a1574c38d71da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:36:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:36:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:36:41 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:36:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:36:49 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6bd0f856bb7acc90ab4443dc259de1333cfda3d76a258b4ecffe0ba0423001`  
		Last Modified: Wed, 05 Oct 2022 04:40:05 GMT  
		Size: 5.5 MB (5488926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec95545cadde7556963cca6dbe9a7a582e532a753fe098f534873a5d44509c58`  
		Last Modified: Wed, 05 Oct 2022 04:40:04 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7103e2fd0a7a94665abf1b872037f51b8beb8142d737d76f5a9571a588df541b`  
		Last Modified: Wed, 05 Oct 2022 04:40:04 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e953560506e2981b9ab4b287853ba7c1e73ba4d90133660ee56b3dca93e904e`  
		Last Modified: Wed, 05 Oct 2022 04:40:05 GMT  
		Size: 238.6 KB (238576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe62b2f572b42f89995db5d09adc8f81e9e2f77b2f8d99f052ba95cc9c82fc2`  
		Last Modified: Wed, 05 Oct 2022 04:40:14 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd20.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:4c5340a833188322de86f6f98165eeb9dd0fec61c2bb1d7e1e72acc3b7530d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32618828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a76552309ba47602f9c6033627eb38098234d4aff78a0731d208ce33feaa2535`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:57:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:57:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:57:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:57:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:57:35 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3730a2cad9cb25a3678d78ba877c9bf0d220929e8f45f9bbff1817122e6f531`  
		Last Modified: Wed, 05 Oct 2022 04:01:41 GMT  
		Size: 5.3 MB (5320766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164c55950381db4d1b78a1b3a2b3f0d3f7bf4de0f4580eccbc1603928ed5b79`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518ae94eca7b012d8ed2f54bc625bd18bf6427860578d187cd9ee1a0a4860106`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2eae91864849c904d629b133ab443a99218e0b47f94c7eeffb491c93da3f31`  
		Last Modified: Wed, 05 Oct 2022 04:01:40 GMT  
		Size: 104.2 KB (104194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92cce2f79bfc53f2bbb7601d0755d5b4bff78cd90ab4898e0a1b36ebda80904`  
		Last Modified: Wed, 05 Oct 2022 04:01:52 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd22.04`

```console
$ docker pull neurodebian@sha256:1f56af1fef4b30426331394c4163f22eaa7a8fc2e51485308c5ffb25ef26e855
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd22.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:68570c859f56a40662fdd5ad693da8340bc814ff1062e465bfd702f06c511aa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34454380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab7a779e9e317fab6b650b30df728b9a6bff2ecfe4c130df9f31e8ddea298ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:37:23 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:24 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:37:25 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:37:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f38da8d95f17de727ff64759972dbf1e6d887efe5f254506a23fd70ba3065b7`  
		Last Modified: Wed, 05 Oct 2022 04:40:26 GMT  
		Size: 3.8 MB (3765865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c10071d6f704357ec6b4fc90149ab1f0266bd2f859745ad5887b496563d5e88`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e117899982ab9f8600b6861f1440be605a7212c3ae586161375e0ed0b14fd34`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7957a4d09ef4cfcc2e4f9e8d9d980498ae723c0f2e087b7dd10975d4c6c3be`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 257.6 KB (257574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd22.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:e2fe15575f83678f39332da0326ecda80016d1dbcd9554b03b310060ec8f57bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32092294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeeffd42f7fc03ffc04e736fdcd562ad468ac2023453bc007b5cf158b1460a25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:57:59 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:00 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:01 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:08 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a74d96cddd31a9b0dcb858a34c9e4f2c2d1730679299ce66a44111af946c220`  
		Last Modified: Wed, 05 Oct 2022 04:02:08 GMT  
		Size: 3.6 MB (3593367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cab1a661086a3dc4eddc2627f2548445bd3185053ba7c024f9f03c9069e039`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c5bdf963687c93eca41e724d30263052cb0477c9b631dc4d14432142488855`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30638b5977520e4c36f1e8c72edd304b0be8f000dc6c349287ae1832ebb83b27`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 114.7 KB (114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd22.04-non-free`

```console
$ docker pull neurodebian@sha256:1668a100744dfe2a1dd0686735fd552f6de3c5d69427e6f5c1e581a15f215e69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd22.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:41e63dc24b0f7238288c4579f5cc7f6f7ed3b28bf31ff384ebf5206969dc4c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34454637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da2fb771ff149985fb315d4b17c331aba072267e0e64e8e23081387d09c9303`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:37:23 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:24 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:37:25 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:37:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:37:36 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f38da8d95f17de727ff64759972dbf1e6d887efe5f254506a23fd70ba3065b7`  
		Last Modified: Wed, 05 Oct 2022 04:40:26 GMT  
		Size: 3.8 MB (3765865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c10071d6f704357ec6b4fc90149ab1f0266bd2f859745ad5887b496563d5e88`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e117899982ab9f8600b6861f1440be605a7212c3ae586161375e0ed0b14fd34`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7957a4d09ef4cfcc2e4f9e8d9d980498ae723c0f2e087b7dd10975d4c6c3be`  
		Last Modified: Wed, 05 Oct 2022 04:40:25 GMT  
		Size: 257.6 KB (257574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be700f0ad8ff547a7babb253a538c948ca0a27f3961a6505219a5df4d6e425cc`  
		Last Modified: Wed, 05 Oct 2022 04:40:34 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd22.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:836593c6bc4045f774a159231de968402fb6cb74c71b0a7831ea7166640fe03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32092550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50c75f4d5587a358e178e8aae43b140ef11fa08b92df691c11f3739ffea93ad0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:57:59 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:00 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:01 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:08 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a74d96cddd31a9b0dcb858a34c9e4f2c2d1730679299ce66a44111af946c220`  
		Last Modified: Wed, 05 Oct 2022 04:02:08 GMT  
		Size: 3.6 MB (3593367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cab1a661086a3dc4eddc2627f2548445bd3185053ba7c024f9f03c9069e039`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c5bdf963687c93eca41e724d30263052cb0477c9b631dc4d14432142488855`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30638b5977520e4c36f1e8c72edd304b0be8f000dc6c349287ae1832ebb83b27`  
		Last Modified: Wed, 05 Oct 2022 04:02:07 GMT  
		Size: 114.7 KB (114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d97faa1fa50fd30713bd4d7d1f5eda0123ce7a0b310dcac4ca92093e8040296`  
		Last Modified: Wed, 05 Oct 2022 04:02:18 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:non-free`

```console
$ docker pull neurodebian@sha256:f0db759e1632d1225899599cce0dfb1562c8d3b39e20cddd98cdbf6055681840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:429703f7e0fee449ecf50ab4cc0361f089ca009722e969ee67d2cd0359c2b297
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66670946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95b57e27da6390014efb505383ed7bcf2053334cc51e76b3a2dbef13db3e7ebb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:05 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:06 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:07 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59519a823826166b6d39d758ec5014bd2a5a294b254600d211895dd9c5a866a`  
		Last Modified: Wed, 05 Oct 2022 04:41:04 GMT  
		Size: 11.3 MB (11310722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ec2e5570ce1fabd90c3f195db1c2491485e03dfbaa959a752acc6de8c4641`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f97d5eff53b93eef2dcda043176e5b2ad126bb890a82dd2f405b0f9fe26f5c7`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3860fd5292dee9ad38ed40b5bab9706f31cf24d1663060f1cda46eb7d4856cc8`  
		Last Modified: Wed, 05 Oct 2022 04:41:03 GMT  
		Size: 311.6 KB (311600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3f2699fcf96f4273335b294c96598796754d1f07e7247bae8bdee5bc4a2e84`  
		Last Modified: Wed, 05 Oct 2022 04:41:16 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:6f6e001cebd2e7dc0a6dcdfac69f62ae40db3ad5a27873ceb5dcbdaa656bad5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64912994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a33532c39658d75d58079d13e51642f56eeac73e1fa42bd67e5e54408cd59f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:54 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:05 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32748b0f6967d6d3a663ec439e7a0b631ffe7f6e19fe0a854fa9f60cfbd8013`  
		Last Modified: Wed, 05 Oct 2022 04:02:54 GMT  
		Size: 11.1 MB (11104845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2cd3f4776c95e95f8cf2fe1866ba88b1f93d61bd9cf77c2b0454c13231a54`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74195093fe58a8f1f862fdb46f29db25a349b6d544a17872538f43ed9f69314`  
		Last Modified: Wed, 05 Oct 2022 04:02:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bb772dba620ade3ee2ee0b39ede83b9e4e52271a3c735aea72ebe200c60d9a`  
		Last Modified: Wed, 05 Oct 2022 04:02:53 GMT  
		Size: 105.2 KB (105178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe1986c4b98c09310059dfffefb45f157872b7f5c09d1d2d4c4a68e3acfb272`  
		Last Modified: Wed, 05 Oct 2022 04:03:08 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:49bec358473d52c6911c4c6deae5298035893c9faf0b40a00f42e315e067caa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67630953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d31e9115c7ef837ee295344dd83e413d4164b55f4a4b8fb32836479f79316ebf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:15:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:15:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:15:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:15:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1913722e4098b05a88200af242b3e4de75036431d863b1330ca708cec7d52fda`  
		Last Modified: Wed, 05 Oct 2022 02:17:23 GMT  
		Size: 11.5 MB (11499735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16eddaf2626ebe571c30e863702e069074b6e5a9a22488db55e5d6dfdb41fdf8`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b6358b663dae0a2653ca7146baf655ba0e0e1b765ac7cc2914cdcc4390ea7b`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2069c1e6d4aa4c4d2b785d1396e8487db0a8e83ff092b0fae2d0454a2d6b9a2`  
		Last Modified: Wed, 05 Oct 2022 02:17:22 GMT  
		Size: 105.1 KB (105067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fcc7395aa5a726c6a498dace0389db7c1a51fa808ba67dfecf838c90d83dd7`  
		Last Modified: Wed, 05 Oct 2022 02:17:37 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:0ab19f9f980c6751be623ec2b81ff301f97899d29bdee08dd10aa725ad5960a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:e6909af965ce64be8f6b1c0f32bb6cfd9e6c57b84ebb544b4a32fdbe56a2dc76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64736983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e431e3a9fc2aae9fc0a48164bcff057e00b97976b328292ef893731c9d07ccf4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:54 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c974a6c61f45043e129e219d4381fa099db2e7a173f61912a8982e579a6fe4c`  
		Last Modified: Wed, 05 Oct 2022 04:41:48 GMT  
		Size: 11.8 MB (11764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722be9facb8de2d4f538cbaa389186d6bbd281727551826bf6df7c7e4792928`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cb23dd2e6424a119cad9e202ce4f86217edd6a42e57c86cf5af490f2086ef2`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0d634f74a911a7f3b806dda7044fdbba550ec77c0a9b1d02e6c4d91b97bfc7`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 285.7 KB (285728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:606fe2624ff9d573725a337157db984416d1c306f5902bfb084818a3486d5f5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64331879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcca08c9aa4f00502bf9002fe0c8d93d67c00042c3e9b5de049a083af432b0d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:47 GMT
ADD file:28797d8b43689eae5ccab5b01e88b732a5fca655590a0c9f066d6f0a4d880a95 in / 
# Tue, 04 Oct 2022 23:45:48 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:59:44 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:59:49 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6499ab100dbfb0305e0d96b62f7ad515906275ab30864ac686f0af8ff2fdd114`  
		Last Modified: Tue, 04 Oct 2022 23:52:17 GMT  
		Size: 52.7 MB (52699991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df1adfecab1461b8bd99768350d329ebd6e7b7f5e62880f44688fa052d81ee5`  
		Last Modified: Wed, 05 Oct 2022 04:03:49 GMT  
		Size: 11.5 MB (11532459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211df1c3633aa1661947564b9ed3696aa1124f6f50b0f8f3b5955b1375b7edc9`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae2e7a8e83e699919e6d0b01c2018d0aa2bab3c68163dd11674788e3045521d`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c48121c4388703126d8476e2c0db10a4f0e3fe3b6cf4b0c6c837990718ec487`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 97.4 KB (97449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; 386

```console
$ docker pull neurodebian@sha256:723fcb4319dc470a62adb2c3765720692d48d6ac68a243dbbb4b078135f63508
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65738969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288db7a1ad4289391574ac79c607ffdc110abea480167360cec2bd805154eefd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:40:48 GMT
ADD file:ea6d247c762f6294c87144d1a4308c30669e9e732bd8ff9ef892c71d14563165 in / 
# Tue, 04 Oct 2022 23:40:49 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:16:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:16:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:16:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:16:10 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a0d07a7940ebb4ded014cd2eaedc6b9aa8767ff5afeee7b1b09fce7cbd7a31e`  
		Last Modified: Tue, 04 Oct 2022 23:47:29 GMT  
		Size: 53.6 MB (53647464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ef37d1ca044b99973bac8a03dd842b017b7e1459194239fd83e9dd188597c`  
		Last Modified: Wed, 05 Oct 2022 02:18:16 GMT  
		Size: 12.0 MB (11992190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7bb9a78d2d85b84ec9ffbfb13e408d286021108c33addfecf65bcc2993839`  
		Last Modified: Wed, 05 Oct 2022 02:18:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994eb0042ba9c275a2f107edab9fd532d71c9a01c5addf5d4966600e9bac59b3`  
		Last Modified: Wed, 05 Oct 2022 02:18:14 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d19a641e13b51478bf8e07a69c870d20f5b6988a813cb8082a4e0636567fa19`  
		Last Modified: Wed, 05 Oct 2022 02:18:15 GMT  
		Size: 97.3 KB (97327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:f98a8c574d13705de4d08216b4585180142412d7251b6c34faf53a1ad5d1ea1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:307e1ad9ad2e2ab3c6aa952f25e895043099dbcc0f7d4339d18d0fd481268348
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64737377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32ea95e69fcf6ee1d5ee097e66f41450ef87e137e8a039a2a89b95a06ed804f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:32 GMT
ADD file:b2f29ff1f75077ccce680becaa7bffdc9dfb9c7938188e93673e1b42bf418630 in / 
# Tue, 04 Oct 2022 23:27:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:38:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:38:54 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 04:38:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 04:38:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:39:04 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a9fedee3000f9dcc2b77410cd53420ec321135a3f7a6c688b43f31e503042e1e`  
		Last Modified: Tue, 04 Oct 2022 23:32:34 GMT  
		Size: 52.7 MB (52684279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c974a6c61f45043e129e219d4381fa099db2e7a173f61912a8982e579a6fe4c`  
		Last Modified: Wed, 05 Oct 2022 04:41:48 GMT  
		Size: 11.8 MB (11764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d722be9facb8de2d4f538cbaa389186d6bbd281727551826bf6df7c7e4792928`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cb23dd2e6424a119cad9e202ce4f86217edd6a42e57c86cf5af490f2086ef2`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0d634f74a911a7f3b806dda7044fdbba550ec77c0a9b1d02e6c4d91b97bfc7`  
		Last Modified: Wed, 05 Oct 2022 04:41:47 GMT  
		Size: 285.7 KB (285728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96912c6f77059af0f7694c93d65d843d899967826d2ba9fa69d481f27864ddc0`  
		Last Modified: Wed, 05 Oct 2022 04:41:57 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:47635762f344317598dce2e4bb4b293c55808ffcf013957b1e17246722503bd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64332274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60878ab35485605801fe9972a19002148644695e6ace672c1675fc53331a90da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:47 GMT
ADD file:28797d8b43689eae5ccab5b01e88b732a5fca655590a0c9f066d6f0a4d880a95 in / 
# Tue, 04 Oct 2022 23:45:48 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:59:44 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:59:49 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:55 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6499ab100dbfb0305e0d96b62f7ad515906275ab30864ac686f0af8ff2fdd114`  
		Last Modified: Tue, 04 Oct 2022 23:52:17 GMT  
		Size: 52.7 MB (52699991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df1adfecab1461b8bd99768350d329ebd6e7b7f5e62880f44688fa052d81ee5`  
		Last Modified: Wed, 05 Oct 2022 04:03:49 GMT  
		Size: 11.5 MB (11532459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211df1c3633aa1661947564b9ed3696aa1124f6f50b0f8f3b5955b1375b7edc9`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae2e7a8e83e699919e6d0b01c2018d0aa2bab3c68163dd11674788e3045521d`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c48121c4388703126d8476e2c0db10a4f0e3fe3b6cf4b0c6c837990718ec487`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 97.4 KB (97449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a122987277c618f99d8e9797c12f5554f3e292599645081a8d40ceb2a5e6f6`  
		Last Modified: Wed, 05 Oct 2022 04:04:00 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:a425770283cda772573807278c0b8b6f038f76ca2dd620354fe49d4ae381080e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65739361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b0b187a067e370c9357a6f1f6a7eefc3e0ed25daf17f316e3b9b537ba736c3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:40:48 GMT
ADD file:ea6d247c762f6294c87144d1a4308c30669e9e732bd8ff9ef892c71d14563165 in / 
# Tue, 04 Oct 2022 23:40:49 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:16:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:16:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:16:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:16:10 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:16:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:8a0d07a7940ebb4ded014cd2eaedc6b9aa8767ff5afeee7b1b09fce7cbd7a31e`  
		Last Modified: Tue, 04 Oct 2022 23:47:29 GMT  
		Size: 53.6 MB (53647464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ef37d1ca044b99973bac8a03dd842b017b7e1459194239fd83e9dd188597c`  
		Last Modified: Wed, 05 Oct 2022 02:18:16 GMT  
		Size: 12.0 MB (11992190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7bb9a78d2d85b84ec9ffbfb13e408d286021108c33addfecf65bcc2993839`  
		Last Modified: Wed, 05 Oct 2022 02:18:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994eb0042ba9c275a2f107edab9fd532d71c9a01c5addf5d4966600e9bac59b3`  
		Last Modified: Wed, 05 Oct 2022 02:18:14 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d19a641e13b51478bf8e07a69c870d20f5b6988a813cb8082a4e0636567fa19`  
		Last Modified: Wed, 05 Oct 2022 02:18:15 GMT  
		Size: 97.3 KB (97327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db70b4bbb814cec277b2bbd389ec555efbbf4fb63b356046e21eca8518708d`  
		Last Modified: Wed, 05 Oct 2022 02:18:26 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:xenial`

```console
$ docker pull neurodebian@sha256:c179df88528644a2b2b5df8f22b96dcab0bff5c4d61f7ac2ec80d06a648262db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:xenial` - linux; amd64

```console
$ docker pull neurodebian@sha256:d80e83bfcc000dd04b02c778a1297c7ad2540cb555ab96c90ec154c6a4f0f495
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60902017c278b0db41b17f8f1de27469127d1ea4898b2469f52647585af6120`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:57:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Mar 2022 17:27:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 16 Mar 2022 17:27:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 16 Mar 2022 17:27:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84732b274efc4bdfc5e30a12f05cbd1a9936e3ed5e8952879d6ee935df35eb79`  
		Last Modified: Tue, 31 Aug 2021 04:00:24 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3505bfdde8eb1415423d95064ff6b92c835526022feb1d95009ab5ec04c115`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3fae1c80c2541f9a1f6a2df3ea6faa8f5c9797dda86103383518675981d44`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a78747ad8c43a648a10d04a1c586defca6040cc6c5a4acf404d3962d361631a`  
		Last Modified: Wed, 16 Mar 2022 17:35:35 GMT  
		Size: 227.0 KB (226984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:xenial` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:0b3d5b0cf4235e5ee1e5a25a0e659b44dd6601d4e870e3ca8bead4d37b9cd648
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41341574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed5da098fa1d015a6450f26d7b085d457c2b01a8b427f2d30849343a381e4ca7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Tue, 19 Jul 2022 19:54:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:54:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 19:54:18 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 21:48:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2aeaf3b81eb7fe1658089024c39952f34ea97c9eaff622b60582fbcd51d8f13`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 3.1 KB (3129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3469adcab4ca9a0392e6f6a8101969d54921e20ad79c2f70df00b7a84f6777e0`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d8dd7eaecc8c7cb61334bd81c2c47c8779b4b04668561f1b1caefd019a4b5`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 97.5 KB (97452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:xenial-non-free`

```console
$ docker pull neurodebian@sha256:a9b79b3f807f716014321b46bafc911ed4b0df804d137f9e5cbef226c5173a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:xenial-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:855db2a2543daaf4e085777944831f96ea7a6212d2231da7614dcb717c8a6df4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46729925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c4860f282209b4ea6a5dfd24af70a0307b7664484b8a5bb97070973e934e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:57:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Mar 2022 17:27:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 16 Mar 2022 17:27:10 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 16 Mar 2022 17:27:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:53:37 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84732b274efc4bdfc5e30a12f05cbd1a9936e3ed5e8952879d6ee935df35eb79`  
		Last Modified: Tue, 31 Aug 2021 04:00:24 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3505bfdde8eb1415423d95064ff6b92c835526022feb1d95009ab5ec04c115`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3fae1c80c2541f9a1f6a2df3ea6faa8f5c9797dda86103383518675981d44`  
		Last Modified: Wed, 16 Mar 2022 17:35:34 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a78747ad8c43a648a10d04a1c586defca6040cc6c5a4acf404d3962d361631a`  
		Last Modified: Wed, 16 Mar 2022 17:35:35 GMT  
		Size: 227.0 KB (226984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb28ad0e4efee889c9e9363676830fcc3b2a6b15e7dbd41af4f1c4241f7c5ba`  
		Last Modified: Tue, 19 Jul 2022 19:56:32 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:xenial-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:020707ea4d325b1a95493865742e9fee81f8252f97090141fced8bc788725e39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41341831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d824467043c6d70fbe5679704bf4275178249cffe0b0408e0802cd9f9ddd1d5c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Tue, 19 Jul 2022 19:54:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:54:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 19:54:18 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian xenial main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel xenial main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 21:48:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 21:48:10 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2aeaf3b81eb7fe1658089024c39952f34ea97c9eaff622b60582fbcd51d8f13`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 3.1 KB (3129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3469adcab4ca9a0392e6f6a8101969d54921e20ad79c2f70df00b7a84f6777e0`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d8dd7eaecc8c7cb61334bd81c2c47c8779b4b04668561f1b1caefd019a4b5`  
		Last Modified: Tue, 19 Jul 2022 21:51:27 GMT  
		Size: 97.5 KB (97452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c2010d9b79b1282b1d8f21875e4010b844f2a3c31af5ab9a1a7c039c85bac`  
		Last Modified: Tue, 19 Jul 2022 21:51:38 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
