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
-	[`neurodebian:nd18.04`](#neurodebiannd1804)
-	[`neurodebian:nd18.04-non-free`](#neurodebiannd1804-non-free)
-	[`neurodebian:nd20.04`](#neurodebiannd2004)
-	[`neurodebian:nd20.04-non-free`](#neurodebiannd2004-non-free)
-	[`neurodebian:nd22.04`](#neurodebiannd2204)
-	[`neurodebian:nd22.04-non-free`](#neurodebiannd2204-non-free)
-	[`neurodebian:non-free`](#neurodebiannon-free)
-	[`neurodebian:sid`](#neurodebiansid)
-	[`neurodebian:sid-non-free`](#neurodebiansid-non-free)

## `neurodebian:bionic`

```console
$ docker pull neurodebian@sha256:0dc0c6379aa9de4c7beb314a77836296ed1b9ecec52b6e370d7d1d8fb37e8c7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:436d0f91b2596d1a67587f416d172e20ea63d2ba9fab4064134e658283be40b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31780513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e54202678ffa323cabbfa7d9142d688755ff6767f3a44607c1eb821edd05ac91`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:34:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:34:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 02 Jun 2023 01:34:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 02 Jun 2023 01:34:48 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134fd3f50024409b1b68a3a6f4702400bd9a64d841513f895cc7d024105b78cc`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 4.8 MB (4821090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc489477c8d20c6f0b75906068dc8bd8fe67e1f59f73730d062182879ae588fc`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e27f6db7ca8cf1f438fd944f25c4f24e021afb589cc28a0069a6dff45807a5`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b84f628a2b60e2cd65ca99d9064b0cf13b65787e82747dad9fa68a2e0f016`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 240.2 KB (240158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:be402681584b912cb441771e9a7e1b039e2da347fe7ebf2d1cd9f3736c2e5b4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28385506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:364f14a0ddb6cdd1d2222f8d8d1cd397a7334c3eb47c91b89028ee7a7e491380`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:45:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:45:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 01 Jun 2023 23:45:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 01 Jun 2023 23:45:57 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca58392fb171b1b6480d0e939cedf1babf2bd1d61cbc5fd8667f30d13cf1e73`  
		Last Modified: Thu, 01 Jun 2023 23:46:48 GMT  
		Size: 4.4 MB (4402672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833dbaa1fde66205ef9230adea619512493c576ac6baf435bdb3dc21e1072e1d`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a674c5e1cc8e1b1dcc8a4daacac73e2c8748f8babf74d3cfff92c15ba68e4d`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ce993d3dfac320106ebff10dddff6363ba6d572101bb95c51d321564439c7b`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 240.0 KB (240022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bionic-non-free`

```console
$ docker pull neurodebian@sha256:c6e4772e5c601ede7ccf289927f339f34eab81e04942d3e803f285f931926a2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:137b909d0e4c4e1c4300fa4479a22b15c053df24cbbef0f13fce395100eafa77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31780770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226a853426c1d4b6bd2f86d099a28d4c4db35b9d83d9a7021c549f5386248a11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:34:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:34:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 02 Jun 2023 01:34:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 02 Jun 2023 01:34:48 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:34:53 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134fd3f50024409b1b68a3a6f4702400bd9a64d841513f895cc7d024105b78cc`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 4.8 MB (4821090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc489477c8d20c6f0b75906068dc8bd8fe67e1f59f73730d062182879ae588fc`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e27f6db7ca8cf1f438fd944f25c4f24e021afb589cc28a0069a6dff45807a5`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b84f628a2b60e2cd65ca99d9064b0cf13b65787e82747dad9fa68a2e0f016`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 240.2 KB (240158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e158a3949abb4a78460b0321777ca278a50c79ac290966e5d6a7f027b04e3dd`  
		Last Modified: Fri, 02 Jun 2023 01:35:57 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:edc6bddeb118195088c3f1948fdc52cc913d453e5f543927c7c89c015fe7bd6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28385761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d966d5bec6e766760870e6f4674ca17b3fe69617f78ade07c2a7b6b3154ac8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:45:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:45:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 01 Jun 2023 23:45:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 01 Jun 2023 23:45:57 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:46:00 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca58392fb171b1b6480d0e939cedf1babf2bd1d61cbc5fd8667f30d13cf1e73`  
		Last Modified: Thu, 01 Jun 2023 23:46:48 GMT  
		Size: 4.4 MB (4402672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833dbaa1fde66205ef9230adea619512493c576ac6baf435bdb3dc21e1072e1d`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a674c5e1cc8e1b1dcc8a4daacac73e2c8748f8babf74d3cfff92c15ba68e4d`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ce993d3dfac320106ebff10dddff6363ba6d572101bb95c51d321564439c7b`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 240.0 KB (240022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350adb1f8b3dcaa1835899b2dc84ec2f5a997c31b87aa8e76470a92bc742bc7f`  
		Last Modified: Thu, 01 Jun 2023 23:46:55 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm`

```console
$ docker pull neurodebian@sha256:e059d3fe3bee6985dfd50da7cd9745232ad1e52bf5a230d6f9cc64ca261571a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm` - linux; amd64

```console
$ docker pull neurodebian@sha256:64d743c73fb4140f5c89a065801a1011772e712da92853458cf990228120312d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61315137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a63dd830017f4581b09dca9c03a9f78e89f546056ffa78e636e5c6ca0e1fe807`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:15 GMT
ADD file:7d8adf68670e8dc2af6b8603870ea610fc65ecbb08799f2ca6a3134f5d47d289 in / 
# Tue, 19 Dec 2023 01:20:16 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:26:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:26:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:26:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bc0734b949dcdcabe5bfdf0c8b9f44491e0fce04cb10c9c6e76282b9f6abdf01`  
		Last Modified: Tue, 19 Dec 2023 01:24:35 GMT  
		Size: 49.6 MB (49561579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60813851d3d4129f056f873cc009e941a14179ae49d530351dee04ec0df8ad54`  
		Last Modified: Tue, 19 Dec 2023 17:27:54 GMT  
		Size: 11.5 MB (11463884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfe18d5147ef1fe4b9a42ed7b57ca5c19f4ebe238093c00b4b7dbe943b7016`  
		Last Modified: Tue, 19 Dec 2023 17:27:52 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de660d6bb77b3b3cc331a91c9a465ef1f3e4edbe3d63d0cbdc857fd691b63f1f`  
		Last Modified: Tue, 19 Dec 2023 17:27:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e384fde624b03e6309d39f76a15ddeff56a9ee7e8b1bf190f416e635708dcf98`  
		Last Modified: Tue, 19 Dec 2023 17:27:53 GMT  
		Size: 287.7 KB (287661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:0dc9866a07d16e6f04cf8feb788a32eda13c8343d6c5dc835760ae88ab095312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61310258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254221e8beee5a2d58e44db505f29e1bcabc70a602dd9cc2967ff64aa7914a37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:02 GMT
ADD file:412f80f75ed3e520f767e70b6b27fc81807f62fc5c6e5adf756507e33af9fa6b in / 
# Tue, 19 Dec 2023 01:41:02 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:22 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:23 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:24 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b66b4ecd3ecfb67b3b7a2a44b0199cbdfc94965c8bd3fefab75cd2e612799740`  
		Last Modified: Tue, 19 Dec 2023 01:44:14 GMT  
		Size: 49.6 MB (49592259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536d08fe62d16991ed44688b2a03cf0a9ad4c1a6a3c91a38aabff54d8dc121f2`  
		Last Modified: Tue, 19 Dec 2023 03:07:57 GMT  
		Size: 11.4 MB (11427684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17a3a06500c5196e68b32c08163cef7f17f514e1edc70f4d842ef892c4f5c5b`  
		Last Modified: Tue, 19 Dec 2023 03:07:56 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edf619636202804b32b3951669c4b66707bb7af37e67f8a0be202699c87cb64`  
		Last Modified: Tue, 19 Dec 2023 03:07:55 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dcde0e73627274650648744924524389f5a680d3b32383a3b53fe1c475259a`  
		Last Modified: Tue, 19 Dec 2023 03:07:56 GMT  
		Size: 288.3 KB (288298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; 386

```console
$ docker pull neurodebian@sha256:13873f1f5441f485e2c264f0dec37c15a1978c08e37131667e9768217c305ea8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62756239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4efa30f46b3252fea5ffd441d5ebdd358458e292f4f7fdd6b8306f50a2793891`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:38:52 GMT
ADD file:c20aace531a43765f8c1b69c75d7f46a4ab443377a663ab47e0bb2ceb013a611 in / 
# Tue, 19 Dec 2023 01:38:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b51fe964cb335e4bc3b61dca07146c7a0aa4c31e5ae9fec90f2a950818a21a4`  
		Last Modified: Tue, 19 Dec 2023 01:43:18 GMT  
		Size: 50.6 MB (50582312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb2f81c47b7b130f3418b0d116d480499c54496b48208ed47c1d8fc839bf85d`  
		Last Modified: Tue, 19 Dec 2023 03:53:03 GMT  
		Size: 11.9 MB (11883835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a351a4d22f54a27ecd69f950120d824c9f9f5e6a6b20e9f258285459822f274`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205522c289f7b88de70a28984bb914948c84a0cc7c29500f7e1f730e0e9db0a4`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5dc22a3c30fe732622f96301ac945a4566da973563854c515b5ca6fac7855f`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 288.1 KB (288078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm-non-free`

```console
$ docker pull neurodebian@sha256:0f5caf6ff3b68f1e9a1a4df0f5018df40d31e98a8b5248f6e6fa40a4cfc55f3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:ae6e1df013b07c2f8e42580da1322753030a87403dd3460b6ba33c7a78d487cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61315570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b4bd21363d3603ebce350347a80c9a2f6bd4e1aada22c9adb09370a21d04ab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:15 GMT
ADD file:7d8adf68670e8dc2af6b8603870ea610fc65ecbb08799f2ca6a3134f5d47d289 in / 
# Tue, 19 Dec 2023 01:20:16 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:26:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:26:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:26:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:19 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:bc0734b949dcdcabe5bfdf0c8b9f44491e0fce04cb10c9c6e76282b9f6abdf01`  
		Last Modified: Tue, 19 Dec 2023 01:24:35 GMT  
		Size: 49.6 MB (49561579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60813851d3d4129f056f873cc009e941a14179ae49d530351dee04ec0df8ad54`  
		Last Modified: Tue, 19 Dec 2023 17:27:54 GMT  
		Size: 11.5 MB (11463884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfe18d5147ef1fe4b9a42ed7b57ca5c19f4ebe238093c00b4b7dbe943b7016`  
		Last Modified: Tue, 19 Dec 2023 17:27:52 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de660d6bb77b3b3cc331a91c9a465ef1f3e4edbe3d63d0cbdc857fd691b63f1f`  
		Last Modified: Tue, 19 Dec 2023 17:27:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e384fde624b03e6309d39f76a15ddeff56a9ee7e8b1bf190f416e635708dcf98`  
		Last Modified: Tue, 19 Dec 2023 17:27:53 GMT  
		Size: 287.7 KB (287661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbb4d41320b96049bbafe069a4274f3ed09e0f6516709d539b0fc3096b204eb`  
		Last Modified: Tue, 19 Dec 2023 17:28:02 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:97e4b885432424139b795ac305ffa9735c8271a48c8540d8f7054494d8c8bf69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61310687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6557c9b6f643f36bfd3aecc7cd482c215de4f6ca556ef892d21dc013d02a4e08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:02 GMT
ADD file:412f80f75ed3e520f767e70b6b27fc81807f62fc5c6e5adf756507e33af9fa6b in / 
# Tue, 19 Dec 2023 01:41:02 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:22 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:23 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:24 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:31 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b66b4ecd3ecfb67b3b7a2a44b0199cbdfc94965c8bd3fefab75cd2e612799740`  
		Last Modified: Tue, 19 Dec 2023 01:44:14 GMT  
		Size: 49.6 MB (49592259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536d08fe62d16991ed44688b2a03cf0a9ad4c1a6a3c91a38aabff54d8dc121f2`  
		Last Modified: Tue, 19 Dec 2023 03:07:57 GMT  
		Size: 11.4 MB (11427684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17a3a06500c5196e68b32c08163cef7f17f514e1edc70f4d842ef892c4f5c5b`  
		Last Modified: Tue, 19 Dec 2023 03:07:56 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edf619636202804b32b3951669c4b66707bb7af37e67f8a0be202699c87cb64`  
		Last Modified: Tue, 19 Dec 2023 03:07:55 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dcde0e73627274650648744924524389f5a680d3b32383a3b53fe1c475259a`  
		Last Modified: Tue, 19 Dec 2023 03:07:56 GMT  
		Size: 288.3 KB (288298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8378c25bd9411f0a142fee243394a286cc6f1f7c217d86581f263bb24ab74ea2`  
		Last Modified: Tue, 19 Dec 2023 03:08:05 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:f99434b0d8bcbdc85a6f4a6dc4f2d572af83eb4e4a853a144933fc1e19bc4606
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62756668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d8f03971e633e63c99322029d9a69b024c210cf1bab077dfb26f38441ef4f81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:38:52 GMT
ADD file:c20aace531a43765f8c1b69c75d7f46a4ab443377a663ab47e0bb2ceb013a611 in / 
# Tue, 19 Dec 2023 01:38:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:41 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:9b51fe964cb335e4bc3b61dca07146c7a0aa4c31e5ae9fec90f2a950818a21a4`  
		Last Modified: Tue, 19 Dec 2023 01:43:18 GMT  
		Size: 50.6 MB (50582312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb2f81c47b7b130f3418b0d116d480499c54496b48208ed47c1d8fc839bf85d`  
		Last Modified: Tue, 19 Dec 2023 03:53:03 GMT  
		Size: 11.9 MB (11883835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a351a4d22f54a27ecd69f950120d824c9f9f5e6a6b20e9f258285459822f274`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205522c289f7b88de70a28984bb914948c84a0cc7c29500f7e1f730e0e9db0a4`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5dc22a3c30fe732622f96301ac945a4566da973563854c515b5ca6fac7855f`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 288.1 KB (288078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5084ee365b51d3a05cddbfc8d59c329e46ad420b9fed6adfc9993e92d775d100`  
		Last Modified: Tue, 19 Dec 2023 03:53:11 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:7741b00acdf38fd8ca15d3ed4d201e876397f1a8e3eba11e1dced1ede42258c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:297bbad7c3560a43ad967a3e5f87ab2bc982ab94ee9ecc2821a30fabcc802056
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66679270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9605beb5a27b9108c59145e3c7d7ffac9e705cfe1f63e2fd86746f2d991ea918`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0856bfbd37c04c98dbed2cfbebaa2c7f12b11d4603e1cb62110aeede128091`  
		Last Modified: Tue, 19 Dec 2023 17:27:32 GMT  
		Size: 11.3 MB (11311904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5429bd5bea56c5bc55594233fc233733046f366dd1123c4a94b04f92f19228`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aecaaacf549bbf53913c6f0f497a5439b394e793b413c0cf0c796f9a040148`  
		Last Modified: Tue, 19 Dec 2023 17:27:31 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfd707f03ef0ab3405a9b45e6cec06e69f42f362ca8170ed6ac867bb3cfc5`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 308.0 KB (308007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:05ae47403683229c382942e9201cc80cec5f93aff3b92fa484586d3f493da6c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65331638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491b1d0b41e609f15065b67955fa1e9ad57896dfb61a7785345b6e12ee9a3ffa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:06 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a678807dec42582e887390c579155f2ff3f3c25b0fdfeb11854c487bfc0479`  
		Last Modified: Tue, 19 Dec 2023 03:07:34 GMT  
		Size: 11.3 MB (11313652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2434d66e0ac932afe623ab8fb9ddeaf97131cee80959a55990df31cdcbf946`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8665dd0adc074adaedc5ecf6d1a9424f986359c007f4c36cbcae0e95056a940b`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9cb0c2c79d2d93968c00288fda1bdc0a21e05ec517669fe68234be55ffd271`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 307.9 KB (307878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; 386

```console
$ docker pull neurodebian@sha256:42bdac607d78c342b9d010ffbf4ab731014da1db8092747d0e8bd54e535e71ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68064908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92da83f63ff7256ee873cf328fac9c99a5068f62517bc346aa23821757a0b40b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:19 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Tue, 19 Dec 2023 01:39:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0a042ddf885a246973867761eaeb7097c4ffba0155dc9ecd3c004dd567e6d6`  
		Last Modified: Tue, 19 Dec 2023 03:52:41 GMT  
		Size: 11.7 MB (11708784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b236339ceeaafd4e56a9404e9528b71ad8f45255c5f053e303f89715c4f09bd`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca1d30df83fb1854dac8182f65566474d229cbccc4c7a4029273bddd4829d`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c554dc1a2dd646999214a1df9a3c0747d1dfb49b0931fd602f90f37f7f2ba84`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 307.8 KB (307775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:2cce0daa7423ab3c692c4904edbe4ca12a6f0bbc3a7d159b20505d0b80798dc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:62f489eb5479e968e8c7c95925b27de9a00e0c8feec115dca3360e7fc0e8577c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66679629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982a6feac3daa4329dd853bb3f5ce5e6aea98c80dff35c9a691ccc6703f6c0a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:58 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0856bfbd37c04c98dbed2cfbebaa2c7f12b11d4603e1cb62110aeede128091`  
		Last Modified: Tue, 19 Dec 2023 17:27:32 GMT  
		Size: 11.3 MB (11311904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5429bd5bea56c5bc55594233fc233733046f366dd1123c4a94b04f92f19228`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aecaaacf549bbf53913c6f0f497a5439b394e793b413c0cf0c796f9a040148`  
		Last Modified: Tue, 19 Dec 2023 17:27:31 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfd707f03ef0ab3405a9b45e6cec06e69f42f362ca8170ed6ac867bb3cfc5`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 308.0 KB (308007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe21a9c4f2844b1731353c2ccf79ed576bb765bc5854eab55e8c885e783c04d`  
		Last Modified: Tue, 19 Dec 2023 17:27:42 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:c0d28e0c05ae9c84fb89006bd6effeb566b7b36c125e840469027ac858a2fea0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65331998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e6683e8b8d8ee63d5c5efe716a4e5f08c490c43604cdb1f28350b960ae8b32`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:06 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:12 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a678807dec42582e887390c579155f2ff3f3c25b0fdfeb11854c487bfc0479`  
		Last Modified: Tue, 19 Dec 2023 03:07:34 GMT  
		Size: 11.3 MB (11313652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2434d66e0ac932afe623ab8fb9ddeaf97131cee80959a55990df31cdcbf946`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8665dd0adc074adaedc5ecf6d1a9424f986359c007f4c36cbcae0e95056a940b`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9cb0c2c79d2d93968c00288fda1bdc0a21e05ec517669fe68234be55ffd271`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 307.9 KB (307878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2849c1469b7eddd754a21b835849faa61f22936935882ba932182e1166a8e`  
		Last Modified: Tue, 19 Dec 2023 03:07:46 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:3525dcc77a6b6f044fb762f2a30c6e1d94790d1853116ce54032830935b37d73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68065268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bd45296a7a75d68f3b5963299ba70aba200d208e0dfe56532f768a6a9ee1cc0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:19 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Tue, 19 Dec 2023 01:39:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:18 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0a042ddf885a246973867761eaeb7097c4ffba0155dc9ecd3c004dd567e6d6`  
		Last Modified: Tue, 19 Dec 2023 03:52:41 GMT  
		Size: 11.7 MB (11708784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b236339ceeaafd4e56a9404e9528b71ad8f45255c5f053e303f89715c4f09bd`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca1d30df83fb1854dac8182f65566474d229cbccc4c7a4029273bddd4829d`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c554dc1a2dd646999214a1df9a3c0747d1dfb49b0931fd602f90f37f7f2ba84`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 307.8 KB (307775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b230d20e89abb46584252eccc63bcf58afb7c16c9f0fe85da93d4a3b3f28442e`  
		Last Modified: Tue, 19 Dec 2023 03:52:51 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:ce0180be636220f3a87835ecb491e44dcac234df82efcbc10d099866b1617ce3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:a62b209877b5c5a25d335582b2bb1167bd12a57d812fbee47b395a35cc125699
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cec7c78b29b47c0541641b7be7d3eeacef33acddf23f606023369d26314c5c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:00 GMT
ADD file:e5e3f2fedf4fa6382f3bbf6203060ba68df1aadc7ebfa3350df20bf31b102f0e in / 
# Tue, 19 Dec 2023 01:21:01 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:27 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:29 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30b73a2ffaab3c39355a8bcc5eae8ba1465bd7d9467f197b91f7635816b16bc9`  
		Last Modified: Tue, 19 Dec 2023 01:25:58 GMT  
		Size: 50.5 MB (50500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab53549f1d6f91ce1fcfb5a6ff812ebeca69b02bd07cbe6a1ae8df426ca90a4`  
		Last Modified: Tue, 19 Dec 2023 17:27:13 GMT  
		Size: 10.5 MB (10504778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e731abcc54cf5bcb086bc36b1e6f12ad7d73ca0f0139f4a0070a16d1bb6105a`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f5821293636913a5e5f156fde6c19fb62901cbcf38d66898b3154b4222b9e4`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2c8d395609db22d85da949ac48af56210ff29e74765f2ae4f6f3dd8007e73c`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 299.4 KB (299435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:600d482db7b7f3d51d4f3421c83edcc89e1f2877a2a2eee0924eb54a7f2ae386
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60101042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a3893cecce63384e1d3f1b1992262b77aefdfae5aaba094ef03c980ff3b6a89`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:31 GMT
ADD file:df5e5dd39efc6ae3cc9132f6ca6bb569731f7a37cf4b41f87bcb7aa1ba9771e8 in / 
# Tue, 19 Dec 2023 01:41:32 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:05:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:05:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:05:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:05:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93507f9712ced9fbfd0d0f689cf7b55fb245cef88530c07ac5dc5cad20fa889d`  
		Last Modified: Tue, 19 Dec 2023 01:45:40 GMT  
		Size: 49.3 MB (49289026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c5fbc51c74a4f8750f148252ed129c0c57cc94d6e2b2f4ae83d5f1420fe9a2`  
		Last Modified: Tue, 19 Dec 2023 03:07:17 GMT  
		Size: 10.5 MB (10510551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7d0a1a828eff413800cec078c31256371b964ca8aa29198aea52bf930d8057`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dd41deea093d7e81d0007ed35420760c6cea45b552f575b45ee9e400eb7beb`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533e3cd401bcc7d93489b3ef17afb87ed22d96e3b19fb76fa2dfc90ee457c0c0`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 299.4 KB (299449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; 386

```console
$ docker pull neurodebian@sha256:ec322aa50424cc143d1686f5c149fa6a13d427e7e3a49126580823944e5101a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff097a81fd1e52e4c0c90fb596ba089dc94e8a830bd1c10c18c463bcaca93815`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:40 GMT
ADD file:4c009b0d408e3df297246382d87b0be68c34886e13ed79ba47feb8ff51acb863 in / 
# Tue, 19 Dec 2023 01:39:41 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:50:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:50:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:50:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:50:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8d351f5ab6958b8ca5f2b8e463c49cba65be4285ead8bdbc1378b5ce2c8cd736`  
		Last Modified: Tue, 19 Dec 2023 01:44:53 GMT  
		Size: 51.3 MB (51255444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01ee695ce5b07c4aa0b90a93605547e631e728141c311b4bbf7c54fdac3be4`  
		Last Modified: Tue, 19 Dec 2023 03:52:23 GMT  
		Size: 10.9 MB (10868372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379f0dec32e0488edb8bff0dcd0be9abb4c04675943257bc5c784bfd82fd870`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56e62a0bf8c627e0bfa8f075fdfdcabfd6fc8d4809a1ec507a91d81eec6c13a`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f016555c3e2050965be5f7aece4aa1a93943629cdaa4359707eb76a9fac47534`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 299.4 KB (299418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:dc6793856187c9c39c2b66375d0c1c937b962fc9b4763e6aef88513c6022b0a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:328b5eade2581994ea8a93d00f30594ac1654d1f41755a825464613a109677dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0384483cda04a7d15823f8140de13eef8410dc29c4509077931167c9a24b790b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:00 GMT
ADD file:e5e3f2fedf4fa6382f3bbf6203060ba68df1aadc7ebfa3350df20bf31b102f0e in / 
# Tue, 19 Dec 2023 01:21:01 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:27 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:29 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:38 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:30b73a2ffaab3c39355a8bcc5eae8ba1465bd7d9467f197b91f7635816b16bc9`  
		Last Modified: Tue, 19 Dec 2023 01:25:58 GMT  
		Size: 50.5 MB (50500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab53549f1d6f91ce1fcfb5a6ff812ebeca69b02bd07cbe6a1ae8df426ca90a4`  
		Last Modified: Tue, 19 Dec 2023 17:27:13 GMT  
		Size: 10.5 MB (10504778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e731abcc54cf5bcb086bc36b1e6f12ad7d73ca0f0139f4a0070a16d1bb6105a`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f5821293636913a5e5f156fde6c19fb62901cbcf38d66898b3154b4222b9e4`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2c8d395609db22d85da949ac48af56210ff29e74765f2ae4f6f3dd8007e73c`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 299.4 KB (299435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420d51671fd62d4e126c31d4831df03a8ab2acf080c8bc83a8eb772760dedd0b`  
		Last Modified: Tue, 19 Dec 2023 17:27:23 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:f764445ceab408a8b33ff6e0e70255f357997da4ad5c15da095c4619d3778441
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60101398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bca1e9bfe9bfa37e72929b0e193a720d329783d7289784ea929d1b75eb5ac9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:31 GMT
ADD file:df5e5dd39efc6ae3cc9132f6ca6bb569731f7a37cf4b41f87bcb7aa1ba9771e8 in / 
# Tue, 19 Dec 2023 01:41:32 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:05:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:05:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:05:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:05:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:05:57 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:93507f9712ced9fbfd0d0f689cf7b55fb245cef88530c07ac5dc5cad20fa889d`  
		Last Modified: Tue, 19 Dec 2023 01:45:40 GMT  
		Size: 49.3 MB (49289026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c5fbc51c74a4f8750f148252ed129c0c57cc94d6e2b2f4ae83d5f1420fe9a2`  
		Last Modified: Tue, 19 Dec 2023 03:07:17 GMT  
		Size: 10.5 MB (10510551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7d0a1a828eff413800cec078c31256371b964ca8aa29198aea52bf930d8057`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dd41deea093d7e81d0007ed35420760c6cea45b552f575b45ee9e400eb7beb`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533e3cd401bcc7d93489b3ef17afb87ed22d96e3b19fb76fa2dfc90ee457c0c0`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 299.4 KB (299449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134eef9048535ffd6796b146e362f4919bd2130d2183feda6ba05db3dcd4df96`  
		Last Modified: Tue, 19 Dec 2023 03:07:25 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:8b36bd35183e06994e6a3ecff588a4906eca28d78ca5cb4e9f15047484150f83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3995db1af7a67fbcd53860257fab3e0fcf305561c0d2bb8d86093d9000fcf4fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:40 GMT
ADD file:4c009b0d408e3df297246382d87b0be68c34886e13ed79ba47feb8ff51acb863 in / 
# Tue, 19 Dec 2023 01:39:41 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:50:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:50:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:50:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:50:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:00 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:8d351f5ab6958b8ca5f2b8e463c49cba65be4285ead8bdbc1378b5ce2c8cd736`  
		Last Modified: Tue, 19 Dec 2023 01:44:53 GMT  
		Size: 51.3 MB (51255444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01ee695ce5b07c4aa0b90a93605547e631e728141c311b4bbf7c54fdac3be4`  
		Last Modified: Tue, 19 Dec 2023 03:52:23 GMT  
		Size: 10.9 MB (10868372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379f0dec32e0488edb8bff0dcd0be9abb4c04675943257bc5c784bfd82fd870`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56e62a0bf8c627e0bfa8f075fdfdcabfd6fc8d4809a1ec507a91d81eec6c13a`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f016555c3e2050965be5f7aece4aa1a93943629cdaa4359707eb76a9fac47534`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 299.4 KB (299418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956c541ecb88d435c686202fe372734189b393a6e7af060a508bd5cc94110ecf`  
		Last Modified: Tue, 19 Dec 2023 03:52:31 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal`

```console
$ docker pull neurodebian@sha256:ba031fd6fd8d10c60789c1e1e36b0f1d6261133c9561aba991f4c34a0975e0a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:44b7d0b76bf7eecb24561da2543c6759b12e4c9c8414f1b9e78935512ad2727c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34320320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ec23d1ce12db52e245fece4cd06f6c0ffff3753f214b1c518735daeb4ee2c22`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:30:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:30:46 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 11:30:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 11:30:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e8e2de0d867ec7e11698bdb11d5da78cb7658f6585c06230c6a1c5a8a2fbbb`  
		Last Modified: Sat, 16 Dec 2023 11:31:56 GMT  
		Size: 5.5 MB (5494756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0973d4d7f63b90a4064cbde84bfe5368a09181a1fa9398b78a60dbc8e11b64ad`  
		Last Modified: Sat, 16 Dec 2023 11:31:55 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496c414a338fcd0964d5bf308922aee54df3b752acf3e50380daa1c0e0fde868`  
		Last Modified: Sat, 16 Dec 2023 11:31:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522217e64373829c117276478f35ac5b21ed22393bff75e3fce4e36b00e5eb90`  
		Last Modified: Sat, 16 Dec 2023 11:31:56 GMT  
		Size: 239.5 KB (239529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:focal` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:f1141274e347e45773d8be49383336333cd34d6d95faf145db741e34a942a790
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32919471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b7457db0e6738e03edc22022e117ad4eadbd81f74b7941fe5a1a82d5edf8faa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:29:33 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:29:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:29:34 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:29:41 GMT
ADD file:9ec8b7bbb2fbc8c90f1f24e19ab22130e03be1cc4727459e1265d2ed652377a1 in / 
# Wed, 13 Dec 2023 10:29:42 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:57:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:57:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 10:57:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 10:57:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5319f8e5f3f0f8f6e663c807041d5294b7c309e06b86d115409bbdb4c9d7165`  
		Last Modified: Thu, 14 Dec 2023 13:03:55 GMT  
		Size: 27.2 MB (27203144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d82e878836647a3198acd6d3342bb489ce6f36423f93eae6fad1bcfb5f8238`  
		Last Modified: Sat, 16 Dec 2023 10:58:54 GMT  
		Size: 5.5 MB (5474754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a11c6e2465b40ebdf20e1ff87f0882767e680eb2a491f8e71c9d655a6a465d`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6297c2a11b1380ae62c841725a9a5970007e1bc75aa5a0c31304c2cb62d9b3b6`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e24ca661ae9b1e0360d4cf84cc5dbf17c22f46e6b5520ecec5c8c1341b2dca`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 239.6 KB (239564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal-non-free`

```console
$ docker pull neurodebian@sha256:28e44c247bccb216319d79168088c695113a5b4e1a60f7cb04c2d95618519750
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:focal-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:b3f3cafbd80fb60d84f06cb6a850f7972632442c52fc209d483cfcce6082e00d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34320578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dcb395334cecfe02f934685afedad044adb17b32726d7d5b049a0ada8825ea3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:30:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:30:46 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 11:30:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 11:30:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:30:57 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e8e2de0d867ec7e11698bdb11d5da78cb7658f6585c06230c6a1c5a8a2fbbb`  
		Last Modified: Sat, 16 Dec 2023 11:31:56 GMT  
		Size: 5.5 MB (5494756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0973d4d7f63b90a4064cbde84bfe5368a09181a1fa9398b78a60dbc8e11b64ad`  
		Last Modified: Sat, 16 Dec 2023 11:31:55 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496c414a338fcd0964d5bf308922aee54df3b752acf3e50380daa1c0e0fde868`  
		Last Modified: Sat, 16 Dec 2023 11:31:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522217e64373829c117276478f35ac5b21ed22393bff75e3fce4e36b00e5eb90`  
		Last Modified: Sat, 16 Dec 2023 11:31:56 GMT  
		Size: 239.5 KB (239529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51570a82a6bbfd07eee978ee080dc61dfbeb817ba567432a8e90a4b696b108df`  
		Last Modified: Sat, 16 Dec 2023 11:32:04 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:focal-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:2a74510ac598b775b0c5e6806309bb643c0bad336314a336a5a7012bf559d4b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32919726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc08a48952fb4706f359961b5ddaac65179ea556854ce9d6cd442162e5051057`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:29:33 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:29:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:29:34 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:29:41 GMT
ADD file:9ec8b7bbb2fbc8c90f1f24e19ab22130e03be1cc4727459e1265d2ed652377a1 in / 
# Wed, 13 Dec 2023 10:29:42 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:57:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:57:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 10:57:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 10:57:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:58:02 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:a5319f8e5f3f0f8f6e663c807041d5294b7c309e06b86d115409bbdb4c9d7165`  
		Last Modified: Thu, 14 Dec 2023 13:03:55 GMT  
		Size: 27.2 MB (27203144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d82e878836647a3198acd6d3342bb489ce6f36423f93eae6fad1bcfb5f8238`  
		Last Modified: Sat, 16 Dec 2023 10:58:54 GMT  
		Size: 5.5 MB (5474754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a11c6e2465b40ebdf20e1ff87f0882767e680eb2a491f8e71c9d655a6a465d`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6297c2a11b1380ae62c841725a9a5970007e1bc75aa5a0c31304c2cb62d9b3b6`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e24ca661ae9b1e0360d4cf84cc5dbf17c22f46e6b5520ecec5c8c1341b2dca`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 239.6 KB (239564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6109e5cc5f76e744d01622cfd74cab3eafaa790607e4df8e93e354b23705278`  
		Last Modified: Sat, 16 Dec 2023 10:59:01 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:jammy`

```console
$ docker pull neurodebian@sha256:ba325e5e6061bf24da78c27502f503a1693550dafd14b2bd75337d06afd1053e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy` - linux; amd64

```console
$ docker pull neurodebian@sha256:832ad5e9329cae055a24b82e2614fb4260f02209aebe2b531754f1198dd3b4c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34467765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6917cbd534a78c0843fe16fe96232df45d6101582900a7bab2146c6b71b602c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:31:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:31:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 11:31:08 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 11:31:13 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62d44c808e32e3a77cd43373f0a8470fdb06d639ba026de364a97150318d33e`  
		Last Modified: Sat, 16 Dec 2023 11:32:13 GMT  
		Size: 3.8 MB (3766320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef772247763c5df1ee7d344d2f5d647e5f66c098b6331e8091e2d15b0061605f`  
		Last Modified: Sat, 16 Dec 2023 11:32:12 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d35d7275d528ee79ed8369114469886a50b319ee8c3f716790ab260e219bbb`  
		Last Modified: Sat, 16 Dec 2023 11:32:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4272c56b744309cef303df1ac073c04ce1c74bd45d3797b2325a65636469a8`  
		Last Modified: Sat, 16 Dec 2023 11:32:13 GMT  
		Size: 252.9 KB (252855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:fd8b8e62b24ae76d9c4dac845f710ff1a7d0abe1706cc06dd2fa62e0f4d6c7b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32396537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf3fceda0bd85cb6068caad7e45ce8d59a7be4541dd78511b5774bbf54ce0089`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:41:50 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:41:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:41:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:41:51 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:41:54 GMT
ADD file:50f947da69b3b6c63695be9c49eee16f7a7dcdecdceb51e5bee1609b845bf483 in / 
# Tue, 12 Dec 2023 11:41:54 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:58:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:58:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 10:58:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 10:58:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7734efb8b826f955c6a3bb51d7c84cb262d0e600ea3980f5bce69fa7f4f92d24`  
		Last Modified: Tue, 12 Dec 2023 16:00:15 GMT  
		Size: 28.4 MB (28400282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502eabb3351c24cea84fb9e5ccf4adb9d6d658b6682fcb7576fd2c82d70f7b70`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 3.7 MB (3740006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8957f77b0604cf331a09bdc53855627bc26526f149533f2960ad2dbc4b6ed32`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5c144174c37657363446c929ba2fc409d387a017fd3babb136a15836cd50ca`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c1cad4f258411c4497ccc895050e1beb7fcacf75785a4807a3f09ae6a3f`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 254.2 KB (254236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:jammy-non-free`

```console
$ docker pull neurodebian@sha256:81749d6f6e02ebab02d467e80d7d88ea6cbed6cf29cda5eaf10a7993bd9ba84d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:2fd21ffe831d7da905d87e689e4d459dc3332f35325b84286eb27a4cf5f6c4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34468022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d00d2ab78b0f1e54b1bdbe7fc8679418d930d3e1bbab0588963c3bfa5e2e1be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:31:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:31:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 11:31:08 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 11:31:13 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:31:17 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62d44c808e32e3a77cd43373f0a8470fdb06d639ba026de364a97150318d33e`  
		Last Modified: Sat, 16 Dec 2023 11:32:13 GMT  
		Size: 3.8 MB (3766320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef772247763c5df1ee7d344d2f5d647e5f66c098b6331e8091e2d15b0061605f`  
		Last Modified: Sat, 16 Dec 2023 11:32:12 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d35d7275d528ee79ed8369114469886a50b319ee8c3f716790ab260e219bbb`  
		Last Modified: Sat, 16 Dec 2023 11:32:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4272c56b744309cef303df1ac073c04ce1c74bd45d3797b2325a65636469a8`  
		Last Modified: Sat, 16 Dec 2023 11:32:13 GMT  
		Size: 252.9 KB (252855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b030e3d725500e3908775fbc82436b7e595c244fe95c9a9073fce868a116579`  
		Last Modified: Sat, 16 Dec 2023 11:32:21 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:a234f2c6b2cf65fd1c6f69b81720033f7d359058455f2c2f81c8600313be2ed7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32396794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e35742c042c1fdbcf4086c65446d3971c3686ed2d0beb5d42207d7e1457aa10`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:41:50 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:41:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:41:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:41:51 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:41:54 GMT
ADD file:50f947da69b3b6c63695be9c49eee16f7a7dcdecdceb51e5bee1609b845bf483 in / 
# Tue, 12 Dec 2023 11:41:54 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:58:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:58:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 10:58:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 10:58:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:58:20 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:7734efb8b826f955c6a3bb51d7c84cb262d0e600ea3980f5bce69fa7f4f92d24`  
		Last Modified: Tue, 12 Dec 2023 16:00:15 GMT  
		Size: 28.4 MB (28400282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502eabb3351c24cea84fb9e5ccf4adb9d6d658b6682fcb7576fd2c82d70f7b70`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 3.7 MB (3740006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8957f77b0604cf331a09bdc53855627bc26526f149533f2960ad2dbc4b6ed32`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5c144174c37657363446c929ba2fc409d387a017fd3babb136a15836cd50ca`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c1cad4f258411c4497ccc895050e1beb7fcacf75785a4807a3f09ae6a3f`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 254.2 KB (254236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff7723f0eeec7ac468595c47a6d85a191198efebe6eb375fde3f2712efae13`  
		Last Modified: Sat, 16 Dec 2023 10:59:17 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:7741b00acdf38fd8ca15d3ed4d201e876397f1a8e3eba11e1dced1ede42258c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:297bbad7c3560a43ad967a3e5f87ab2bc982ab94ee9ecc2821a30fabcc802056
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66679270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9605beb5a27b9108c59145e3c7d7ffac9e705cfe1f63e2fd86746f2d991ea918`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0856bfbd37c04c98dbed2cfbebaa2c7f12b11d4603e1cb62110aeede128091`  
		Last Modified: Tue, 19 Dec 2023 17:27:32 GMT  
		Size: 11.3 MB (11311904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5429bd5bea56c5bc55594233fc233733046f366dd1123c4a94b04f92f19228`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aecaaacf549bbf53913c6f0f497a5439b394e793b413c0cf0c796f9a040148`  
		Last Modified: Tue, 19 Dec 2023 17:27:31 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfd707f03ef0ab3405a9b45e6cec06e69f42f362ca8170ed6ac867bb3cfc5`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 308.0 KB (308007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:05ae47403683229c382942e9201cc80cec5f93aff3b92fa484586d3f493da6c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65331638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491b1d0b41e609f15065b67955fa1e9ad57896dfb61a7785345b6e12ee9a3ffa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:06 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a678807dec42582e887390c579155f2ff3f3c25b0fdfeb11854c487bfc0479`  
		Last Modified: Tue, 19 Dec 2023 03:07:34 GMT  
		Size: 11.3 MB (11313652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2434d66e0ac932afe623ab8fb9ddeaf97131cee80959a55990df31cdcbf946`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8665dd0adc074adaedc5ecf6d1a9424f986359c007f4c36cbcae0e95056a940b`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9cb0c2c79d2d93968c00288fda1bdc0a21e05ec517669fe68234be55ffd271`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 307.9 KB (307878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; 386

```console
$ docker pull neurodebian@sha256:42bdac607d78c342b9d010ffbf4ab731014da1db8092747d0e8bd54e535e71ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68064908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92da83f63ff7256ee873cf328fac9c99a5068f62517bc346aa23821757a0b40b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:19 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Tue, 19 Dec 2023 01:39:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0a042ddf885a246973867761eaeb7097c4ffba0155dc9ecd3c004dd567e6d6`  
		Last Modified: Tue, 19 Dec 2023 03:52:41 GMT  
		Size: 11.7 MB (11708784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b236339ceeaafd4e56a9404e9528b71ad8f45255c5f053e303f89715c4f09bd`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca1d30df83fb1854dac8182f65566474d229cbccc4c7a4029273bddd4829d`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c554dc1a2dd646999214a1df9a3c0747d1dfb49b0931fd602f90f37f7f2ba84`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 307.8 KB (307775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:3076bd759dcaaf48c55bfbe851b186199c007138b2ffa6878b99d549c0f4cb33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:72eaa2172d7b06d9cf398c5cfebb9f5ed0ead79a19f217572c987ecc980250bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64245379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bba5e2b1186af02ec519fbc2894ba188c724776fa994fc49a039a0239492991`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:05 GMT
ADD file:0e0fcf0b6bc9c9794502332cd0f45625ac991c8a06ab284afd8673f8d5ab789c in / 
# Tue, 19 Dec 2023 01:22:06 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:26:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:26:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:26:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:716f2525263989014ccf51727e00b6ee9f74018b7b13e996b0e06409e58a44a3`  
		Last Modified: Tue, 19 Dec 2023 01:27:57 GMT  
		Size: 52.2 MB (52246819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46595495b42823cfd778cfc3563c43755220822555cb22afac60d826272f92b`  
		Last Modified: Tue, 19 Dec 2023 17:28:13 GMT  
		Size: 11.7 MB (11710401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4996e7c637126b150a9569e1dd22c978b1c1e339a6e7d0853831f7d4b7cff2d5`  
		Last Modified: Tue, 19 Dec 2023 17:28:11 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1681fc2520614d5bf50a4f35cb2b68d40484e39379bf891fbdaea3a4a8fb426d`  
		Last Modified: Tue, 19 Dec 2023 17:28:11 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10da9506cdc97636bf343b88b8f41f346687505451481b89bda91ccd5edb191`  
		Last Modified: Tue, 19 Dec 2023 17:28:12 GMT  
		Size: 286.1 KB (286148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:dc92210bca05150670c4b103f4248092b98dc9d3ea8d8950d4b449472528f49b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7beb2b34e8aab8e7bf6e1a2736a1884f078694989962ddcfc1b9c3c1a1369b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:13 GMT
ADD file:b95bf5556d43a8a1d79a2dbf26ab8a4a912869d65cc1b76a372ca80259a65b7b in / 
# Tue, 19 Dec 2023 01:42:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f38ee39d2143cc6781c8d40b267519e59c558f7902df442f2e5ecfcefb01689`  
		Last Modified: Tue, 19 Dec 2023 01:47:24 GMT  
		Size: 49.7 MB (49689786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e289d2bd50130a54f42a5188139efd22f1e4f872bf3d2ea9ee64df6bbe8a2d`  
		Last Modified: Tue, 19 Dec 2023 03:08:14 GMT  
		Size: 14.2 MB (14163608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6592770f5ba6afac48334ec1e5b9f57d99a6972ab6ea31b37e445e6ed7836a81`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b92ab013a67f046cd17d84ea7ab3e4f6eedba968eef8b8e56083974801edbb4`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c053063e1b60822a02be21a864c0d45e978a421c861555ff8a276300ea58b7`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 286.7 KB (286688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; 386

```console
$ docker pull neurodebian@sha256:d7d1f07c58b1aae651c695df84e0da0a5f8422df9601b840a9901f84e8d33a22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65577251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f217e36f8007ed868e04aabe3583cda7a03dd90f9a32f5b29e6b88c8bd7c86e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:40:47 GMT
ADD file:736d4b14c103f5161855a9c14b05565523005af03b61bcfb3d6bfaddee9431f3 in / 
# Tue, 19 Dec 2023 01:40:47 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:52:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:567001fd97421e53b722a950bba83f44d7635056bc895f0b4f77b68d779fc15e`  
		Last Modified: Tue, 19 Dec 2023 01:46:59 GMT  
		Size: 50.6 MB (50559243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d5db5fdec42c82bcc5337d39f7bf6b089a42b3787d180eedd48aaf4d4a2bb`  
		Last Modified: Tue, 19 Dec 2023 03:53:24 GMT  
		Size: 14.7 MB (14729998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9aec2cefffd0c64a74a6846300482dea9046c877c1c1559aae5523f25d8610`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58ce81bf04c62ba5934917b776534fb6478af6e9325c3ee241a2345c0d800d5`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00decda9d198acc08dcefd5412a863c2625149c3aca917edadf313f6696f075`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 286.0 KB (285999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:74c5ce132c284f42d278fffb820453094898d04f31d5e14d92248029bc0090e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:5433d59a93640547e4e4d13f12391bd44b5bb48206ddd45e1c14d2942656c94a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64245775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d02372f30baca20d5ee39f4895aaadd7beaec17985d062baaef894430312e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:05 GMT
ADD file:0e0fcf0b6bc9c9794502332cd0f45625ac991c8a06ab284afd8673f8d5ab789c in / 
# Tue, 19 Dec 2023 01:22:06 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:26:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:26:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:26:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:43 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:716f2525263989014ccf51727e00b6ee9f74018b7b13e996b0e06409e58a44a3`  
		Last Modified: Tue, 19 Dec 2023 01:27:57 GMT  
		Size: 52.2 MB (52246819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46595495b42823cfd778cfc3563c43755220822555cb22afac60d826272f92b`  
		Last Modified: Tue, 19 Dec 2023 17:28:13 GMT  
		Size: 11.7 MB (11710401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4996e7c637126b150a9569e1dd22c978b1c1e339a6e7d0853831f7d4b7cff2d5`  
		Last Modified: Tue, 19 Dec 2023 17:28:11 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1681fc2520614d5bf50a4f35cb2b68d40484e39379bf891fbdaea3a4a8fb426d`  
		Last Modified: Tue, 19 Dec 2023 17:28:11 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10da9506cdc97636bf343b88b8f41f346687505451481b89bda91ccd5edb191`  
		Last Modified: Tue, 19 Dec 2023 17:28:12 GMT  
		Size: 286.1 KB (286148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2be8bf1a62341a28a6873c460beb3f00e9256b4f65320f71d31e07630a38cf`  
		Last Modified: Tue, 19 Dec 2023 17:28:20 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:82cd99d15d3a48ea5f267295680e9de1fcc372bf0fe088b57df45b9978ab6dfb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58c971a0a9a9e11e50fbb65fc492626dcec8c326556acb8dcdd888eb23e19e65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:13 GMT
ADD file:b95bf5556d43a8a1d79a2dbf26ab8a4a912869d65cc1b76a372ca80259a65b7b in / 
# Tue, 19 Dec 2023 01:42:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:49 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:2f38ee39d2143cc6781c8d40b267519e59c558f7902df442f2e5ecfcefb01689`  
		Last Modified: Tue, 19 Dec 2023 01:47:24 GMT  
		Size: 49.7 MB (49689786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e289d2bd50130a54f42a5188139efd22f1e4f872bf3d2ea9ee64df6bbe8a2d`  
		Last Modified: Tue, 19 Dec 2023 03:08:14 GMT  
		Size: 14.2 MB (14163608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6592770f5ba6afac48334ec1e5b9f57d99a6972ab6ea31b37e445e6ed7836a81`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b92ab013a67f046cd17d84ea7ab3e4f6eedba968eef8b8e56083974801edbb4`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c053063e1b60822a02be21a864c0d45e978a421c861555ff8a276300ea58b7`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 286.7 KB (286688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69a478f4b8b4d7f1802cbc5ebb6db8b13e757c1605ab3b55293ff8f58465165`  
		Last Modified: Tue, 19 Dec 2023 03:08:22 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:94976f90e5fa87a0ed44333f409cfeeab6a7ba07db6eb883d1489cc084e394c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65577648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6efd9e9e6b90b99f7d877031cc657ed13ef8a42e944e21227291ec87c9f2833f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:40:47 GMT
ADD file:736d4b14c103f5161855a9c14b05565523005af03b61bcfb3d6bfaddee9431f3 in / 
# Tue, 19 Dec 2023 01:40:47 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:52:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:52:06 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:567001fd97421e53b722a950bba83f44d7635056bc895f0b4f77b68d779fc15e`  
		Last Modified: Tue, 19 Dec 2023 01:46:59 GMT  
		Size: 50.6 MB (50559243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d5db5fdec42c82bcc5337d39f7bf6b089a42b3787d180eedd48aaf4d4a2bb`  
		Last Modified: Tue, 19 Dec 2023 03:53:24 GMT  
		Size: 14.7 MB (14729998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9aec2cefffd0c64a74a6846300482dea9046c877c1c1559aae5523f25d8610`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58ce81bf04c62ba5934917b776534fb6478af6e9325c3ee241a2345c0d800d5`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00decda9d198acc08dcefd5412a863c2625149c3aca917edadf313f6696f075`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 286.0 KB (285999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e688bdf943114a5f9eb7b38d60a3aedc84797466a58af2a005c848c05173c0`  
		Last Modified: Tue, 19 Dec 2023 03:53:32 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100`

```console
$ docker pull neurodebian@sha256:ce0180be636220f3a87835ecb491e44dcac234df82efcbc10d099866b1617ce3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100` - linux; amd64

```console
$ docker pull neurodebian@sha256:a62b209877b5c5a25d335582b2bb1167bd12a57d812fbee47b395a35cc125699
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cec7c78b29b47c0541641b7be7d3eeacef33acddf23f606023369d26314c5c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:00 GMT
ADD file:e5e3f2fedf4fa6382f3bbf6203060ba68df1aadc7ebfa3350df20bf31b102f0e in / 
# Tue, 19 Dec 2023 01:21:01 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:27 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:29 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30b73a2ffaab3c39355a8bcc5eae8ba1465bd7d9467f197b91f7635816b16bc9`  
		Last Modified: Tue, 19 Dec 2023 01:25:58 GMT  
		Size: 50.5 MB (50500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab53549f1d6f91ce1fcfb5a6ff812ebeca69b02bd07cbe6a1ae8df426ca90a4`  
		Last Modified: Tue, 19 Dec 2023 17:27:13 GMT  
		Size: 10.5 MB (10504778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e731abcc54cf5bcb086bc36b1e6f12ad7d73ca0f0139f4a0070a16d1bb6105a`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f5821293636913a5e5f156fde6c19fb62901cbcf38d66898b3154b4222b9e4`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2c8d395609db22d85da949ac48af56210ff29e74765f2ae4f6f3dd8007e73c`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 299.4 KB (299435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:600d482db7b7f3d51d4f3421c83edcc89e1f2877a2a2eee0924eb54a7f2ae386
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60101042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a3893cecce63384e1d3f1b1992262b77aefdfae5aaba094ef03c980ff3b6a89`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:31 GMT
ADD file:df5e5dd39efc6ae3cc9132f6ca6bb569731f7a37cf4b41f87bcb7aa1ba9771e8 in / 
# Tue, 19 Dec 2023 01:41:32 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:05:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:05:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:05:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:05:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93507f9712ced9fbfd0d0f689cf7b55fb245cef88530c07ac5dc5cad20fa889d`  
		Last Modified: Tue, 19 Dec 2023 01:45:40 GMT  
		Size: 49.3 MB (49289026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c5fbc51c74a4f8750f148252ed129c0c57cc94d6e2b2f4ae83d5f1420fe9a2`  
		Last Modified: Tue, 19 Dec 2023 03:07:17 GMT  
		Size: 10.5 MB (10510551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7d0a1a828eff413800cec078c31256371b964ca8aa29198aea52bf930d8057`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dd41deea093d7e81d0007ed35420760c6cea45b552f575b45ee9e400eb7beb`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533e3cd401bcc7d93489b3ef17afb87ed22d96e3b19fb76fa2dfc90ee457c0c0`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 299.4 KB (299449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100` - linux; 386

```console
$ docker pull neurodebian@sha256:ec322aa50424cc143d1686f5c149fa6a13d427e7e3a49126580823944e5101a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff097a81fd1e52e4c0c90fb596ba089dc94e8a830bd1c10c18c463bcaca93815`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:40 GMT
ADD file:4c009b0d408e3df297246382d87b0be68c34886e13ed79ba47feb8ff51acb863 in / 
# Tue, 19 Dec 2023 01:39:41 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:50:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:50:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:50:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:50:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8d351f5ab6958b8ca5f2b8e463c49cba65be4285ead8bdbc1378b5ce2c8cd736`  
		Last Modified: Tue, 19 Dec 2023 01:44:53 GMT  
		Size: 51.3 MB (51255444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01ee695ce5b07c4aa0b90a93605547e631e728141c311b4bbf7c54fdac3be4`  
		Last Modified: Tue, 19 Dec 2023 03:52:23 GMT  
		Size: 10.9 MB (10868372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379f0dec32e0488edb8bff0dcd0be9abb4c04675943257bc5c784bfd82fd870`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56e62a0bf8c627e0bfa8f075fdfdcabfd6fc8d4809a1ec507a91d81eec6c13a`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f016555c3e2050965be5f7aece4aa1a93943629cdaa4359707eb76a9fac47534`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 299.4 KB (299418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:dc6793856187c9c39c2b66375d0c1c937b962fc9b4763e6aef88513c6022b0a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:328b5eade2581994ea8a93d00f30594ac1654d1f41755a825464613a109677dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0384483cda04a7d15823f8140de13eef8410dc29c4509077931167c9a24b790b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:00 GMT
ADD file:e5e3f2fedf4fa6382f3bbf6203060ba68df1aadc7ebfa3350df20bf31b102f0e in / 
# Tue, 19 Dec 2023 01:21:01 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:27 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:29 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:38 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:30b73a2ffaab3c39355a8bcc5eae8ba1465bd7d9467f197b91f7635816b16bc9`  
		Last Modified: Tue, 19 Dec 2023 01:25:58 GMT  
		Size: 50.5 MB (50500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab53549f1d6f91ce1fcfb5a6ff812ebeca69b02bd07cbe6a1ae8df426ca90a4`  
		Last Modified: Tue, 19 Dec 2023 17:27:13 GMT  
		Size: 10.5 MB (10504778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e731abcc54cf5bcb086bc36b1e6f12ad7d73ca0f0139f4a0070a16d1bb6105a`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f5821293636913a5e5f156fde6c19fb62901cbcf38d66898b3154b4222b9e4`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2c8d395609db22d85da949ac48af56210ff29e74765f2ae4f6f3dd8007e73c`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 299.4 KB (299435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420d51671fd62d4e126c31d4831df03a8ab2acf080c8bc83a8eb772760dedd0b`  
		Last Modified: Tue, 19 Dec 2023 17:27:23 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:f764445ceab408a8b33ff6e0e70255f357997da4ad5c15da095c4619d3778441
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60101398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bca1e9bfe9bfa37e72929b0e193a720d329783d7289784ea929d1b75eb5ac9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:31 GMT
ADD file:df5e5dd39efc6ae3cc9132f6ca6bb569731f7a37cf4b41f87bcb7aa1ba9771e8 in / 
# Tue, 19 Dec 2023 01:41:32 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:05:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:05:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:05:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:05:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:05:57 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:93507f9712ced9fbfd0d0f689cf7b55fb245cef88530c07ac5dc5cad20fa889d`  
		Last Modified: Tue, 19 Dec 2023 01:45:40 GMT  
		Size: 49.3 MB (49289026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c5fbc51c74a4f8750f148252ed129c0c57cc94d6e2b2f4ae83d5f1420fe9a2`  
		Last Modified: Tue, 19 Dec 2023 03:07:17 GMT  
		Size: 10.5 MB (10510551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7d0a1a828eff413800cec078c31256371b964ca8aa29198aea52bf930d8057`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dd41deea093d7e81d0007ed35420760c6cea45b552f575b45ee9e400eb7beb`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533e3cd401bcc7d93489b3ef17afb87ed22d96e3b19fb76fa2dfc90ee457c0c0`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 299.4 KB (299449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134eef9048535ffd6796b146e362f4919bd2130d2183feda6ba05db3dcd4df96`  
		Last Modified: Tue, 19 Dec 2023 03:07:25 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:8b36bd35183e06994e6a3ecff588a4906eca28d78ca5cb4e9f15047484150f83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3995db1af7a67fbcd53860257fab3e0fcf305561c0d2bb8d86093d9000fcf4fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:40 GMT
ADD file:4c009b0d408e3df297246382d87b0be68c34886e13ed79ba47feb8ff51acb863 in / 
# Tue, 19 Dec 2023 01:39:41 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:50:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:50:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:50:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:50:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:00 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:8d351f5ab6958b8ca5f2b8e463c49cba65be4285ead8bdbc1378b5ce2c8cd736`  
		Last Modified: Tue, 19 Dec 2023 01:44:53 GMT  
		Size: 51.3 MB (51255444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01ee695ce5b07c4aa0b90a93605547e631e728141c311b4bbf7c54fdac3be4`  
		Last Modified: Tue, 19 Dec 2023 03:52:23 GMT  
		Size: 10.9 MB (10868372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379f0dec32e0488edb8bff0dcd0be9abb4c04675943257bc5c784bfd82fd870`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56e62a0bf8c627e0bfa8f075fdfdcabfd6fc8d4809a1ec507a91d81eec6c13a`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f016555c3e2050965be5f7aece4aa1a93943629cdaa4359707eb76a9fac47534`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 299.4 KB (299418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956c541ecb88d435c686202fe372734189b393a6e7af060a508bd5cc94110ecf`  
		Last Modified: Tue, 19 Dec 2023 03:52:31 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110`

```console
$ docker pull neurodebian@sha256:7741b00acdf38fd8ca15d3ed4d201e876397f1a8e3eba11e1dced1ede42258c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110` - linux; amd64

```console
$ docker pull neurodebian@sha256:297bbad7c3560a43ad967a3e5f87ab2bc982ab94ee9ecc2821a30fabcc802056
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66679270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9605beb5a27b9108c59145e3c7d7ffac9e705cfe1f63e2fd86746f2d991ea918`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0856bfbd37c04c98dbed2cfbebaa2c7f12b11d4603e1cb62110aeede128091`  
		Last Modified: Tue, 19 Dec 2023 17:27:32 GMT  
		Size: 11.3 MB (11311904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5429bd5bea56c5bc55594233fc233733046f366dd1123c4a94b04f92f19228`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aecaaacf549bbf53913c6f0f497a5439b394e793b413c0cf0c796f9a040148`  
		Last Modified: Tue, 19 Dec 2023 17:27:31 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfd707f03ef0ab3405a9b45e6cec06e69f42f362ca8170ed6ac867bb3cfc5`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 308.0 KB (308007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:05ae47403683229c382942e9201cc80cec5f93aff3b92fa484586d3f493da6c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65331638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491b1d0b41e609f15065b67955fa1e9ad57896dfb61a7785345b6e12ee9a3ffa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:06 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a678807dec42582e887390c579155f2ff3f3c25b0fdfeb11854c487bfc0479`  
		Last Modified: Tue, 19 Dec 2023 03:07:34 GMT  
		Size: 11.3 MB (11313652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2434d66e0ac932afe623ab8fb9ddeaf97131cee80959a55990df31cdcbf946`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8665dd0adc074adaedc5ecf6d1a9424f986359c007f4c36cbcae0e95056a940b`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9cb0c2c79d2d93968c00288fda1bdc0a21e05ec517669fe68234be55ffd271`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 307.9 KB (307878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110` - linux; 386

```console
$ docker pull neurodebian@sha256:42bdac607d78c342b9d010ffbf4ab731014da1db8092747d0e8bd54e535e71ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68064908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92da83f63ff7256ee873cf328fac9c99a5068f62517bc346aa23821757a0b40b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:19 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Tue, 19 Dec 2023 01:39:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0a042ddf885a246973867761eaeb7097c4ffba0155dc9ecd3c004dd567e6d6`  
		Last Modified: Tue, 19 Dec 2023 03:52:41 GMT  
		Size: 11.7 MB (11708784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b236339ceeaafd4e56a9404e9528b71ad8f45255c5f053e303f89715c4f09bd`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca1d30df83fb1854dac8182f65566474d229cbccc4c7a4029273bddd4829d`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c554dc1a2dd646999214a1df9a3c0747d1dfb49b0931fd602f90f37f7f2ba84`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 307.8 KB (307775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:2cce0daa7423ab3c692c4904edbe4ca12a6f0bbc3a7d159b20505d0b80798dc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:62f489eb5479e968e8c7c95925b27de9a00e0c8feec115dca3360e7fc0e8577c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66679629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982a6feac3daa4329dd853bb3f5ce5e6aea98c80dff35c9a691ccc6703f6c0a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:58 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0856bfbd37c04c98dbed2cfbebaa2c7f12b11d4603e1cb62110aeede128091`  
		Last Modified: Tue, 19 Dec 2023 17:27:32 GMT  
		Size: 11.3 MB (11311904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5429bd5bea56c5bc55594233fc233733046f366dd1123c4a94b04f92f19228`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aecaaacf549bbf53913c6f0f497a5439b394e793b413c0cf0c796f9a040148`  
		Last Modified: Tue, 19 Dec 2023 17:27:31 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfd707f03ef0ab3405a9b45e6cec06e69f42f362ca8170ed6ac867bb3cfc5`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 308.0 KB (308007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe21a9c4f2844b1731353c2ccf79ed576bb765bc5854eab55e8c885e783c04d`  
		Last Modified: Tue, 19 Dec 2023 17:27:42 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:c0d28e0c05ae9c84fb89006bd6effeb566b7b36c125e840469027ac858a2fea0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65331998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e6683e8b8d8ee63d5c5efe716a4e5f08c490c43604cdb1f28350b960ae8b32`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:06 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:12 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a678807dec42582e887390c579155f2ff3f3c25b0fdfeb11854c487bfc0479`  
		Last Modified: Tue, 19 Dec 2023 03:07:34 GMT  
		Size: 11.3 MB (11313652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2434d66e0ac932afe623ab8fb9ddeaf97131cee80959a55990df31cdcbf946`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8665dd0adc074adaedc5ecf6d1a9424f986359c007f4c36cbcae0e95056a940b`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9cb0c2c79d2d93968c00288fda1bdc0a21e05ec517669fe68234be55ffd271`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 307.9 KB (307878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2849c1469b7eddd754a21b835849faa61f22936935882ba932182e1166a8e`  
		Last Modified: Tue, 19 Dec 2023 03:07:46 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:3525dcc77a6b6f044fb762f2a30c6e1d94790d1853116ce54032830935b37d73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68065268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bd45296a7a75d68f3b5963299ba70aba200d208e0dfe56532f768a6a9ee1cc0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:19 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Tue, 19 Dec 2023 01:39:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:18 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0a042ddf885a246973867761eaeb7097c4ffba0155dc9ecd3c004dd567e6d6`  
		Last Modified: Tue, 19 Dec 2023 03:52:41 GMT  
		Size: 11.7 MB (11708784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b236339ceeaafd4e56a9404e9528b71ad8f45255c5f053e303f89715c4f09bd`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca1d30df83fb1854dac8182f65566474d229cbccc4c7a4029273bddd4829d`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c554dc1a2dd646999214a1df9a3c0747d1dfb49b0931fd602f90f37f7f2ba84`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 307.8 KB (307775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b230d20e89abb46584252eccc63bcf58afb7c16c9f0fe85da93d4a3b3f28442e`  
		Last Modified: Tue, 19 Dec 2023 03:52:51 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120`

```console
$ docker pull neurodebian@sha256:e059d3fe3bee6985dfd50da7cd9745232ad1e52bf5a230d6f9cc64ca261571a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120` - linux; amd64

```console
$ docker pull neurodebian@sha256:64d743c73fb4140f5c89a065801a1011772e712da92853458cf990228120312d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61315137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a63dd830017f4581b09dca9c03a9f78e89f546056ffa78e636e5c6ca0e1fe807`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:15 GMT
ADD file:7d8adf68670e8dc2af6b8603870ea610fc65ecbb08799f2ca6a3134f5d47d289 in / 
# Tue, 19 Dec 2023 01:20:16 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:26:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:26:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:26:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bc0734b949dcdcabe5bfdf0c8b9f44491e0fce04cb10c9c6e76282b9f6abdf01`  
		Last Modified: Tue, 19 Dec 2023 01:24:35 GMT  
		Size: 49.6 MB (49561579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60813851d3d4129f056f873cc009e941a14179ae49d530351dee04ec0df8ad54`  
		Last Modified: Tue, 19 Dec 2023 17:27:54 GMT  
		Size: 11.5 MB (11463884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfe18d5147ef1fe4b9a42ed7b57ca5c19f4ebe238093c00b4b7dbe943b7016`  
		Last Modified: Tue, 19 Dec 2023 17:27:52 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de660d6bb77b3b3cc331a91c9a465ef1f3e4edbe3d63d0cbdc857fd691b63f1f`  
		Last Modified: Tue, 19 Dec 2023 17:27:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e384fde624b03e6309d39f76a15ddeff56a9ee7e8b1bf190f416e635708dcf98`  
		Last Modified: Tue, 19 Dec 2023 17:27:53 GMT  
		Size: 287.7 KB (287661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:0dc9866a07d16e6f04cf8feb788a32eda13c8343d6c5dc835760ae88ab095312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61310258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254221e8beee5a2d58e44db505f29e1bcabc70a602dd9cc2967ff64aa7914a37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:02 GMT
ADD file:412f80f75ed3e520f767e70b6b27fc81807f62fc5c6e5adf756507e33af9fa6b in / 
# Tue, 19 Dec 2023 01:41:02 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:22 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:23 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:24 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b66b4ecd3ecfb67b3b7a2a44b0199cbdfc94965c8bd3fefab75cd2e612799740`  
		Last Modified: Tue, 19 Dec 2023 01:44:14 GMT  
		Size: 49.6 MB (49592259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536d08fe62d16991ed44688b2a03cf0a9ad4c1a6a3c91a38aabff54d8dc121f2`  
		Last Modified: Tue, 19 Dec 2023 03:07:57 GMT  
		Size: 11.4 MB (11427684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17a3a06500c5196e68b32c08163cef7f17f514e1edc70f4d842ef892c4f5c5b`  
		Last Modified: Tue, 19 Dec 2023 03:07:56 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edf619636202804b32b3951669c4b66707bb7af37e67f8a0be202699c87cb64`  
		Last Modified: Tue, 19 Dec 2023 03:07:55 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dcde0e73627274650648744924524389f5a680d3b32383a3b53fe1c475259a`  
		Last Modified: Tue, 19 Dec 2023 03:07:56 GMT  
		Size: 288.3 KB (288298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120` - linux; 386

```console
$ docker pull neurodebian@sha256:13873f1f5441f485e2c264f0dec37c15a1978c08e37131667e9768217c305ea8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62756239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4efa30f46b3252fea5ffd441d5ebdd358458e292f4f7fdd6b8306f50a2793891`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:38:52 GMT
ADD file:c20aace531a43765f8c1b69c75d7f46a4ab443377a663ab47e0bb2ceb013a611 in / 
# Tue, 19 Dec 2023 01:38:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b51fe964cb335e4bc3b61dca07146c7a0aa4c31e5ae9fec90f2a950818a21a4`  
		Last Modified: Tue, 19 Dec 2023 01:43:18 GMT  
		Size: 50.6 MB (50582312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb2f81c47b7b130f3418b0d116d480499c54496b48208ed47c1d8fc839bf85d`  
		Last Modified: Tue, 19 Dec 2023 03:53:03 GMT  
		Size: 11.9 MB (11883835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a351a4d22f54a27ecd69f950120d824c9f9f5e6a6b20e9f258285459822f274`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205522c289f7b88de70a28984bb914948c84a0cc7c29500f7e1f730e0e9db0a4`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5dc22a3c30fe732622f96301ac945a4566da973563854c515b5ca6fac7855f`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 288.1 KB (288078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:0f5caf6ff3b68f1e9a1a4df0f5018df40d31e98a8b5248f6e6fa40a4cfc55f3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:ae6e1df013b07c2f8e42580da1322753030a87403dd3460b6ba33c7a78d487cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61315570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b4bd21363d3603ebce350347a80c9a2f6bd4e1aada22c9adb09370a21d04ab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:15 GMT
ADD file:7d8adf68670e8dc2af6b8603870ea610fc65ecbb08799f2ca6a3134f5d47d289 in / 
# Tue, 19 Dec 2023 01:20:16 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:26:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:26:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:26:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:19 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:bc0734b949dcdcabe5bfdf0c8b9f44491e0fce04cb10c9c6e76282b9f6abdf01`  
		Last Modified: Tue, 19 Dec 2023 01:24:35 GMT  
		Size: 49.6 MB (49561579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60813851d3d4129f056f873cc009e941a14179ae49d530351dee04ec0df8ad54`  
		Last Modified: Tue, 19 Dec 2023 17:27:54 GMT  
		Size: 11.5 MB (11463884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfe18d5147ef1fe4b9a42ed7b57ca5c19f4ebe238093c00b4b7dbe943b7016`  
		Last Modified: Tue, 19 Dec 2023 17:27:52 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de660d6bb77b3b3cc331a91c9a465ef1f3e4edbe3d63d0cbdc857fd691b63f1f`  
		Last Modified: Tue, 19 Dec 2023 17:27:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e384fde624b03e6309d39f76a15ddeff56a9ee7e8b1bf190f416e635708dcf98`  
		Last Modified: Tue, 19 Dec 2023 17:27:53 GMT  
		Size: 287.7 KB (287661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbb4d41320b96049bbafe069a4274f3ed09e0f6516709d539b0fc3096b204eb`  
		Last Modified: Tue, 19 Dec 2023 17:28:02 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:97e4b885432424139b795ac305ffa9735c8271a48c8540d8f7054494d8c8bf69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61310687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6557c9b6f643f36bfd3aecc7cd482c215de4f6ca556ef892d21dc013d02a4e08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:02 GMT
ADD file:412f80f75ed3e520f767e70b6b27fc81807f62fc5c6e5adf756507e33af9fa6b in / 
# Tue, 19 Dec 2023 01:41:02 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:22 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:23 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:24 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:31 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b66b4ecd3ecfb67b3b7a2a44b0199cbdfc94965c8bd3fefab75cd2e612799740`  
		Last Modified: Tue, 19 Dec 2023 01:44:14 GMT  
		Size: 49.6 MB (49592259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536d08fe62d16991ed44688b2a03cf0a9ad4c1a6a3c91a38aabff54d8dc121f2`  
		Last Modified: Tue, 19 Dec 2023 03:07:57 GMT  
		Size: 11.4 MB (11427684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17a3a06500c5196e68b32c08163cef7f17f514e1edc70f4d842ef892c4f5c5b`  
		Last Modified: Tue, 19 Dec 2023 03:07:56 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edf619636202804b32b3951669c4b66707bb7af37e67f8a0be202699c87cb64`  
		Last Modified: Tue, 19 Dec 2023 03:07:55 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dcde0e73627274650648744924524389f5a680d3b32383a3b53fe1c475259a`  
		Last Modified: Tue, 19 Dec 2023 03:07:56 GMT  
		Size: 288.3 KB (288298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8378c25bd9411f0a142fee243394a286cc6f1f7c217d86581f263bb24ab74ea2`  
		Last Modified: Tue, 19 Dec 2023 03:08:05 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:f99434b0d8bcbdc85a6f4a6dc4f2d572af83eb4e4a853a144933fc1e19bc4606
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62756668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d8f03971e633e63c99322029d9a69b024c210cf1bab077dfb26f38441ef4f81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:38:52 GMT
ADD file:c20aace531a43765f8c1b69c75d7f46a4ab443377a663ab47e0bb2ceb013a611 in / 
# Tue, 19 Dec 2023 01:38:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:41 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:9b51fe964cb335e4bc3b61dca07146c7a0aa4c31e5ae9fec90f2a950818a21a4`  
		Last Modified: Tue, 19 Dec 2023 01:43:18 GMT  
		Size: 50.6 MB (50582312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb2f81c47b7b130f3418b0d116d480499c54496b48208ed47c1d8fc839bf85d`  
		Last Modified: Tue, 19 Dec 2023 03:53:03 GMT  
		Size: 11.9 MB (11883835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a351a4d22f54a27ecd69f950120d824c9f9f5e6a6b20e9f258285459822f274`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205522c289f7b88de70a28984bb914948c84a0cc7c29500f7e1f730e0e9db0a4`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5dc22a3c30fe732622f96301ac945a4566da973563854c515b5ca6fac7855f`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 288.1 KB (288078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5084ee365b51d3a05cddbfc8d59c329e46ad420b9fed6adfc9993e92d775d100`  
		Last Modified: Tue, 19 Dec 2023 03:53:11 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04`

```console
$ docker pull neurodebian@sha256:0dc0c6379aa9de4c7beb314a77836296ed1b9ecec52b6e370d7d1d8fb37e8c7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd18.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:436d0f91b2596d1a67587f416d172e20ea63d2ba9fab4064134e658283be40b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31780513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e54202678ffa323cabbfa7d9142d688755ff6767f3a44607c1eb821edd05ac91`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:34:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:34:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 02 Jun 2023 01:34:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 02 Jun 2023 01:34:48 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134fd3f50024409b1b68a3a6f4702400bd9a64d841513f895cc7d024105b78cc`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 4.8 MB (4821090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc489477c8d20c6f0b75906068dc8bd8fe67e1f59f73730d062182879ae588fc`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e27f6db7ca8cf1f438fd944f25c4f24e021afb589cc28a0069a6dff45807a5`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b84f628a2b60e2cd65ca99d9064b0cf13b65787e82747dad9fa68a2e0f016`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 240.2 KB (240158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd18.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:be402681584b912cb441771e9a7e1b039e2da347fe7ebf2d1cd9f3736c2e5b4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28385506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:364f14a0ddb6cdd1d2222f8d8d1cd397a7334c3eb47c91b89028ee7a7e491380`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:45:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:45:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 01 Jun 2023 23:45:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 01 Jun 2023 23:45:57 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca58392fb171b1b6480d0e939cedf1babf2bd1d61cbc5fd8667f30d13cf1e73`  
		Last Modified: Thu, 01 Jun 2023 23:46:48 GMT  
		Size: 4.4 MB (4402672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833dbaa1fde66205ef9230adea619512493c576ac6baf435bdb3dc21e1072e1d`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a674c5e1cc8e1b1dcc8a4daacac73e2c8748f8babf74d3cfff92c15ba68e4d`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ce993d3dfac320106ebff10dddff6363ba6d572101bb95c51d321564439c7b`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 240.0 KB (240022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04-non-free`

```console
$ docker pull neurodebian@sha256:c6e4772e5c601ede7ccf289927f339f34eab81e04942d3e803f285f931926a2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd18.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:137b909d0e4c4e1c4300fa4479a22b15c053df24cbbef0f13fce395100eafa77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31780770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226a853426c1d4b6bd2f86d099a28d4c4db35b9d83d9a7021c549f5386248a11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:34:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:34:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 02 Jun 2023 01:34:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 02 Jun 2023 01:34:48 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:34:53 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134fd3f50024409b1b68a3a6f4702400bd9a64d841513f895cc7d024105b78cc`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 4.8 MB (4821090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc489477c8d20c6f0b75906068dc8bd8fe67e1f59f73730d062182879ae588fc`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e27f6db7ca8cf1f438fd944f25c4f24e021afb589cc28a0069a6dff45807a5`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b84f628a2b60e2cd65ca99d9064b0cf13b65787e82747dad9fa68a2e0f016`  
		Last Modified: Fri, 02 Jun 2023 01:35:49 GMT  
		Size: 240.2 KB (240158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e158a3949abb4a78460b0321777ca278a50c79ac290966e5d6a7f027b04e3dd`  
		Last Modified: Fri, 02 Jun 2023 01:35:57 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd18.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:edc6bddeb118195088c3f1948fdc52cc913d453e5f543927c7c89c015fe7bd6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28385761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d966d5bec6e766760870e6f4674ca17b3fe69617f78ade07c2a7b6b3154ac8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:45:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:45:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 01 Jun 2023 23:45:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 01 Jun 2023 23:45:57 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:46:00 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca58392fb171b1b6480d0e939cedf1babf2bd1d61cbc5fd8667f30d13cf1e73`  
		Last Modified: Thu, 01 Jun 2023 23:46:48 GMT  
		Size: 4.4 MB (4402672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833dbaa1fde66205ef9230adea619512493c576ac6baf435bdb3dc21e1072e1d`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a674c5e1cc8e1b1dcc8a4daacac73e2c8748f8babf74d3cfff92c15ba68e4d`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ce993d3dfac320106ebff10dddff6363ba6d572101bb95c51d321564439c7b`  
		Last Modified: Thu, 01 Jun 2023 23:46:47 GMT  
		Size: 240.0 KB (240022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350adb1f8b3dcaa1835899b2dc84ec2f5a997c31b87aa8e76470a92bc742bc7f`  
		Last Modified: Thu, 01 Jun 2023 23:46:55 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04`

```console
$ docker pull neurodebian@sha256:ba031fd6fd8d10c60789c1e1e36b0f1d6261133c9561aba991f4c34a0975e0a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd20.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:44b7d0b76bf7eecb24561da2543c6759b12e4c9c8414f1b9e78935512ad2727c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34320320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ec23d1ce12db52e245fece4cd06f6c0ffff3753f214b1c518735daeb4ee2c22`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:30:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:30:46 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 11:30:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 11:30:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e8e2de0d867ec7e11698bdb11d5da78cb7658f6585c06230c6a1c5a8a2fbbb`  
		Last Modified: Sat, 16 Dec 2023 11:31:56 GMT  
		Size: 5.5 MB (5494756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0973d4d7f63b90a4064cbde84bfe5368a09181a1fa9398b78a60dbc8e11b64ad`  
		Last Modified: Sat, 16 Dec 2023 11:31:55 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496c414a338fcd0964d5bf308922aee54df3b752acf3e50380daa1c0e0fde868`  
		Last Modified: Sat, 16 Dec 2023 11:31:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522217e64373829c117276478f35ac5b21ed22393bff75e3fce4e36b00e5eb90`  
		Last Modified: Sat, 16 Dec 2023 11:31:56 GMT  
		Size: 239.5 KB (239529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd20.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:f1141274e347e45773d8be49383336333cd34d6d95faf145db741e34a942a790
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32919471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b7457db0e6738e03edc22022e117ad4eadbd81f74b7941fe5a1a82d5edf8faa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:29:33 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:29:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:29:34 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:29:41 GMT
ADD file:9ec8b7bbb2fbc8c90f1f24e19ab22130e03be1cc4727459e1265d2ed652377a1 in / 
# Wed, 13 Dec 2023 10:29:42 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:57:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:57:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 10:57:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 10:57:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5319f8e5f3f0f8f6e663c807041d5294b7c309e06b86d115409bbdb4c9d7165`  
		Last Modified: Thu, 14 Dec 2023 13:03:55 GMT  
		Size: 27.2 MB (27203144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d82e878836647a3198acd6d3342bb489ce6f36423f93eae6fad1bcfb5f8238`  
		Last Modified: Sat, 16 Dec 2023 10:58:54 GMT  
		Size: 5.5 MB (5474754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a11c6e2465b40ebdf20e1ff87f0882767e680eb2a491f8e71c9d655a6a465d`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6297c2a11b1380ae62c841725a9a5970007e1bc75aa5a0c31304c2cb62d9b3b6`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e24ca661ae9b1e0360d4cf84cc5dbf17c22f46e6b5520ecec5c8c1341b2dca`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 239.6 KB (239564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04-non-free`

```console
$ docker pull neurodebian@sha256:28e44c247bccb216319d79168088c695113a5b4e1a60f7cb04c2d95618519750
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd20.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:b3f3cafbd80fb60d84f06cb6a850f7972632442c52fc209d483cfcce6082e00d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34320578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dcb395334cecfe02f934685afedad044adb17b32726d7d5b049a0ada8825ea3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:30:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:30:46 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 11:30:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 11:30:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:30:57 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e8e2de0d867ec7e11698bdb11d5da78cb7658f6585c06230c6a1c5a8a2fbbb`  
		Last Modified: Sat, 16 Dec 2023 11:31:56 GMT  
		Size: 5.5 MB (5494756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0973d4d7f63b90a4064cbde84bfe5368a09181a1fa9398b78a60dbc8e11b64ad`  
		Last Modified: Sat, 16 Dec 2023 11:31:55 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496c414a338fcd0964d5bf308922aee54df3b752acf3e50380daa1c0e0fde868`  
		Last Modified: Sat, 16 Dec 2023 11:31:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522217e64373829c117276478f35ac5b21ed22393bff75e3fce4e36b00e5eb90`  
		Last Modified: Sat, 16 Dec 2023 11:31:56 GMT  
		Size: 239.5 KB (239529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51570a82a6bbfd07eee978ee080dc61dfbeb817ba567432a8e90a4b696b108df`  
		Last Modified: Sat, 16 Dec 2023 11:32:04 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd20.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:2a74510ac598b775b0c5e6806309bb643c0bad336314a336a5a7012bf559d4b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32919726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc08a48952fb4706f359961b5ddaac65179ea556854ce9d6cd442162e5051057`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:29:33 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:29:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:29:34 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:29:41 GMT
ADD file:9ec8b7bbb2fbc8c90f1f24e19ab22130e03be1cc4727459e1265d2ed652377a1 in / 
# Wed, 13 Dec 2023 10:29:42 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:57:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:57:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 10:57:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 10:57:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:58:02 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:a5319f8e5f3f0f8f6e663c807041d5294b7c309e06b86d115409bbdb4c9d7165`  
		Last Modified: Thu, 14 Dec 2023 13:03:55 GMT  
		Size: 27.2 MB (27203144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d82e878836647a3198acd6d3342bb489ce6f36423f93eae6fad1bcfb5f8238`  
		Last Modified: Sat, 16 Dec 2023 10:58:54 GMT  
		Size: 5.5 MB (5474754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a11c6e2465b40ebdf20e1ff87f0882767e680eb2a491f8e71c9d655a6a465d`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6297c2a11b1380ae62c841725a9a5970007e1bc75aa5a0c31304c2cb62d9b3b6`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e24ca661ae9b1e0360d4cf84cc5dbf17c22f46e6b5520ecec5c8c1341b2dca`  
		Last Modified: Sat, 16 Dec 2023 10:58:53 GMT  
		Size: 239.6 KB (239564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6109e5cc5f76e744d01622cfd74cab3eafaa790607e4df8e93e354b23705278`  
		Last Modified: Sat, 16 Dec 2023 10:59:01 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd22.04`

```console
$ docker pull neurodebian@sha256:ba325e5e6061bf24da78c27502f503a1693550dafd14b2bd75337d06afd1053e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd22.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:832ad5e9329cae055a24b82e2614fb4260f02209aebe2b531754f1198dd3b4c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34467765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6917cbd534a78c0843fe16fe96232df45d6101582900a7bab2146c6b71b602c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:31:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:31:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 11:31:08 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 11:31:13 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62d44c808e32e3a77cd43373f0a8470fdb06d639ba026de364a97150318d33e`  
		Last Modified: Sat, 16 Dec 2023 11:32:13 GMT  
		Size: 3.8 MB (3766320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef772247763c5df1ee7d344d2f5d647e5f66c098b6331e8091e2d15b0061605f`  
		Last Modified: Sat, 16 Dec 2023 11:32:12 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d35d7275d528ee79ed8369114469886a50b319ee8c3f716790ab260e219bbb`  
		Last Modified: Sat, 16 Dec 2023 11:32:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4272c56b744309cef303df1ac073c04ce1c74bd45d3797b2325a65636469a8`  
		Last Modified: Sat, 16 Dec 2023 11:32:13 GMT  
		Size: 252.9 KB (252855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd22.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:fd8b8e62b24ae76d9c4dac845f710ff1a7d0abe1706cc06dd2fa62e0f4d6c7b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32396537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf3fceda0bd85cb6068caad7e45ce8d59a7be4541dd78511b5774bbf54ce0089`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:41:50 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:41:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:41:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:41:51 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:41:54 GMT
ADD file:50f947da69b3b6c63695be9c49eee16f7a7dcdecdceb51e5bee1609b845bf483 in / 
# Tue, 12 Dec 2023 11:41:54 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:58:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:58:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 10:58:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 10:58:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7734efb8b826f955c6a3bb51d7c84cb262d0e600ea3980f5bce69fa7f4f92d24`  
		Last Modified: Tue, 12 Dec 2023 16:00:15 GMT  
		Size: 28.4 MB (28400282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502eabb3351c24cea84fb9e5ccf4adb9d6d658b6682fcb7576fd2c82d70f7b70`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 3.7 MB (3740006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8957f77b0604cf331a09bdc53855627bc26526f149533f2960ad2dbc4b6ed32`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5c144174c37657363446c929ba2fc409d387a017fd3babb136a15836cd50ca`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c1cad4f258411c4497ccc895050e1beb7fcacf75785a4807a3f09ae6a3f`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 254.2 KB (254236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd22.04-non-free`

```console
$ docker pull neurodebian@sha256:81749d6f6e02ebab02d467e80d7d88ea6cbed6cf29cda5eaf10a7993bd9ba84d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd22.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:2fd21ffe831d7da905d87e689e4d459dc3332f35325b84286eb27a4cf5f6c4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34468022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d00d2ab78b0f1e54b1bdbe7fc8679418d930d3e1bbab0588963c3bfa5e2e1be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:31:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:31:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 11:31:08 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 11:31:13 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:31:17 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62d44c808e32e3a77cd43373f0a8470fdb06d639ba026de364a97150318d33e`  
		Last Modified: Sat, 16 Dec 2023 11:32:13 GMT  
		Size: 3.8 MB (3766320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef772247763c5df1ee7d344d2f5d647e5f66c098b6331e8091e2d15b0061605f`  
		Last Modified: Sat, 16 Dec 2023 11:32:12 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d35d7275d528ee79ed8369114469886a50b319ee8c3f716790ab260e219bbb`  
		Last Modified: Sat, 16 Dec 2023 11:32:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4272c56b744309cef303df1ac073c04ce1c74bd45d3797b2325a65636469a8`  
		Last Modified: Sat, 16 Dec 2023 11:32:13 GMT  
		Size: 252.9 KB (252855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b030e3d725500e3908775fbc82436b7e595c244fe95c9a9073fce868a116579`  
		Last Modified: Sat, 16 Dec 2023 11:32:21 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd22.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:a234f2c6b2cf65fd1c6f69b81720033f7d359058455f2c2f81c8600313be2ed7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32396794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e35742c042c1fdbcf4086c65446d3971c3686ed2d0beb5d42207d7e1457aa10`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:41:50 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:41:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:41:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:41:51 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:41:54 GMT
ADD file:50f947da69b3b6c63695be9c49eee16f7a7dcdecdceb51e5bee1609b845bf483 in / 
# Tue, 12 Dec 2023 11:41:54 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:58:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:58:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 16 Dec 2023 10:58:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 16 Dec 2023 10:58:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:58:20 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:7734efb8b826f955c6a3bb51d7c84cb262d0e600ea3980f5bce69fa7f4f92d24`  
		Last Modified: Tue, 12 Dec 2023 16:00:15 GMT  
		Size: 28.4 MB (28400282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502eabb3351c24cea84fb9e5ccf4adb9d6d658b6682fcb7576fd2c82d70f7b70`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 3.7 MB (3740006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8957f77b0604cf331a09bdc53855627bc26526f149533f2960ad2dbc4b6ed32`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5c144174c37657363446c929ba2fc409d387a017fd3babb136a15836cd50ca`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501a1c1cad4f258411c4497ccc895050e1beb7fcacf75785a4807a3f09ae6a3f`  
		Last Modified: Sat, 16 Dec 2023 10:59:09 GMT  
		Size: 254.2 KB (254236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff7723f0eeec7ac468595c47a6d85a191198efebe6eb375fde3f2712efae13`  
		Last Modified: Sat, 16 Dec 2023 10:59:17 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:non-free`

```console
$ docker pull neurodebian@sha256:2cce0daa7423ab3c692c4904edbe4ca12a6f0bbc3a7d159b20505d0b80798dc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:62f489eb5479e968e8c7c95925b27de9a00e0c8feec115dca3360e7fc0e8577c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66679629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982a6feac3daa4329dd853bb3f5ce5e6aea98c80dff35c9a691ccc6703f6c0a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:58 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0856bfbd37c04c98dbed2cfbebaa2c7f12b11d4603e1cb62110aeede128091`  
		Last Modified: Tue, 19 Dec 2023 17:27:32 GMT  
		Size: 11.3 MB (11311904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5429bd5bea56c5bc55594233fc233733046f366dd1123c4a94b04f92f19228`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aecaaacf549bbf53913c6f0f497a5439b394e793b413c0cf0c796f9a040148`  
		Last Modified: Tue, 19 Dec 2023 17:27:31 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfd707f03ef0ab3405a9b45e6cec06e69f42f362ca8170ed6ac867bb3cfc5`  
		Last Modified: Tue, 19 Dec 2023 17:27:30 GMT  
		Size: 308.0 KB (308007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe21a9c4f2844b1731353c2ccf79ed576bb765bc5854eab55e8c885e783c04d`  
		Last Modified: Tue, 19 Dec 2023 17:27:42 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:c0d28e0c05ae9c84fb89006bd6effeb566b7b36c125e840469027ac858a2fea0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65331998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e6683e8b8d8ee63d5c5efe716a4e5f08c490c43604cdb1f28350b960ae8b32`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:06 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:12 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a678807dec42582e887390c579155f2ff3f3c25b0fdfeb11854c487bfc0479`  
		Last Modified: Tue, 19 Dec 2023 03:07:34 GMT  
		Size: 11.3 MB (11313652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2434d66e0ac932afe623ab8fb9ddeaf97131cee80959a55990df31cdcbf946`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8665dd0adc074adaedc5ecf6d1a9424f986359c007f4c36cbcae0e95056a940b`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9cb0c2c79d2d93968c00288fda1bdc0a21e05ec517669fe68234be55ffd271`  
		Last Modified: Tue, 19 Dec 2023 03:07:33 GMT  
		Size: 307.9 KB (307878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2849c1469b7eddd754a21b835849faa61f22936935882ba932182e1166a8e`  
		Last Modified: Tue, 19 Dec 2023 03:07:46 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:3525dcc77a6b6f044fb762f2a30c6e1d94790d1853116ce54032830935b37d73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68065268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bd45296a7a75d68f3b5963299ba70aba200d208e0dfe56532f768a6a9ee1cc0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:19 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Tue, 19 Dec 2023 01:39:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:18 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0a042ddf885a246973867761eaeb7097c4ffba0155dc9ecd3c004dd567e6d6`  
		Last Modified: Tue, 19 Dec 2023 03:52:41 GMT  
		Size: 11.7 MB (11708784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b236339ceeaafd4e56a9404e9528b71ad8f45255c5f053e303f89715c4f09bd`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca1d30df83fb1854dac8182f65566474d229cbccc4c7a4029273bddd4829d`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c554dc1a2dd646999214a1df9a3c0747d1dfb49b0931fd602f90f37f7f2ba84`  
		Last Modified: Tue, 19 Dec 2023 03:52:39 GMT  
		Size: 307.8 KB (307775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b230d20e89abb46584252eccc63bcf58afb7c16c9f0fe85da93d4a3b3f28442e`  
		Last Modified: Tue, 19 Dec 2023 03:52:51 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:3076bd759dcaaf48c55bfbe851b186199c007138b2ffa6878b99d549c0f4cb33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:72eaa2172d7b06d9cf398c5cfebb9f5ed0ead79a19f217572c987ecc980250bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64245379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bba5e2b1186af02ec519fbc2894ba188c724776fa994fc49a039a0239492991`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:05 GMT
ADD file:0e0fcf0b6bc9c9794502332cd0f45625ac991c8a06ab284afd8673f8d5ab789c in / 
# Tue, 19 Dec 2023 01:22:06 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:26:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:26:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:26:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:716f2525263989014ccf51727e00b6ee9f74018b7b13e996b0e06409e58a44a3`  
		Last Modified: Tue, 19 Dec 2023 01:27:57 GMT  
		Size: 52.2 MB (52246819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46595495b42823cfd778cfc3563c43755220822555cb22afac60d826272f92b`  
		Last Modified: Tue, 19 Dec 2023 17:28:13 GMT  
		Size: 11.7 MB (11710401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4996e7c637126b150a9569e1dd22c978b1c1e339a6e7d0853831f7d4b7cff2d5`  
		Last Modified: Tue, 19 Dec 2023 17:28:11 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1681fc2520614d5bf50a4f35cb2b68d40484e39379bf891fbdaea3a4a8fb426d`  
		Last Modified: Tue, 19 Dec 2023 17:28:11 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10da9506cdc97636bf343b88b8f41f346687505451481b89bda91ccd5edb191`  
		Last Modified: Tue, 19 Dec 2023 17:28:12 GMT  
		Size: 286.1 KB (286148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:dc92210bca05150670c4b103f4248092b98dc9d3ea8d8950d4b449472528f49b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7beb2b34e8aab8e7bf6e1a2736a1884f078694989962ddcfc1b9c3c1a1369b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:13 GMT
ADD file:b95bf5556d43a8a1d79a2dbf26ab8a4a912869d65cc1b76a372ca80259a65b7b in / 
# Tue, 19 Dec 2023 01:42:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f38ee39d2143cc6781c8d40b267519e59c558f7902df442f2e5ecfcefb01689`  
		Last Modified: Tue, 19 Dec 2023 01:47:24 GMT  
		Size: 49.7 MB (49689786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e289d2bd50130a54f42a5188139efd22f1e4f872bf3d2ea9ee64df6bbe8a2d`  
		Last Modified: Tue, 19 Dec 2023 03:08:14 GMT  
		Size: 14.2 MB (14163608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6592770f5ba6afac48334ec1e5b9f57d99a6972ab6ea31b37e445e6ed7836a81`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b92ab013a67f046cd17d84ea7ab3e4f6eedba968eef8b8e56083974801edbb4`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c053063e1b60822a02be21a864c0d45e978a421c861555ff8a276300ea58b7`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 286.7 KB (286688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; 386

```console
$ docker pull neurodebian@sha256:d7d1f07c58b1aae651c695df84e0da0a5f8422df9601b840a9901f84e8d33a22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65577251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f217e36f8007ed868e04aabe3583cda7a03dd90f9a32f5b29e6b88c8bd7c86e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:40:47 GMT
ADD file:736d4b14c103f5161855a9c14b05565523005af03b61bcfb3d6bfaddee9431f3 in / 
# Tue, 19 Dec 2023 01:40:47 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:52:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:567001fd97421e53b722a950bba83f44d7635056bc895f0b4f77b68d779fc15e`  
		Last Modified: Tue, 19 Dec 2023 01:46:59 GMT  
		Size: 50.6 MB (50559243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d5db5fdec42c82bcc5337d39f7bf6b089a42b3787d180eedd48aaf4d4a2bb`  
		Last Modified: Tue, 19 Dec 2023 03:53:24 GMT  
		Size: 14.7 MB (14729998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9aec2cefffd0c64a74a6846300482dea9046c877c1c1559aae5523f25d8610`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58ce81bf04c62ba5934917b776534fb6478af6e9325c3ee241a2345c0d800d5`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00decda9d198acc08dcefd5412a863c2625149c3aca917edadf313f6696f075`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 286.0 KB (285999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:74c5ce132c284f42d278fffb820453094898d04f31d5e14d92248029bc0090e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:5433d59a93640547e4e4d13f12391bd44b5bb48206ddd45e1c14d2942656c94a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64245775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d02372f30baca20d5ee39f4895aaadd7beaec17985d062baaef894430312e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:05 GMT
ADD file:0e0fcf0b6bc9c9794502332cd0f45625ac991c8a06ab284afd8673f8d5ab789c in / 
# Tue, 19 Dec 2023 01:22:06 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:26:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:26:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:26:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:43 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:716f2525263989014ccf51727e00b6ee9f74018b7b13e996b0e06409e58a44a3`  
		Last Modified: Tue, 19 Dec 2023 01:27:57 GMT  
		Size: 52.2 MB (52246819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46595495b42823cfd778cfc3563c43755220822555cb22afac60d826272f92b`  
		Last Modified: Tue, 19 Dec 2023 17:28:13 GMT  
		Size: 11.7 MB (11710401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4996e7c637126b150a9569e1dd22c978b1c1e339a6e7d0853831f7d4b7cff2d5`  
		Last Modified: Tue, 19 Dec 2023 17:28:11 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1681fc2520614d5bf50a4f35cb2b68d40484e39379bf891fbdaea3a4a8fb426d`  
		Last Modified: Tue, 19 Dec 2023 17:28:11 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10da9506cdc97636bf343b88b8f41f346687505451481b89bda91ccd5edb191`  
		Last Modified: Tue, 19 Dec 2023 17:28:12 GMT  
		Size: 286.1 KB (286148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2be8bf1a62341a28a6873c460beb3f00e9256b4f65320f71d31e07630a38cf`  
		Last Modified: Tue, 19 Dec 2023 17:28:20 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:82cd99d15d3a48ea5f267295680e9de1fcc372bf0fe088b57df45b9978ab6dfb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58c971a0a9a9e11e50fbb65fc492626dcec8c326556acb8dcdd888eb23e19e65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:13 GMT
ADD file:b95bf5556d43a8a1d79a2dbf26ab8a4a912869d65cc1b76a372ca80259a65b7b in / 
# Tue, 19 Dec 2023 01:42:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:49 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:2f38ee39d2143cc6781c8d40b267519e59c558f7902df442f2e5ecfcefb01689`  
		Last Modified: Tue, 19 Dec 2023 01:47:24 GMT  
		Size: 49.7 MB (49689786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e289d2bd50130a54f42a5188139efd22f1e4f872bf3d2ea9ee64df6bbe8a2d`  
		Last Modified: Tue, 19 Dec 2023 03:08:14 GMT  
		Size: 14.2 MB (14163608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6592770f5ba6afac48334ec1e5b9f57d99a6972ab6ea31b37e445e6ed7836a81`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b92ab013a67f046cd17d84ea7ab3e4f6eedba968eef8b8e56083974801edbb4`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c053063e1b60822a02be21a864c0d45e978a421c861555ff8a276300ea58b7`  
		Last Modified: Tue, 19 Dec 2023 03:08:12 GMT  
		Size: 286.7 KB (286688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69a478f4b8b4d7f1802cbc5ebb6db8b13e757c1605ab3b55293ff8f58465165`  
		Last Modified: Tue, 19 Dec 2023 03:08:22 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:94976f90e5fa87a0ed44333f409cfeeab6a7ba07db6eb883d1489cc084e394c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65577648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6efd9e9e6b90b99f7d877031cc657ed13ef8a42e944e21227291ec87c9f2833f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:40:47 GMT
ADD file:736d4b14c103f5161855a9c14b05565523005af03b61bcfb3d6bfaddee9431f3 in / 
# Tue, 19 Dec 2023 01:40:47 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:52:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:52:06 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:567001fd97421e53b722a950bba83f44d7635056bc895f0b4f77b68d779fc15e`  
		Last Modified: Tue, 19 Dec 2023 01:46:59 GMT  
		Size: 50.6 MB (50559243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d5db5fdec42c82bcc5337d39f7bf6b089a42b3787d180eedd48aaf4d4a2bb`  
		Last Modified: Tue, 19 Dec 2023 03:53:24 GMT  
		Size: 14.7 MB (14729998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9aec2cefffd0c64a74a6846300482dea9046c877c1c1559aae5523f25d8610`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58ce81bf04c62ba5934917b776534fb6478af6e9325c3ee241a2345c0d800d5`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00decda9d198acc08dcefd5412a863c2625149c3aca917edadf313f6696f075`  
		Last Modified: Tue, 19 Dec 2023 03:53:21 GMT  
		Size: 286.0 KB (285999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e688bdf943114a5f9eb7b38d60a3aedc84797466a58af2a005c848c05173c0`  
		Last Modified: Tue, 19 Dec 2023 03:53:32 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
