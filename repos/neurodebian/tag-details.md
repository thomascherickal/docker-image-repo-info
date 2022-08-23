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
-	[`neurodebian:impish`](#neurodebianimpish)
-	[`neurodebian:impish-non-free`](#neurodebianimpish-non-free)
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
-	[`neurodebian:nd21.10`](#neurodebiannd2110)
-	[`neurodebian:nd21.10-non-free`](#neurodebiannd2110-non-free)
-	[`neurodebian:nd22.04`](#neurodebiannd2204)
-	[`neurodebian:nd22.04-non-free`](#neurodebiannd2204-non-free)
-	[`neurodebian:non-free`](#neurodebiannon-free)
-	[`neurodebian:sid`](#neurodebiansid)
-	[`neurodebian:sid-non-free`](#neurodebiansid-non-free)
-	[`neurodebian:xenial`](#neurodebianxenial)
-	[`neurodebian:xenial-non-free`](#neurodebianxenial-non-free)

## `neurodebian:bionic`

```console
$ docker pull neurodebian@sha256:9ab965459ae2bd217870be353b6f97c9471afd3714596165bb87af8e5a200660
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:b5f2aabf177e961f5a10e1aef1b67a88ea50257f5e7adb62b54d912fa6efa25c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31767824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9498ede1206c7bb1becb2bd5a3cd3d283ce41d485477a20ec6e3361262a9f1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:10:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:10:48 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:10:49 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:10:55 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc542f6a209fdc44cb2483f852cc908a5d32f220fe23e6e977b9643b2dcc099`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 4.8 MB (4815560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b60e40858b07af317895f3351764c9b61ab25d5602df053b12d72a7b1d3e7fb`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0311a98d0b14ede1e3db9b1932f26b285c4d856ab4977227253ebcf073bb5fa`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12ed6db2b1c4c9825e9af9155777566a7f5fe52a8226886ac94d141a09ee90e`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 240.1 KB (240083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:e3c9fbb356c6bcb3e38c0e5c14bd8eee04098ef82bea56f8b216175400394b08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28107710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5894ac96771951b519122f466116cf07e04f19d9d43a01b4a6ca0fd6354321c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:06:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:12 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:06:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:06:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de78e4f730cf83f3f03ca96a7f7531a6372d67935eb2637f2f3230b1c83fb6c`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 4.3 MB (4263826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b39acb592654a8c7c01dc37815f993a6304d931d7bfe43ab7d1f7f2fe942b5`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 1.6 KB (1643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4d447e4c8e7333c968cb129edb84c2f689db4d8485500970c619ffc579b3b9`  
		Last Modified: Tue, 02 Aug 2022 04:10:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca0c608f502516035d83cf6fb13c86c462da71d47f8d1373dccb0a18f6183b7`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 107.3 KB (107283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bionic-non-free`

```console
$ docker pull neurodebian@sha256:c96063b0f74ec7b62c233156fdf6abae87351f17536aa595caff129ff2daf692
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:84b2749fa94bbe07d80e5a8050387f3c0889827ddaee08985b5c3c4ad8d73a0e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31768082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21cd21c8c00bf8fe943d887ce4b7826bb43fd002a5a0529e93599f2151897f53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:10:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:10:48 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:10:49 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:10:55 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:11:05 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc542f6a209fdc44cb2483f852cc908a5d32f220fe23e6e977b9643b2dcc099`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 4.8 MB (4815560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b60e40858b07af317895f3351764c9b61ab25d5602df053b12d72a7b1d3e7fb`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0311a98d0b14ede1e3db9b1932f26b285c4d856ab4977227253ebcf073bb5fa`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12ed6db2b1c4c9825e9af9155777566a7f5fe52a8226886ac94d141a09ee90e`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 240.1 KB (240083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0477f72700b46658739abdb42d4119ede52403b342d23bac9082effed8b13`  
		Last Modified: Tue, 02 Aug 2022 05:14:37 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:538b4a3c4f05679213416c0e34106b3c53489b4ec63a71d0dd67e5046baff586
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28107966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5f8df5591bf442efc2dd206cba7f6d01c217476c97f0f758abd515935566de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:06:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:12 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:06:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:06:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:26 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de78e4f730cf83f3f03ca96a7f7531a6372d67935eb2637f2f3230b1c83fb6c`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 4.3 MB (4263826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b39acb592654a8c7c01dc37815f993a6304d931d7bfe43ab7d1f7f2fe942b5`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 1.6 KB (1643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4d447e4c8e7333c968cb129edb84c2f689db4d8485500970c619ffc579b3b9`  
		Last Modified: Tue, 02 Aug 2022 04:10:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca0c608f502516035d83cf6fb13c86c462da71d47f8d1373dccb0a18f6183b7`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 107.3 KB (107283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c136ff57d30f443e379cc670f3087bbacddb3a39822586734a72d633d9c009`  
		Last Modified: Tue, 02 Aug 2022 04:11:15 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm`

```console
$ docker pull neurodebian@sha256:c0f3913ad90b01b6c4a2b7f1d39255c5ba93f4bd4f7ba214871bf120337aff2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm` - linux; amd64

```console
$ docker pull neurodebian@sha256:e9b86a05b01bb3c13f1fbc55430a53a71ebdf56851d3e5f03a1004c828fc485f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64670529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd27b630e384cdd385cf278e33ce89c088a06229332747f55b15259410ae263d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650c798b6bdd1512fe63c6cf25cc09780086b64703ad0bc4208790384f464363`  
		Last Modified: Tue, 23 Aug 2022 03:57:58 GMT  
		Size: 11.7 MB (11650437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c927b815f82cc37ed61292156716f9fffd225fc2cc423508787a104d35b4dc`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3fffa8e969c190aadb7263dc443f80fde51e18ad3b19e797cfc97b05b69940`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca479e17c89ef83eefe0368d4c0efc753811049db26c00d5210dd776cc7ba069`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 292.3 KB (292348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:fb50057f786f4b2c6e22bbbbc35e76bdf385d4505fe805e5c74b6c583fb1e986
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64642154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d85f229e0b7f2957ef7fefd986c043647a4ae1b7fbe4236bf2054a58d5701a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:01 GMT
ADD file:66ffd29b395276f108023b4be1a449714b6fb1fcbcaf770debb7ec6910e84294 in / 
# Tue, 02 Aug 2022 00:40:02 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c76fc726ec0ec853818bf6b42fbe47810086904b89f146d4ccce624e8c5a33e2`  
		Last Modified: Tue, 02 Aug 2022 00:44:53 GMT  
		Size: 53.1 MB (53097492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b768647485ba512058dc5e8741e2633c2c824515b3df68d6bb529b00c027383b`  
		Last Modified: Tue, 02 Aug 2022 04:13:26 GMT  
		Size: 11.4 MB (11445780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eedfc078f5df40bbb0cad3dbfc969497baef9523a741429b5b2bcd493d2a5a5`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c29cbbb169da338ba631b8a90284fc7413927453ea27d1cfa4a2d378b78f71`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89968d15418e30518b52b9a088f8c53d803dcc1fb8eb40381b333d096f88bf08`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 96.9 KB (96891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; 386

```console
$ docker pull neurodebian@sha256:5eb5eb4acc8154408f13fc2a6b9ad02ceba4ae124c05666b50087a1f67df07e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65952811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cbfebda63a0d1620a55e3595e28ab380dcf1387ac32ed9b6f9fb87bfbf9049c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:38:40 GMT
ADD file:f331e5b0e8626bfcbb682d701943586f63db1ff65d9add0d94759ecaeb8c8269 in / 
# Tue, 02 Aug 2022 00:38:41 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:20:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f78c3dc38f418186e278713175ef4cfc4bc70d85867d3597da89d03b5b956170`  
		Last Modified: Tue, 02 Aug 2022 00:43:55 GMT  
		Size: 54.0 MB (53974067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae8c66b4bb8cadf4b53644ccd234088106515eb05365f06331b37d3bc5eb099`  
		Last Modified: Tue, 02 Aug 2022 16:22:18 GMT  
		Size: 11.9 MB (11879913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bde24dd5326f2de30597d887c86597ef038a904e5dd0900a9d07c4662867ff4`  
		Last Modified: Tue, 02 Aug 2022 16:22:16 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0ab6157a1370156c19d5abf99e97f661c9e34b852d02789efe28253fbc45d0`  
		Last Modified: Tue, 02 Aug 2022 16:22:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415b8ec7e6730b1e84a05a158f37b694c42ddf99177223214958b8848f205c42`  
		Last Modified: Tue, 02 Aug 2022 16:22:17 GMT  
		Size: 96.8 KB (96842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm-non-free`

```console
$ docker pull neurodebian@sha256:477de897f99c14040de7270def851b6f4472cd32da198260e63ac6c34147feee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:8e832b29196db0f32af55eda6ef202b9f4b697690e13c8ddb78ff2230d35b154
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64670889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c057e56d52e96c4c40faea2abb608948144d4234b4023acd2c846fc23125086`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:56:03 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650c798b6bdd1512fe63c6cf25cc09780086b64703ad0bc4208790384f464363`  
		Last Modified: Tue, 23 Aug 2022 03:57:58 GMT  
		Size: 11.7 MB (11650437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c927b815f82cc37ed61292156716f9fffd225fc2cc423508787a104d35b4dc`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3fffa8e969c190aadb7263dc443f80fde51e18ad3b19e797cfc97b05b69940`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca479e17c89ef83eefe0368d4c0efc753811049db26c00d5210dd776cc7ba069`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 292.3 KB (292348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a89ced0cec2c05752478822c2ef56c88dc4576dceb06e84590537f004ba6452`  
		Last Modified: Tue, 23 Aug 2022 03:58:07 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:12243140f0c0c32e932ac5086ccab8cceaf1ccaeb6f80927d572170bb422006f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64642515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712d8beae36ac59b31fe8119071ac1f76bba49ad51cb9515c2c87a7db62b929d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:01 GMT
ADD file:66ffd29b395276f108023b4be1a449714b6fb1fcbcaf770debb7ec6910e84294 in / 
# Tue, 02 Aug 2022 00:40:02 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:55 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c76fc726ec0ec853818bf6b42fbe47810086904b89f146d4ccce624e8c5a33e2`  
		Last Modified: Tue, 02 Aug 2022 00:44:53 GMT  
		Size: 53.1 MB (53097492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b768647485ba512058dc5e8741e2633c2c824515b3df68d6bb529b00c027383b`  
		Last Modified: Tue, 02 Aug 2022 04:13:26 GMT  
		Size: 11.4 MB (11445780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eedfc078f5df40bbb0cad3dbfc969497baef9523a741429b5b2bcd493d2a5a5`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c29cbbb169da338ba631b8a90284fc7413927453ea27d1cfa4a2d378b78f71`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89968d15418e30518b52b9a088f8c53d803dcc1fb8eb40381b333d096f88bf08`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 96.9 KB (96891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346e6a04f24d8d621fb9d40b0debe135c0a50185a8dacb26f023616703395642`  
		Last Modified: Tue, 02 Aug 2022 04:13:37 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:dcab9250ea1c2d1c5dafdf4bf158ea86856d45ce1d9844d9f749594e9a9ec0ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65953171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f551bfedb0e03a0e0b335b674b898c65dd08f7475d54f130f09d44aa92edfd3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:38:40 GMT
ADD file:f331e5b0e8626bfcbb682d701943586f63db1ff65d9add0d94759ecaeb8c8269 in / 
# Tue, 02 Aug 2022 00:38:41 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:20:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:20:06 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:f78c3dc38f418186e278713175ef4cfc4bc70d85867d3597da89d03b5b956170`  
		Last Modified: Tue, 02 Aug 2022 00:43:55 GMT  
		Size: 54.0 MB (53974067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae8c66b4bb8cadf4b53644ccd234088106515eb05365f06331b37d3bc5eb099`  
		Last Modified: Tue, 02 Aug 2022 16:22:18 GMT  
		Size: 11.9 MB (11879913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bde24dd5326f2de30597d887c86597ef038a904e5dd0900a9d07c4662867ff4`  
		Last Modified: Tue, 02 Aug 2022 16:22:16 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0ab6157a1370156c19d5abf99e97f661c9e34b852d02789efe28253fbc45d0`  
		Last Modified: Tue, 02 Aug 2022 16:22:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415b8ec7e6730b1e84a05a158f37b694c42ddf99177223214958b8848f205c42`  
		Last Modified: Tue, 02 Aug 2022 16:22:17 GMT  
		Size: 96.8 KB (96842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb68ac818e8338ef3401f599abe51a6f30439a03cd7bf0f913eac22f90a6a8`  
		Last Modified: Tue, 02 Aug 2022 16:22:29 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:a787fc343a73552b4731121e6f1d53aad3824d5e7ddb2a9839c0d73b9c8d92c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:925b83db7405da1325c1268ff63ca9bb5e5ac45f7240470237360854cdedc503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66631781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a07513a0a8d86c586a86d5f596f28f61be26dbab8b17d51a40c4433da577c39`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:34 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:35 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:39 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da4c47f93a29385c466f0b8d06c34810d3c2fcf6a9fd424a039d0a9dd5ba91a`  
		Last Modified: Tue, 23 Aug 2022 03:57:33 GMT  
		Size: 11.3 MB (11310656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baadeaeeef9ec92fffddaf3f7991f97f2852ce3310c7e7115279778ce1b60c23`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6357f4e4c8211177f51c1526a9d04ce62e0dd0ed3eeb6745feda9f395463d`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb160502891152d59ef71771495e79282a1d437e3a848021655e73ad1c5e6e48`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 311.6 KB (311560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5c75df0ee6ad2444b0fe68c959fad3425b088cb2f61f67f40df27d4be6a82cc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64894895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3213f95beb3a3b214f2bf9711b42adadf7f11141e22174aa8a437a59a991d3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff40e6a469794f9119b4074673af50f6e14202e8140c999b2934d90e5d334532`  
		Last Modified: Tue, 02 Aug 2022 04:12:56 GMT  
		Size: 11.1 MB (11104729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2a776b73fedde99a37ad1a5b4225e4cbc0b571fca2183b5ed2f22eb8808108`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28656afe730c0967736477f5ec1ed6f2366700ed354642dc492275fe287e71cb`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee0dbec7c4163720ac1f0d28a757f4e31c98305ec91f34c9e15dc034a6ad6b`  
		Last Modified: Tue, 02 Aug 2022 04:12:55 GMT  
		Size: 105.2 KB (105171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; 386

```console
$ docker pull neurodebian@sha256:e00517773d96d9b676da9bcb06ada35db29be58697ca84b630e3acb13a2c9303
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67608918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27ccc22c0149dda2a05324c98959c4dbaad98fd64b160a6ad1d605958bfd5515`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:05 GMT
ADD file:ade7fe80dd06354b3eab9283f6c354047be2b94806dbe1dedee8d5a0f658f7be in / 
# Tue, 02 Aug 2022 00:39:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84601b97875630e4b14ebdb276bc4c68f89eafe6d12dec64b54dbcaed7c0c802`  
		Last Modified: Tue, 02 Aug 2022 00:44:40 GMT  
		Size: 56.0 MB (56002231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27896781078532c6ddb430224d3c48f834d093e2ab3ae5ff4805af3597860da1`  
		Last Modified: Tue, 02 Aug 2022 16:21:46 GMT  
		Size: 11.5 MB (11499635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f1ce447767d12a4c29740ef298c72902b324eecc4f8f0f0c763e38c98bab6d`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a522090ef6aa533a52810a47e789f07e4c7ff1a06cd9c5191eb0feebd0fb5a`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b003d4600f8668923f8466f8795c15318ecc94ee07d7631411f57e6a5cb9e8b`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 105.1 KB (105064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:8f46a81df71a6fd6eb3e8743319ce935638ff7d4f4ba25f48c5c796651410246
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:f865df23569ce8d81cc0f8ccd3e8b33d6ccc250ae34a26352f9161e0a074215a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66632140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b60780d8b2d8dd6b19f7afa2f9602864ccf2d9aa4ceb546623604bbbfb470b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:34 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:35 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:39 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:43 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da4c47f93a29385c466f0b8d06c34810d3c2fcf6a9fd424a039d0a9dd5ba91a`  
		Last Modified: Tue, 23 Aug 2022 03:57:33 GMT  
		Size: 11.3 MB (11310656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baadeaeeef9ec92fffddaf3f7991f97f2852ce3310c7e7115279778ce1b60c23`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6357f4e4c8211177f51c1526a9d04ce62e0dd0ed3eeb6745feda9f395463d`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb160502891152d59ef71771495e79282a1d437e3a848021655e73ad1c5e6e48`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 311.6 KB (311560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d754d80adef35e288ba8c81b0c1d43a68a7a9e9ea44bc4c28954e7006e4c2ec9`  
		Last Modified: Tue, 23 Aug 2022 03:57:44 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:4a4b0248eac44e958218d5cc595b06a281d5ec394de57a48e127631d166842f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64895258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fd53427e1b819b7fefedba74bd470e4361c2d66d6458836639fd8820cfb41d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:26 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff40e6a469794f9119b4074673af50f6e14202e8140c999b2934d90e5d334532`  
		Last Modified: Tue, 02 Aug 2022 04:12:56 GMT  
		Size: 11.1 MB (11104729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2a776b73fedde99a37ad1a5b4225e4cbc0b571fca2183b5ed2f22eb8808108`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28656afe730c0967736477f5ec1ed6f2366700ed354642dc492275fe287e71cb`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee0dbec7c4163720ac1f0d28a757f4e31c98305ec91f34c9e15dc034a6ad6b`  
		Last Modified: Tue, 02 Aug 2022 04:12:55 GMT  
		Size: 105.2 KB (105171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c0342191d269718b61134e36c597d1f0c21655afbd52d6ad48fdf07054b7e`  
		Last Modified: Tue, 02 Aug 2022 04:13:10 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:e98da7e376fde4c546e16b52735e663eb876819b1795a560666f1ee80330b929
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67609277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2aa7047da75911beb318e8f6a833147b12b661ba5dae09517fd3a378231cd6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:05 GMT
ADD file:ade7fe80dd06354b3eab9283f6c354047be2b94806dbe1dedee8d5a0f658f7be in / 
# Tue, 02 Aug 2022 00:39:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:32 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:84601b97875630e4b14ebdb276bc4c68f89eafe6d12dec64b54dbcaed7c0c802`  
		Last Modified: Tue, 02 Aug 2022 00:44:40 GMT  
		Size: 56.0 MB (56002231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27896781078532c6ddb430224d3c48f834d093e2ab3ae5ff4805af3597860da1`  
		Last Modified: Tue, 02 Aug 2022 16:21:46 GMT  
		Size: 11.5 MB (11499635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f1ce447767d12a4c29740ef298c72902b324eecc4f8f0f0c763e38c98bab6d`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a522090ef6aa533a52810a47e789f07e4c7ff1a06cd9c5191eb0feebd0fb5a`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b003d4600f8668923f8466f8795c15318ecc94ee07d7631411f57e6a5cb9e8b`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 105.1 KB (105064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b434f1dc0af5922193126a834695fe056c58896604f9207fe6f1224461fb59c`  
		Last Modified: Tue, 02 Aug 2022 16:22:01 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:71a2eae8a74514991dc69475e8ea75ed2a3c387d95755c13f9b821f821f273ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:ee2c68e9b6832fba5bf06ec089492493958657068ce57cccc7adbc59f61967f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61246561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dad9ac5a38a301180d4a38e1a47f2680657dc10354b71d4dc57b78e5a8f23a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f1f3483383008e9bdfdb0946317d5a1f06e96826631b67aad6ea88390f8f59`  
		Last Modified: Tue, 23 Aug 2022 03:57:13 GMT  
		Size: 10.5 MB (10501366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f071bb9ea0575e1048a0b93e7c9f6d2471dcb313b290eb2dc170274a5627995a`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30b909f6364845c06673d20a3679be820d2b7c92fa8fdc4ddee19421c2983e4`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cb4aa9dee1e926332df8474f45adde8fc0af961f37092953110a68b479fcf9`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 302.9 KB (302910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:8a5714488c5e8b7a754867d7ee61135da10dd8d42740155a6a1014e0bb5addb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59636766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c9ba384f3c57096357f1c97b80b7cab4076da999fd61c2972f5afa7120d06f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:49 GMT
ADD file:dfd7e3791fa0512f0f7c9cc8530233d6bc1b0a586a3656fd3950ea386754808a in / 
# Tue, 02 Aug 2022 00:40:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:07:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:07:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:07:56 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:71209d5eb534b9e48223962276993c68559f68e230f73c8a0efc2a2998362bd9`  
		Last Modified: Tue, 02 Aug 2022 00:46:28 GMT  
		Size: 49.2 MB (49229053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ad9175bab50a203372a0e5e18519ece155815088752e2900f451f9dd7792de`  
		Last Modified: Tue, 02 Aug 2022 04:12:21 GMT  
		Size: 10.3 MB (10297208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527a3912e4982e1d06db4d8b2f3d684833010e1d4cfc16801787b9fed69d31a`  
		Last Modified: Tue, 02 Aug 2022 04:12:20 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4199933e5d6634a8d460a6099aa3dbadee5483211ddc926a0da379fb5e417c26`  
		Last Modified: Tue, 02 Aug 2022 04:12:18 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9418e61ef8a7313b3cf88c397a2fb0a35dfc117517fa2d0ab5366dd3e54aa80`  
		Last Modified: Tue, 02 Aug 2022 04:12:18 GMT  
		Size: 108.5 KB (108521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; 386

```console
$ docker pull neurodebian@sha256:a708ad27908b311aad7f1b1d27134cbd2043ed3a5bea0037bd1ffc2dcf09fce7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a37832cbbb9aa939def4b2ef363c946e7ed92499feedef560c0110635c3e66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:31 GMT
ADD file:a25646092eaa55ba1e77da8bf292a71c17f8f54e6fa7a3cc057a8bd7d2febd63 in / 
# Tue, 02 Aug 2022 00:39:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:18:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:18:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:18:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87423d7294b9d02dc4a6174f8947a28436937897c107e94249f27f8c987b91b5`  
		Last Modified: Tue, 02 Aug 2022 00:45:43 GMT  
		Size: 51.2 MB (51204266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bde8b75add39bff8346a40cf19a696d90f83fc7b4d1e3c035b478656d7034b7`  
		Last Modified: Tue, 02 Aug 2022 16:21:22 GMT  
		Size: 10.7 MB (10669192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc885a3a4c2e7820a9531f2e81d8567cae93afa593b55a5463ca3a7ad84eb1`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5107873d404a90d6b95e3407b818195c97a7437da9b1681d920e70b2e94752fc`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b27a5bfa9663386e2233f61f36aafa47682e7e3a82789f89f624d252b95f3db`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 108.5 KB (108479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:97c77a612d02a401333cf127744ac62e6d002423b5d6f45548dc6701c10ee8b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:661c38bb86e5ed57d24fada2eed2f6c715188910630668957c92dd3fbf8874dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61246917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ea03b70092eab2070eb14a47ae6a1c5cccdb1d7d72ba121afa69d57ae50007`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:24 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f1f3483383008e9bdfdb0946317d5a1f06e96826631b67aad6ea88390f8f59`  
		Last Modified: Tue, 23 Aug 2022 03:57:13 GMT  
		Size: 10.5 MB (10501366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f071bb9ea0575e1048a0b93e7c9f6d2471dcb313b290eb2dc170274a5627995a`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30b909f6364845c06673d20a3679be820d2b7c92fa8fdc4ddee19421c2983e4`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cb4aa9dee1e926332df8474f45adde8fc0af961f37092953110a68b479fcf9`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 302.9 KB (302910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358f39f8acf514cee19da7adbef733365b49904196581dc621ba39e8604ffb97`  
		Last Modified: Tue, 23 Aug 2022 03:57:22 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:601556c364c99a36c4755e12e45e1e77d13275fb99424f4cb21639d46736836a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59637122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45145cc49520afbfcf3356ce44e38853bd46c74239c501e67dc3348ac7238c5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:49 GMT
ADD file:dfd7e3791fa0512f0f7c9cc8530233d6bc1b0a586a3656fd3950ea386754808a in / 
# Tue, 02 Aug 2022 00:40:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:07:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:07:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:07:56 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:03 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:71209d5eb534b9e48223962276993c68559f68e230f73c8a0efc2a2998362bd9`  
		Last Modified: Tue, 02 Aug 2022 00:46:28 GMT  
		Size: 49.2 MB (49229053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ad9175bab50a203372a0e5e18519ece155815088752e2900f451f9dd7792de`  
		Last Modified: Tue, 02 Aug 2022 04:12:21 GMT  
		Size: 10.3 MB (10297208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527a3912e4982e1d06db4d8b2f3d684833010e1d4cfc16801787b9fed69d31a`  
		Last Modified: Tue, 02 Aug 2022 04:12:20 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4199933e5d6634a8d460a6099aa3dbadee5483211ddc926a0da379fb5e417c26`  
		Last Modified: Tue, 02 Aug 2022 04:12:18 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9418e61ef8a7313b3cf88c397a2fb0a35dfc117517fa2d0ab5366dd3e54aa80`  
		Last Modified: Tue, 02 Aug 2022 04:12:18 GMT  
		Size: 108.5 KB (108521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6fc2a8b0d927cb6e31155575514ce5721bdb9a7b223b2345c89c414520514a`  
		Last Modified: Tue, 02 Aug 2022 04:12:39 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:a3faa589c0f7d2376bd5144f638008ea6554c79dc1fe9d838d0490d5174a5a79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61984278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6c7186a299849c2aedce736ddefd6128bd7a701454c2782e842de93ef2a5f6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:31 GMT
ADD file:a25646092eaa55ba1e77da8bf292a71c17f8f54e6fa7a3cc057a8bd7d2febd63 in / 
# Tue, 02 Aug 2022 00:39:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:18:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:18:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:18:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:07 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:87423d7294b9d02dc4a6174f8947a28436937897c107e94249f27f8c987b91b5`  
		Last Modified: Tue, 02 Aug 2022 00:45:43 GMT  
		Size: 51.2 MB (51204266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bde8b75add39bff8346a40cf19a696d90f83fc7b4d1e3c035b478656d7034b7`  
		Last Modified: Tue, 02 Aug 2022 16:21:22 GMT  
		Size: 10.7 MB (10669192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc885a3a4c2e7820a9531f2e81d8567cae93afa593b55a5463ca3a7ad84eb1`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5107873d404a90d6b95e3407b818195c97a7437da9b1681d920e70b2e94752fc`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b27a5bfa9663386e2233f61f36aafa47682e7e3a82789f89f624d252b95f3db`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 108.5 KB (108479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3eaeb1d1d2ad5ef4049a1c039e03903213e67bc473c3462ee551e87c96e9587`  
		Last Modified: Tue, 02 Aug 2022 16:21:33 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal`

```console
$ docker pull neurodebian@sha256:014012d14722450c1ecf31613399158a79a2f4fb5499f813ace8af368ead8a4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:aa21cd8266ee48dba8c14bc51bbe83426cddd8e7b7f306752d7f4a3aa6a490a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a261e9ccff37779edee41b9e36e03bdedee1b6fb7493f9f50dfd861f030147e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:11:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:11:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:11:40 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:11:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18eb2a1e33744cf455dc8e5b43ca272348d2bb06277f449482526acd9dd2e3c7`  
		Last Modified: Tue, 02 Aug 2022 05:14:48 GMT  
		Size: 5.5 MB (5488986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718aa848cdd79073ccfb03cb65426e6111aa4a1f53798d583a2708c905adb45e`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f054786ccdc81eeb880c3863b74c837c0af9adf50199142610bbfe5517bd0e65`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8854b477ce6477f7c67f2e8049fff57e239bbd197771d9b0f02860a53a993f73`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 238.5 KB (238546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:focal` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:ea57ba9779c6719381851e9a0473064767de43873042272c4994ba3d3b320bb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32620836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b13a4b9dc8246a71c988392a50f49a49b582f6b175ac7456916e0febdfe183b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:06:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:06:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:06:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebefee5e1b9da86fcbbca29d2c03f5892fe9486f9f8f0eaa8bcf500a5b8156d3`  
		Last Modified: Tue, 02 Aug 2022 04:11:28 GMT  
		Size: 5.3 MB (5321730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6168a75c411fa9792f31df8a0462fd6eaece0c841e490727350664b64bbfaae`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb09a7a9597120a18a94eb0a6f5c3b7163a468b75d1ab5ae6d6a98140aa1222`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dce270fac0448b9538b37ff41ebbabef4503fb776a81d633757dbb19b7ad036`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 105.3 KB (105316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal-non-free`

```console
$ docker pull neurodebian@sha256:50870fcb7cd3675d44c36f2afeef868dbbce409f4044c7dcc445bba538f5c5d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:focal-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:97cd25161a5b8497ff6ee41bb32435e07376d482165a3ea9d4f5d1d6c1c364c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4e1e85d7f13b5a1992aef372fbb4c6aef09d36913adf036c0cedd027206335`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:11:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:11:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:11:40 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:11:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:11:48 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18eb2a1e33744cf455dc8e5b43ca272348d2bb06277f449482526acd9dd2e3c7`  
		Last Modified: Tue, 02 Aug 2022 05:14:48 GMT  
		Size: 5.5 MB (5488986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718aa848cdd79073ccfb03cb65426e6111aa4a1f53798d583a2708c905adb45e`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f054786ccdc81eeb880c3863b74c837c0af9adf50199142610bbfe5517bd0e65`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8854b477ce6477f7c67f2e8049fff57e239bbd197771d9b0f02860a53a993f73`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 238.5 KB (238546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006b63a9e6c106d97accf1f8d76d620462cb5aa6b149073bfe32766d8b53f8d1`  
		Last Modified: Tue, 02 Aug 2022 05:14:57 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:focal-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:ebc00ba3160adf4d00847f33e7f816eacd6cdf76f45b97bf741445e94757cb2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32621093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c84b2f66e72fd17572486826218e08d29359280850d1577b61dcb60b7b0b00b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:06:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:06:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:06:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:58 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebefee5e1b9da86fcbbca29d2c03f5892fe9486f9f8f0eaa8bcf500a5b8156d3`  
		Last Modified: Tue, 02 Aug 2022 04:11:28 GMT  
		Size: 5.3 MB (5321730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6168a75c411fa9792f31df8a0462fd6eaece0c841e490727350664b64bbfaae`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb09a7a9597120a18a94eb0a6f5c3b7163a468b75d1ab5ae6d6a98140aa1222`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dce270fac0448b9538b37ff41ebbabef4503fb776a81d633757dbb19b7ad036`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 105.3 KB (105316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0afab03236a5302ef8495cdca5dc8d773b3a75c13cc5e54d8deca5901f9a6`  
		Last Modified: Tue, 02 Aug 2022 04:11:39 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:impish`

```console
$ docker pull neurodebian@sha256:bb234b796f7d12aa085bfd99ec7b3653453c9ca31f39c7ae8b73d78761c30561
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:impish` - linux; amd64

```console
$ docker pull neurodebian@sha256:db1963ee159e0dca0159562742ad532d2a086a988b9354057ed8d77647b5e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34384580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e017fc712553f899766998fdb9db30eee355df9033c23dd72ba12b43aa47eb`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:38:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:38:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:38:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4222215fe5bb0924cc9cbcbbb6d524fc181c91b66bd31430a258a78ebce2c519`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 3.8 MB (3752244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983039d4e1a2415f0f809ddd83bcc60a90fe40cf2e2c3a4f93ded36ac4cab37a`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d378c9cd6485d098e5bcf609a3e34edc5c31a424035a4bd61de01eadbab71c6`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e2ecd075adf7f432e69fbe49ea1b42a7c15c0cf6114789b57ffa534f851834`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 250.0 KB (250036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:impish` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:e1fc2dc1b64614617f8ce4060fb2907481ab2353c8bf21c3050761a267fbd9d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32856492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3c14d270240a3fa26a0147e6dc5bb70a299f8c8e8a0b9caf2a3d0c5f8d2551`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:24 GMT
ADD file:d1932d13ea73e26ad39647db09c23895cf0644ba34851cb87e777778d59b6730 in / 
# Tue, 07 Jun 2022 01:25:24 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:09:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:09:26 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:09:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:10:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:166e0294b8df947d819744f38e21281ed5f29a2a3b19d191deee511cbfb0e473`  
		Last Modified: Tue, 07 Jun 2022 01:27:26 GMT  
		Size: 29.0 MB (29018061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fd390207922789eacc8378770b82705bf3ef6a8ee15ff29c896c4c7b3a8737`  
		Last Modified: Tue, 19 Jul 2022 20:15:09 GMT  
		Size: 3.7 MB (3726896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41123559e445d7fd43518edd8d4445a77c75c6fed0745b660394be39800e2e06`  
		Last Modified: Tue, 19 Jul 2022 20:15:07 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3949fbe2cfc1efed7983069b8e05e484d5bbe3334f54d1142a5bbb1dff8d3f`  
		Last Modified: Tue, 19 Jul 2022 20:15:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7168a0a709927f8d07cdd160accd5040d26e868fb92cc598d965c3654d28c3f`  
		Last Modified: Tue, 19 Jul 2022 20:15:08 GMT  
		Size: 109.5 KB (109547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:impish-non-free`

```console
$ docker pull neurodebian@sha256:d8dd2cc8165345590b62af26fc7a2e0df2f5060d4450b4610e7b6b23517f1535
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:impish-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:fa54f734923cf3bc814f9ca42375869480681699d414e88acb6e22b84dc40570
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34384840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a47ecb4e0e0a6f4fa722091c451eb400637d32dcf1bb57d808dcb0e1b55c994`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:38:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:38:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:38:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:53:52 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4222215fe5bb0924cc9cbcbbb6d524fc181c91b66bd31430a258a78ebce2c519`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 3.8 MB (3752244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983039d4e1a2415f0f809ddd83bcc60a90fe40cf2e2c3a4f93ded36ac4cab37a`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d378c9cd6485d098e5bcf609a3e34edc5c31a424035a4bd61de01eadbab71c6`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e2ecd075adf7f432e69fbe49ea1b42a7c15c0cf6114789b57ffa534f851834`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 250.0 KB (250036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cf61727686c8d90437ef15476fa41e9fb4a62ac20103873c80d2c3a11c3f3b`  
		Last Modified: Tue, 19 Jul 2022 19:57:02 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:impish-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:d4317d75f7993f1c0989813fb01ddb8c37b2c45f469d348b3f06cf10fb4fc29e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32856749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2014687e1f50bb858f914f8177891ca3949ae87fc8fbbd65b7b1a140b43d7e70`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:24 GMT
ADD file:d1932d13ea73e26ad39647db09c23895cf0644ba34851cb87e777778d59b6730 in / 
# Tue, 07 Jun 2022 01:25:24 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:09:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:09:26 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:09:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:10:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:10:16 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:166e0294b8df947d819744f38e21281ed5f29a2a3b19d191deee511cbfb0e473`  
		Last Modified: Tue, 07 Jun 2022 01:27:26 GMT  
		Size: 29.0 MB (29018061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fd390207922789eacc8378770b82705bf3ef6a8ee15ff29c896c4c7b3a8737`  
		Last Modified: Tue, 19 Jul 2022 20:15:09 GMT  
		Size: 3.7 MB (3726896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41123559e445d7fd43518edd8d4445a77c75c6fed0745b660394be39800e2e06`  
		Last Modified: Tue, 19 Jul 2022 20:15:07 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3949fbe2cfc1efed7983069b8e05e484d5bbe3334f54d1142a5bbb1dff8d3f`  
		Last Modified: Tue, 19 Jul 2022 20:15:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7168a0a709927f8d07cdd160accd5040d26e868fb92cc598d965c3654d28c3f`  
		Last Modified: Tue, 19 Jul 2022 20:15:08 GMT  
		Size: 109.5 KB (109547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2bd7e7df381379f1dde19c12b40e93e765871170afe519be5f19b996972af`  
		Last Modified: Tue, 19 Jul 2022 20:15:19 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:jammy`

```console
$ docker pull neurodebian@sha256:baf5f59d711b96b68a32075b8acbeb2ccab8964532f1d6537dfaab6a8899735d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy` - linux; amd64

```console
$ docker pull neurodebian@sha256:0480f6ae6d663b07a1099780dffd6e89cbabe10c12d526384d7da32d9a3acb9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34450999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fbc15d724c59441a6cd3beebd6bc516023144076e4f2a61123c1eeb5af96d4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:12:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:12:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:12:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:12:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09202f1c776958afd50a2a64423fea360c253b75477dcbc34d89bf93966c518a`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 3.8 MB (3765806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf0688d1300705116dbdedfac9df50b6133cedc3be665079dd77c7fcaf9e30d`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b9676b9f1dd5a78ad2195a513b7ff19c199b163eb36941a029e7e754a42b87`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce8c95cde21ecb9062feba61921aa4ba04124489e73edf7e98f51b8ecbc1c54`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 257.0 KB (257045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:71239ac11306e9df0dbc7f92f518661747844c5608c9d3f2cd20013b1ec5ce3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32092016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23503e08ad9a81606e7046f475b9563b32b59225ee4d6f26a039393879847e11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:07:21 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:23 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:07:24 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:07:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d10adfa05511ba6785d83dd0cbc9965a3bfa7c2e5f66b36bd9582dd28efae2`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 3.6 MB (3594085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6664f868aa1787343b46632fc0210a72d96f7f15e81c9bd46911630d2bfe64`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb6881b552e541f1b15a6156fd149417746a8d62945e4c1f4e7541577d4ba58`  
		Last Modified: Tue, 02 Aug 2022 04:11:53 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8b558fcf3bbee7daa5e75d734cddf9f5b7de2ef3952381ce23ec576ffdbf5f`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 114.8 KB (114788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:jammy-non-free`

```console
$ docker pull neurodebian@sha256:1197e00ad522be0d59bfddceb65477790419e5d78f28ef45d891f5f4ba34326e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:1e9be3aca705fffeec64d28b6887fa5e0dbd257ae13855191ca0daddb31a98b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34451255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bd4d70243f871994419f7aa9747bbcaa5d4fdd8961d5023641181d6119f3a4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:12:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:12:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:12:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:12:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:12:28 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09202f1c776958afd50a2a64423fea360c253b75477dcbc34d89bf93966c518a`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 3.8 MB (3765806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf0688d1300705116dbdedfac9df50b6133cedc3be665079dd77c7fcaf9e30d`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b9676b9f1dd5a78ad2195a513b7ff19c199b163eb36941a029e7e754a42b87`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce8c95cde21ecb9062feba61921aa4ba04124489e73edf7e98f51b8ecbc1c54`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 257.0 KB (257045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0892b7c65de090a7c4cc54770df7517af33e780fffae00e6d582aa47a3732131`  
		Last Modified: Tue, 02 Aug 2022 05:15:19 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:ee35cfb6932ff887193402b97dad1e76561d53ca7e38327ec00ca1ad1c2e9b3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32092275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41c6c08826d3bb3d12a952ab5fed7db31727ef5be49e8cd9a9dcf2c9c9d896a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:07:21 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:23 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:07:24 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:07:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:38 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d10adfa05511ba6785d83dd0cbc9965a3bfa7c2e5f66b36bd9582dd28efae2`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 3.6 MB (3594085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6664f868aa1787343b46632fc0210a72d96f7f15e81c9bd46911630d2bfe64`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb6881b552e541f1b15a6156fd149417746a8d62945e4c1f4e7541577d4ba58`  
		Last Modified: Tue, 02 Aug 2022 04:11:53 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8b558fcf3bbee7daa5e75d734cddf9f5b7de2ef3952381ce23ec576ffdbf5f`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 114.8 KB (114788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507e338e8285a94cc9f44eaccf411f4ec3a6ca2e09e4814bf97f8119e2dda481`  
		Last Modified: Tue, 02 Aug 2022 04:12:05 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:a787fc343a73552b4731121e6f1d53aad3824d5e7ddb2a9839c0d73b9c8d92c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:925b83db7405da1325c1268ff63ca9bb5e5ac45f7240470237360854cdedc503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66631781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a07513a0a8d86c586a86d5f596f28f61be26dbab8b17d51a40c4433da577c39`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:34 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:35 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:39 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da4c47f93a29385c466f0b8d06c34810d3c2fcf6a9fd424a039d0a9dd5ba91a`  
		Last Modified: Tue, 23 Aug 2022 03:57:33 GMT  
		Size: 11.3 MB (11310656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baadeaeeef9ec92fffddaf3f7991f97f2852ce3310c7e7115279778ce1b60c23`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6357f4e4c8211177f51c1526a9d04ce62e0dd0ed3eeb6745feda9f395463d`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb160502891152d59ef71771495e79282a1d437e3a848021655e73ad1c5e6e48`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 311.6 KB (311560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5c75df0ee6ad2444b0fe68c959fad3425b088cb2f61f67f40df27d4be6a82cc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64894895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3213f95beb3a3b214f2bf9711b42adadf7f11141e22174aa8a437a59a991d3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff40e6a469794f9119b4074673af50f6e14202e8140c999b2934d90e5d334532`  
		Last Modified: Tue, 02 Aug 2022 04:12:56 GMT  
		Size: 11.1 MB (11104729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2a776b73fedde99a37ad1a5b4225e4cbc0b571fca2183b5ed2f22eb8808108`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28656afe730c0967736477f5ec1ed6f2366700ed354642dc492275fe287e71cb`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee0dbec7c4163720ac1f0d28a757f4e31c98305ec91f34c9e15dc034a6ad6b`  
		Last Modified: Tue, 02 Aug 2022 04:12:55 GMT  
		Size: 105.2 KB (105171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; 386

```console
$ docker pull neurodebian@sha256:e00517773d96d9b676da9bcb06ada35db29be58697ca84b630e3acb13a2c9303
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67608918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27ccc22c0149dda2a05324c98959c4dbaad98fd64b160a6ad1d605958bfd5515`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:05 GMT
ADD file:ade7fe80dd06354b3eab9283f6c354047be2b94806dbe1dedee8d5a0f658f7be in / 
# Tue, 02 Aug 2022 00:39:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84601b97875630e4b14ebdb276bc4c68f89eafe6d12dec64b54dbcaed7c0c802`  
		Last Modified: Tue, 02 Aug 2022 00:44:40 GMT  
		Size: 56.0 MB (56002231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27896781078532c6ddb430224d3c48f834d093e2ab3ae5ff4805af3597860da1`  
		Last Modified: Tue, 02 Aug 2022 16:21:46 GMT  
		Size: 11.5 MB (11499635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f1ce447767d12a4c29740ef298c72902b324eecc4f8f0f0c763e38c98bab6d`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a522090ef6aa533a52810a47e789f07e4c7ff1a06cd9c5191eb0feebd0fb5a`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b003d4600f8668923f8466f8795c15318ecc94ee07d7631411f57e6a5cb9e8b`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 105.1 KB (105064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:d2a2ae1159e5e98fab23316b1c87251ab3148fa02bd8dc35e0b4fec3425b510c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:7273039834b88053ebeca3c10c991a96e3c9527884c5b2327829dccf9327a076
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64714411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a8a2facbac503153a56869752b3dc14c8ef1ea00d9f784e8e6720fdd67336b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:56:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:56:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:56:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:56:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154f30b7649dd9ff36175e6592055cf8360c6e985876034a2272424287be1cd7`  
		Last Modified: Tue, 23 Aug 2022 03:58:18 GMT  
		Size: 11.7 MB (11650922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c00af28db2666c58eba10693268b55f170ca7e71d33f6cfe0d665fca65b1b7`  
		Last Modified: Tue, 23 Aug 2022 03:58:16 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f335f65a3d201956ff81ba9ecd2c1f5355df35fc67a4b449123d4d0d3dbf09`  
		Last Modified: Tue, 23 Aug 2022 03:58:17 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4abb7659ae1e8863abcaf9faf27843788a20b3d8a6ab97236c67a4ab6ae8e3`  
		Last Modified: Tue, 23 Aug 2022 03:58:17 GMT  
		Size: 292.7 KB (292697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:298d06f9fede57c37c75a2a15c45e367cfc4bf149b6b161348973624740271ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64856469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3ba2c11ffb710e401d30c92bd6e56a7d6169bb48780f8039be0ce102939a6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:38 GMT
ADD file:477966410dd9e274b01740d7af857db5c024b4c4e53a5e83b5da6854d5b0c209 in / 
# Tue, 02 Aug 2022 00:41:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:09:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:09:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:09:09 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:09:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17bcb8e39c7f35480d4c2e5b46b6c0a58dac180206453cc49052707aa8053632`  
		Last Modified: Tue, 02 Aug 2022 00:48:00 GMT  
		Size: 53.3 MB (53311787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b23f22c8c00046bbf67cd59cd4f2af07dce5c5fa7a24ab5543ae0bb3564f4aa`  
		Last Modified: Tue, 02 Aug 2022 04:13:49 GMT  
		Size: 11.4 MB (11445839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155e679260259d507584bee8d944d898d1181db2db8ee4e81b619ee20fe55dd0`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe48f40923db8199277d01e875d32310e9fc5ebbf9e02ea16c1397f9c07f2479`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707dc6bc4aa4606f4136b46e3735effc8020caaff4770ef7e70e7cfdc6946bd2`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 96.9 KB (96860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; 386

```console
$ docker pull neurodebian@sha256:376dad16c227357a26b95fa5af0a5b8386173d1e79fd72c29b8796d920a58823
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66173823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91aabef4df60debd2a22d26ff5f4e921904afa674132f60afb2577aa2996cdf9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:23 GMT
ADD file:40a2042e14b22d803da216af628cd6e8603c923c4fe79ca3c4c79c95c1c1e878 in / 
# Tue, 02 Aug 2022 00:40:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:20:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:20:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:20:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:20:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ef86b631f45587b4b6d1c16b80732997a4895ae8df072b14d68c25aeff8b901e`  
		Last Modified: Tue, 02 Aug 2022 00:47:20 GMT  
		Size: 54.2 MB (54195066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad56ce46d52bfd83905b2ba1001b937d0d384c2e9f52223b216e0205c495152`  
		Last Modified: Tue, 02 Aug 2022 16:22:42 GMT  
		Size: 11.9 MB (11879907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1643e5b63805dccebfbcaa3e8093baf3557f5e2d535c490c03e1dc32589240a`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e09ccea7ebbf3f00dff13f17b94a50a8828ca7a220bc06fca82b09fd996b414`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54f18cb63a52981a30664a1778e0a688a3aa900a519ae5ca7ec36351fd2ef6`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 96.9 KB (96869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:564e706b881a6f8c317ed565e2cba68aa39a2c67520e0e57a3d1fa33f8f1c3b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:fc0676b486d9fb81a658bfb0437aad832de7cc1bd4fdb3921f046ba0a0b19e06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64714808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d38f7230946bb568bd5d6c13c5575905fb3170262c5dbe4cf23af7a0e2e6c9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:56:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:56:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:56:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:56:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:56:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154f30b7649dd9ff36175e6592055cf8360c6e985876034a2272424287be1cd7`  
		Last Modified: Tue, 23 Aug 2022 03:58:18 GMT  
		Size: 11.7 MB (11650922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c00af28db2666c58eba10693268b55f170ca7e71d33f6cfe0d665fca65b1b7`  
		Last Modified: Tue, 23 Aug 2022 03:58:16 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f335f65a3d201956ff81ba9ecd2c1f5355df35fc67a4b449123d4d0d3dbf09`  
		Last Modified: Tue, 23 Aug 2022 03:58:17 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4abb7659ae1e8863abcaf9faf27843788a20b3d8a6ab97236c67a4ab6ae8e3`  
		Last Modified: Tue, 23 Aug 2022 03:58:17 GMT  
		Size: 292.7 KB (292697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e31bea2350446c52f2efeef74112da2d2a9bb4c743a40f71aeb2974c793b3e9`  
		Last Modified: Tue, 23 Aug 2022 03:58:27 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:d6da1355fb08035ff6642e9a44a2c50f2a930512694c14d72d7730689036a5f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64856868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2239bfedc0b0b09064acc7d3944ea0e2c0af6eb2f5de108b4d1b2c6015b9469`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:38 GMT
ADD file:477966410dd9e274b01740d7af857db5c024b4c4e53a5e83b5da6854d5b0c209 in / 
# Tue, 02 Aug 2022 00:41:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:09:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:09:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:09:09 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:09:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:09:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:17bcb8e39c7f35480d4c2e5b46b6c0a58dac180206453cc49052707aa8053632`  
		Last Modified: Tue, 02 Aug 2022 00:48:00 GMT  
		Size: 53.3 MB (53311787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b23f22c8c00046bbf67cd59cd4f2af07dce5c5fa7a24ab5543ae0bb3564f4aa`  
		Last Modified: Tue, 02 Aug 2022 04:13:49 GMT  
		Size: 11.4 MB (11445839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155e679260259d507584bee8d944d898d1181db2db8ee4e81b619ee20fe55dd0`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe48f40923db8199277d01e875d32310e9fc5ebbf9e02ea16c1397f9c07f2479`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707dc6bc4aa4606f4136b46e3735effc8020caaff4770ef7e70e7cfdc6946bd2`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 96.9 KB (96860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939008275e6fc63ae497488f2dd00411fc6aebe348e916c5aa4cf8740460deee`  
		Last Modified: Tue, 02 Aug 2022 04:14:00 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:2664ba2001554b4c81910197606dbd5210149e9217d543f6b543217451c8f202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66174221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7288077efa30d1f51895d8e4c18f4f3f0de8fb4bfbc5acb06bfff49e038cc3d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:23 GMT
ADD file:40a2042e14b22d803da216af628cd6e8603c923c4fe79ca3c4c79c95c1c1e878 in / 
# Tue, 02 Aug 2022 00:40:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:20:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:20:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:20:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:20:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:20:31 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ef86b631f45587b4b6d1c16b80732997a4895ae8df072b14d68c25aeff8b901e`  
		Last Modified: Tue, 02 Aug 2022 00:47:20 GMT  
		Size: 54.2 MB (54195066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad56ce46d52bfd83905b2ba1001b937d0d384c2e9f52223b216e0205c495152`  
		Last Modified: Tue, 02 Aug 2022 16:22:42 GMT  
		Size: 11.9 MB (11879907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1643e5b63805dccebfbcaa3e8093baf3557f5e2d535c490c03e1dc32589240a`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e09ccea7ebbf3f00dff13f17b94a50a8828ca7a220bc06fca82b09fd996b414`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54f18cb63a52981a30664a1778e0a688a3aa900a519ae5ca7ec36351fd2ef6`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 96.9 KB (96869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b198f0f40db6b4de8cb7252ebc6718942cb14b2fbd559aebb205f5dc5301217`  
		Last Modified: Tue, 02 Aug 2022 16:22:53 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100`

```console
$ docker pull neurodebian@sha256:71a2eae8a74514991dc69475e8ea75ed2a3c387d95755c13f9b821f821f273ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100` - linux; amd64

```console
$ docker pull neurodebian@sha256:ee2c68e9b6832fba5bf06ec089492493958657068ce57cccc7adbc59f61967f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61246561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dad9ac5a38a301180d4a38e1a47f2680657dc10354b71d4dc57b78e5a8f23a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f1f3483383008e9bdfdb0946317d5a1f06e96826631b67aad6ea88390f8f59`  
		Last Modified: Tue, 23 Aug 2022 03:57:13 GMT  
		Size: 10.5 MB (10501366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f071bb9ea0575e1048a0b93e7c9f6d2471dcb313b290eb2dc170274a5627995a`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30b909f6364845c06673d20a3679be820d2b7c92fa8fdc4ddee19421c2983e4`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cb4aa9dee1e926332df8474f45adde8fc0af961f37092953110a68b479fcf9`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 302.9 KB (302910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:8a5714488c5e8b7a754867d7ee61135da10dd8d42740155a6a1014e0bb5addb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59636766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c9ba384f3c57096357f1c97b80b7cab4076da999fd61c2972f5afa7120d06f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:49 GMT
ADD file:dfd7e3791fa0512f0f7c9cc8530233d6bc1b0a586a3656fd3950ea386754808a in / 
# Tue, 02 Aug 2022 00:40:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:07:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:07:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:07:56 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:71209d5eb534b9e48223962276993c68559f68e230f73c8a0efc2a2998362bd9`  
		Last Modified: Tue, 02 Aug 2022 00:46:28 GMT  
		Size: 49.2 MB (49229053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ad9175bab50a203372a0e5e18519ece155815088752e2900f451f9dd7792de`  
		Last Modified: Tue, 02 Aug 2022 04:12:21 GMT  
		Size: 10.3 MB (10297208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527a3912e4982e1d06db4d8b2f3d684833010e1d4cfc16801787b9fed69d31a`  
		Last Modified: Tue, 02 Aug 2022 04:12:20 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4199933e5d6634a8d460a6099aa3dbadee5483211ddc926a0da379fb5e417c26`  
		Last Modified: Tue, 02 Aug 2022 04:12:18 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9418e61ef8a7313b3cf88c397a2fb0a35dfc117517fa2d0ab5366dd3e54aa80`  
		Last Modified: Tue, 02 Aug 2022 04:12:18 GMT  
		Size: 108.5 KB (108521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100` - linux; 386

```console
$ docker pull neurodebian@sha256:a708ad27908b311aad7f1b1d27134cbd2043ed3a5bea0037bd1ffc2dcf09fce7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a37832cbbb9aa939def4b2ef363c946e7ed92499feedef560c0110635c3e66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:31 GMT
ADD file:a25646092eaa55ba1e77da8bf292a71c17f8f54e6fa7a3cc057a8bd7d2febd63 in / 
# Tue, 02 Aug 2022 00:39:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:18:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:18:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:18:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87423d7294b9d02dc4a6174f8947a28436937897c107e94249f27f8c987b91b5`  
		Last Modified: Tue, 02 Aug 2022 00:45:43 GMT  
		Size: 51.2 MB (51204266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bde8b75add39bff8346a40cf19a696d90f83fc7b4d1e3c035b478656d7034b7`  
		Last Modified: Tue, 02 Aug 2022 16:21:22 GMT  
		Size: 10.7 MB (10669192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc885a3a4c2e7820a9531f2e81d8567cae93afa593b55a5463ca3a7ad84eb1`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5107873d404a90d6b95e3407b818195c97a7437da9b1681d920e70b2e94752fc`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b27a5bfa9663386e2233f61f36aafa47682e7e3a82789f89f624d252b95f3db`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 108.5 KB (108479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:97c77a612d02a401333cf127744ac62e6d002423b5d6f45548dc6701c10ee8b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:661c38bb86e5ed57d24fada2eed2f6c715188910630668957c92dd3fbf8874dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61246917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ea03b70092eab2070eb14a47ae6a1c5cccdb1d7d72ba121afa69d57ae50007`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:24 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f1f3483383008e9bdfdb0946317d5a1f06e96826631b67aad6ea88390f8f59`  
		Last Modified: Tue, 23 Aug 2022 03:57:13 GMT  
		Size: 10.5 MB (10501366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f071bb9ea0575e1048a0b93e7c9f6d2471dcb313b290eb2dc170274a5627995a`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30b909f6364845c06673d20a3679be820d2b7c92fa8fdc4ddee19421c2983e4`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cb4aa9dee1e926332df8474f45adde8fc0af961f37092953110a68b479fcf9`  
		Last Modified: Tue, 23 Aug 2022 03:57:12 GMT  
		Size: 302.9 KB (302910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358f39f8acf514cee19da7adbef733365b49904196581dc621ba39e8604ffb97`  
		Last Modified: Tue, 23 Aug 2022 03:57:22 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:601556c364c99a36c4755e12e45e1e77d13275fb99424f4cb21639d46736836a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59637122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45145cc49520afbfcf3356ce44e38853bd46c74239c501e67dc3348ac7238c5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:49 GMT
ADD file:dfd7e3791fa0512f0f7c9cc8530233d6bc1b0a586a3656fd3950ea386754808a in / 
# Tue, 02 Aug 2022 00:40:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:07:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:51 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:07:52 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:07:56 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:03 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:71209d5eb534b9e48223962276993c68559f68e230f73c8a0efc2a2998362bd9`  
		Last Modified: Tue, 02 Aug 2022 00:46:28 GMT  
		Size: 49.2 MB (49229053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ad9175bab50a203372a0e5e18519ece155815088752e2900f451f9dd7792de`  
		Last Modified: Tue, 02 Aug 2022 04:12:21 GMT  
		Size: 10.3 MB (10297208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527a3912e4982e1d06db4d8b2f3d684833010e1d4cfc16801787b9fed69d31a`  
		Last Modified: Tue, 02 Aug 2022 04:12:20 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4199933e5d6634a8d460a6099aa3dbadee5483211ddc926a0da379fb5e417c26`  
		Last Modified: Tue, 02 Aug 2022 04:12:18 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9418e61ef8a7313b3cf88c397a2fb0a35dfc117517fa2d0ab5366dd3e54aa80`  
		Last Modified: Tue, 02 Aug 2022 04:12:18 GMT  
		Size: 108.5 KB (108521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6fc2a8b0d927cb6e31155575514ce5721bdb9a7b223b2345c89c414520514a`  
		Last Modified: Tue, 02 Aug 2022 04:12:39 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:a3faa589c0f7d2376bd5144f638008ea6554c79dc1fe9d838d0490d5174a5a79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61984278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6c7186a299849c2aedce736ddefd6128bd7a701454c2782e842de93ef2a5f6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:31 GMT
ADD file:a25646092eaa55ba1e77da8bf292a71c17f8f54e6fa7a3cc057a8bd7d2febd63 in / 
# Tue, 02 Aug 2022 00:39:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:18:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:18:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:18:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:07 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:87423d7294b9d02dc4a6174f8947a28436937897c107e94249f27f8c987b91b5`  
		Last Modified: Tue, 02 Aug 2022 00:45:43 GMT  
		Size: 51.2 MB (51204266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bde8b75add39bff8346a40cf19a696d90f83fc7b4d1e3c035b478656d7034b7`  
		Last Modified: Tue, 02 Aug 2022 16:21:22 GMT  
		Size: 10.7 MB (10669192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc885a3a4c2e7820a9531f2e81d8567cae93afa593b55a5463ca3a7ad84eb1`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5107873d404a90d6b95e3407b818195c97a7437da9b1681d920e70b2e94752fc`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b27a5bfa9663386e2233f61f36aafa47682e7e3a82789f89f624d252b95f3db`  
		Last Modified: Tue, 02 Aug 2022 16:21:19 GMT  
		Size: 108.5 KB (108479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3eaeb1d1d2ad5ef4049a1c039e03903213e67bc473c3462ee551e87c96e9587`  
		Last Modified: Tue, 02 Aug 2022 16:21:33 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110`

```console
$ docker pull neurodebian@sha256:a787fc343a73552b4731121e6f1d53aad3824d5e7ddb2a9839c0d73b9c8d92c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110` - linux; amd64

```console
$ docker pull neurodebian@sha256:925b83db7405da1325c1268ff63ca9bb5e5ac45f7240470237360854cdedc503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66631781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a07513a0a8d86c586a86d5f596f28f61be26dbab8b17d51a40c4433da577c39`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:34 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:35 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:39 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da4c47f93a29385c466f0b8d06c34810d3c2fcf6a9fd424a039d0a9dd5ba91a`  
		Last Modified: Tue, 23 Aug 2022 03:57:33 GMT  
		Size: 11.3 MB (11310656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baadeaeeef9ec92fffddaf3f7991f97f2852ce3310c7e7115279778ce1b60c23`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6357f4e4c8211177f51c1526a9d04ce62e0dd0ed3eeb6745feda9f395463d`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb160502891152d59ef71771495e79282a1d437e3a848021655e73ad1c5e6e48`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 311.6 KB (311560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5c75df0ee6ad2444b0fe68c959fad3425b088cb2f61f67f40df27d4be6a82cc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64894895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3213f95beb3a3b214f2bf9711b42adadf7f11141e22174aa8a437a59a991d3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff40e6a469794f9119b4074673af50f6e14202e8140c999b2934d90e5d334532`  
		Last Modified: Tue, 02 Aug 2022 04:12:56 GMT  
		Size: 11.1 MB (11104729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2a776b73fedde99a37ad1a5b4225e4cbc0b571fca2183b5ed2f22eb8808108`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28656afe730c0967736477f5ec1ed6f2366700ed354642dc492275fe287e71cb`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee0dbec7c4163720ac1f0d28a757f4e31c98305ec91f34c9e15dc034a6ad6b`  
		Last Modified: Tue, 02 Aug 2022 04:12:55 GMT  
		Size: 105.2 KB (105171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110` - linux; 386

```console
$ docker pull neurodebian@sha256:e00517773d96d9b676da9bcb06ada35db29be58697ca84b630e3acb13a2c9303
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67608918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27ccc22c0149dda2a05324c98959c4dbaad98fd64b160a6ad1d605958bfd5515`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:05 GMT
ADD file:ade7fe80dd06354b3eab9283f6c354047be2b94806dbe1dedee8d5a0f658f7be in / 
# Tue, 02 Aug 2022 00:39:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84601b97875630e4b14ebdb276bc4c68f89eafe6d12dec64b54dbcaed7c0c802`  
		Last Modified: Tue, 02 Aug 2022 00:44:40 GMT  
		Size: 56.0 MB (56002231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27896781078532c6ddb430224d3c48f834d093e2ab3ae5ff4805af3597860da1`  
		Last Modified: Tue, 02 Aug 2022 16:21:46 GMT  
		Size: 11.5 MB (11499635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f1ce447767d12a4c29740ef298c72902b324eecc4f8f0f0c763e38c98bab6d`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a522090ef6aa533a52810a47e789f07e4c7ff1a06cd9c5191eb0feebd0fb5a`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b003d4600f8668923f8466f8795c15318ecc94ee07d7631411f57e6a5cb9e8b`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 105.1 KB (105064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:8f46a81df71a6fd6eb3e8743319ce935638ff7d4f4ba25f48c5c796651410246
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:f865df23569ce8d81cc0f8ccd3e8b33d6ccc250ae34a26352f9161e0a074215a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66632140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b60780d8b2d8dd6b19f7afa2f9602864ccf2d9aa4ceb546623604bbbfb470b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:34 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:35 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:39 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:43 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da4c47f93a29385c466f0b8d06c34810d3c2fcf6a9fd424a039d0a9dd5ba91a`  
		Last Modified: Tue, 23 Aug 2022 03:57:33 GMT  
		Size: 11.3 MB (11310656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baadeaeeef9ec92fffddaf3f7991f97f2852ce3310c7e7115279778ce1b60c23`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6357f4e4c8211177f51c1526a9d04ce62e0dd0ed3eeb6745feda9f395463d`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb160502891152d59ef71771495e79282a1d437e3a848021655e73ad1c5e6e48`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 311.6 KB (311560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d754d80adef35e288ba8c81b0c1d43a68a7a9e9ea44bc4c28954e7006e4c2ec9`  
		Last Modified: Tue, 23 Aug 2022 03:57:44 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:4a4b0248eac44e958218d5cc595b06a281d5ec394de57a48e127631d166842f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64895258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fd53427e1b819b7fefedba74bd470e4361c2d66d6458836639fd8820cfb41d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:26 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff40e6a469794f9119b4074673af50f6e14202e8140c999b2934d90e5d334532`  
		Last Modified: Tue, 02 Aug 2022 04:12:56 GMT  
		Size: 11.1 MB (11104729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2a776b73fedde99a37ad1a5b4225e4cbc0b571fca2183b5ed2f22eb8808108`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28656afe730c0967736477f5ec1ed6f2366700ed354642dc492275fe287e71cb`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee0dbec7c4163720ac1f0d28a757f4e31c98305ec91f34c9e15dc034a6ad6b`  
		Last Modified: Tue, 02 Aug 2022 04:12:55 GMT  
		Size: 105.2 KB (105171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c0342191d269718b61134e36c597d1f0c21655afbd52d6ad48fdf07054b7e`  
		Last Modified: Tue, 02 Aug 2022 04:13:10 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:e98da7e376fde4c546e16b52735e663eb876819b1795a560666f1ee80330b929
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67609277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2aa7047da75911beb318e8f6a833147b12b661ba5dae09517fd3a378231cd6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:05 GMT
ADD file:ade7fe80dd06354b3eab9283f6c354047be2b94806dbe1dedee8d5a0f658f7be in / 
# Tue, 02 Aug 2022 00:39:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:32 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:84601b97875630e4b14ebdb276bc4c68f89eafe6d12dec64b54dbcaed7c0c802`  
		Last Modified: Tue, 02 Aug 2022 00:44:40 GMT  
		Size: 56.0 MB (56002231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27896781078532c6ddb430224d3c48f834d093e2ab3ae5ff4805af3597860da1`  
		Last Modified: Tue, 02 Aug 2022 16:21:46 GMT  
		Size: 11.5 MB (11499635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f1ce447767d12a4c29740ef298c72902b324eecc4f8f0f0c763e38c98bab6d`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a522090ef6aa533a52810a47e789f07e4c7ff1a06cd9c5191eb0feebd0fb5a`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b003d4600f8668923f8466f8795c15318ecc94ee07d7631411f57e6a5cb9e8b`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 105.1 KB (105064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b434f1dc0af5922193126a834695fe056c58896604f9207fe6f1224461fb59c`  
		Last Modified: Tue, 02 Aug 2022 16:22:01 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120`

```console
$ docker pull neurodebian@sha256:c0f3913ad90b01b6c4a2b7f1d39255c5ba93f4bd4f7ba214871bf120337aff2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120` - linux; amd64

```console
$ docker pull neurodebian@sha256:e9b86a05b01bb3c13f1fbc55430a53a71ebdf56851d3e5f03a1004c828fc485f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64670529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd27b630e384cdd385cf278e33ce89c088a06229332747f55b15259410ae263d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650c798b6bdd1512fe63c6cf25cc09780086b64703ad0bc4208790384f464363`  
		Last Modified: Tue, 23 Aug 2022 03:57:58 GMT  
		Size: 11.7 MB (11650437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c927b815f82cc37ed61292156716f9fffd225fc2cc423508787a104d35b4dc`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3fffa8e969c190aadb7263dc443f80fde51e18ad3b19e797cfc97b05b69940`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca479e17c89ef83eefe0368d4c0efc753811049db26c00d5210dd776cc7ba069`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 292.3 KB (292348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:fb50057f786f4b2c6e22bbbbc35e76bdf385d4505fe805e5c74b6c583fb1e986
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64642154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d85f229e0b7f2957ef7fefd986c043647a4ae1b7fbe4236bf2054a58d5701a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:01 GMT
ADD file:66ffd29b395276f108023b4be1a449714b6fb1fcbcaf770debb7ec6910e84294 in / 
# Tue, 02 Aug 2022 00:40:02 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c76fc726ec0ec853818bf6b42fbe47810086904b89f146d4ccce624e8c5a33e2`  
		Last Modified: Tue, 02 Aug 2022 00:44:53 GMT  
		Size: 53.1 MB (53097492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b768647485ba512058dc5e8741e2633c2c824515b3df68d6bb529b00c027383b`  
		Last Modified: Tue, 02 Aug 2022 04:13:26 GMT  
		Size: 11.4 MB (11445780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eedfc078f5df40bbb0cad3dbfc969497baef9523a741429b5b2bcd493d2a5a5`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c29cbbb169da338ba631b8a90284fc7413927453ea27d1cfa4a2d378b78f71`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89968d15418e30518b52b9a088f8c53d803dcc1fb8eb40381b333d096f88bf08`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 96.9 KB (96891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120` - linux; 386

```console
$ docker pull neurodebian@sha256:5eb5eb4acc8154408f13fc2a6b9ad02ceba4ae124c05666b50087a1f67df07e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65952811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cbfebda63a0d1620a55e3595e28ab380dcf1387ac32ed9b6f9fb87bfbf9049c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:38:40 GMT
ADD file:f331e5b0e8626bfcbb682d701943586f63db1ff65d9add0d94759ecaeb8c8269 in / 
# Tue, 02 Aug 2022 00:38:41 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:20:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f78c3dc38f418186e278713175ef4cfc4bc70d85867d3597da89d03b5b956170`  
		Last Modified: Tue, 02 Aug 2022 00:43:55 GMT  
		Size: 54.0 MB (53974067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae8c66b4bb8cadf4b53644ccd234088106515eb05365f06331b37d3bc5eb099`  
		Last Modified: Tue, 02 Aug 2022 16:22:18 GMT  
		Size: 11.9 MB (11879913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bde24dd5326f2de30597d887c86597ef038a904e5dd0900a9d07c4662867ff4`  
		Last Modified: Tue, 02 Aug 2022 16:22:16 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0ab6157a1370156c19d5abf99e97f661c9e34b852d02789efe28253fbc45d0`  
		Last Modified: Tue, 02 Aug 2022 16:22:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415b8ec7e6730b1e84a05a158f37b694c42ddf99177223214958b8848f205c42`  
		Last Modified: Tue, 02 Aug 2022 16:22:17 GMT  
		Size: 96.8 KB (96842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:477de897f99c14040de7270def851b6f4472cd32da198260e63ac6c34147feee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:8e832b29196db0f32af55eda6ef202b9f4b697690e13c8ddb78ff2230d35b154
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64670889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c057e56d52e96c4c40faea2abb608948144d4234b4023acd2c846fc23125086`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:56:03 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650c798b6bdd1512fe63c6cf25cc09780086b64703ad0bc4208790384f464363`  
		Last Modified: Tue, 23 Aug 2022 03:57:58 GMT  
		Size: 11.7 MB (11650437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c927b815f82cc37ed61292156716f9fffd225fc2cc423508787a104d35b4dc`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3fffa8e969c190aadb7263dc443f80fde51e18ad3b19e797cfc97b05b69940`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca479e17c89ef83eefe0368d4c0efc753811049db26c00d5210dd776cc7ba069`  
		Last Modified: Tue, 23 Aug 2022 03:57:56 GMT  
		Size: 292.3 KB (292348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a89ced0cec2c05752478822c2ef56c88dc4576dceb06e84590537f004ba6452`  
		Last Modified: Tue, 23 Aug 2022 03:58:07 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:12243140f0c0c32e932ac5086ccab8cceaf1ccaeb6f80927d572170bb422006f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64642515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712d8beae36ac59b31fe8119071ac1f76bba49ad51cb9515c2c87a7db62b929d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:01 GMT
ADD file:66ffd29b395276f108023b4be1a449714b6fb1fcbcaf770debb7ec6910e84294 in / 
# Tue, 02 Aug 2022 00:40:02 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:55 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c76fc726ec0ec853818bf6b42fbe47810086904b89f146d4ccce624e8c5a33e2`  
		Last Modified: Tue, 02 Aug 2022 00:44:53 GMT  
		Size: 53.1 MB (53097492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b768647485ba512058dc5e8741e2633c2c824515b3df68d6bb529b00c027383b`  
		Last Modified: Tue, 02 Aug 2022 04:13:26 GMT  
		Size: 11.4 MB (11445780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eedfc078f5df40bbb0cad3dbfc969497baef9523a741429b5b2bcd493d2a5a5`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c29cbbb169da338ba631b8a90284fc7413927453ea27d1cfa4a2d378b78f71`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89968d15418e30518b52b9a088f8c53d803dcc1fb8eb40381b333d096f88bf08`  
		Last Modified: Tue, 02 Aug 2022 04:13:25 GMT  
		Size: 96.9 KB (96891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346e6a04f24d8d621fb9d40b0debe135c0a50185a8dacb26f023616703395642`  
		Last Modified: Tue, 02 Aug 2022 04:13:37 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:dcab9250ea1c2d1c5dafdf4bf158ea86856d45ce1d9844d9f749594e9a9ec0ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65953171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f551bfedb0e03a0e0b335b674b898c65dd08f7475d54f130f09d44aa92edfd3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:38:40 GMT
ADD file:f331e5b0e8626bfcbb682d701943586f63db1ff65d9add0d94759ecaeb8c8269 in / 
# Tue, 02 Aug 2022 00:38:41 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:20:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:20:06 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:f78c3dc38f418186e278713175ef4cfc4bc70d85867d3597da89d03b5b956170`  
		Last Modified: Tue, 02 Aug 2022 00:43:55 GMT  
		Size: 54.0 MB (53974067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae8c66b4bb8cadf4b53644ccd234088106515eb05365f06331b37d3bc5eb099`  
		Last Modified: Tue, 02 Aug 2022 16:22:18 GMT  
		Size: 11.9 MB (11879913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bde24dd5326f2de30597d887c86597ef038a904e5dd0900a9d07c4662867ff4`  
		Last Modified: Tue, 02 Aug 2022 16:22:16 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0ab6157a1370156c19d5abf99e97f661c9e34b852d02789efe28253fbc45d0`  
		Last Modified: Tue, 02 Aug 2022 16:22:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415b8ec7e6730b1e84a05a158f37b694c42ddf99177223214958b8848f205c42`  
		Last Modified: Tue, 02 Aug 2022 16:22:17 GMT  
		Size: 96.8 KB (96842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb68ac818e8338ef3401f599abe51a6f30439a03cd7bf0f913eac22f90a6a8`  
		Last Modified: Tue, 02 Aug 2022 16:22:29 GMT  
		Size: 360.0 B  
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
$ docker pull neurodebian@sha256:9ab965459ae2bd217870be353b6f97c9471afd3714596165bb87af8e5a200660
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd18.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:b5f2aabf177e961f5a10e1aef1b67a88ea50257f5e7adb62b54d912fa6efa25c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31767824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9498ede1206c7bb1becb2bd5a3cd3d283ce41d485477a20ec6e3361262a9f1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:10:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:10:48 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:10:49 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:10:55 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc542f6a209fdc44cb2483f852cc908a5d32f220fe23e6e977b9643b2dcc099`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 4.8 MB (4815560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b60e40858b07af317895f3351764c9b61ab25d5602df053b12d72a7b1d3e7fb`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0311a98d0b14ede1e3db9b1932f26b285c4d856ab4977227253ebcf073bb5fa`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12ed6db2b1c4c9825e9af9155777566a7f5fe52a8226886ac94d141a09ee90e`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 240.1 KB (240083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd18.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:e3c9fbb356c6bcb3e38c0e5c14bd8eee04098ef82bea56f8b216175400394b08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28107710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5894ac96771951b519122f466116cf07e04f19d9d43a01b4a6ca0fd6354321c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:06:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:12 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:06:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:06:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de78e4f730cf83f3f03ca96a7f7531a6372d67935eb2637f2f3230b1c83fb6c`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 4.3 MB (4263826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b39acb592654a8c7c01dc37815f993a6304d931d7bfe43ab7d1f7f2fe942b5`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 1.6 KB (1643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4d447e4c8e7333c968cb129edb84c2f689db4d8485500970c619ffc579b3b9`  
		Last Modified: Tue, 02 Aug 2022 04:10:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca0c608f502516035d83cf6fb13c86c462da71d47f8d1373dccb0a18f6183b7`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 107.3 KB (107283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04-non-free`

```console
$ docker pull neurodebian@sha256:c96063b0f74ec7b62c233156fdf6abae87351f17536aa595caff129ff2daf692
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd18.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:84b2749fa94bbe07d80e5a8050387f3c0889827ddaee08985b5c3c4ad8d73a0e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31768082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21cd21c8c00bf8fe943d887ce4b7826bb43fd002a5a0529e93599f2151897f53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:10:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:10:48 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:10:49 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:10:55 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:11:05 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc542f6a209fdc44cb2483f852cc908a5d32f220fe23e6e977b9643b2dcc099`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 4.8 MB (4815560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b60e40858b07af317895f3351764c9b61ab25d5602df053b12d72a7b1d3e7fb`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0311a98d0b14ede1e3db9b1932f26b285c4d856ab4977227253ebcf073bb5fa`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12ed6db2b1c4c9825e9af9155777566a7f5fe52a8226886ac94d141a09ee90e`  
		Last Modified: Tue, 02 Aug 2022 05:14:27 GMT  
		Size: 240.1 KB (240083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0477f72700b46658739abdb42d4119ede52403b342d23bac9082effed8b13`  
		Last Modified: Tue, 02 Aug 2022 05:14:37 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd18.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:538b4a3c4f05679213416c0e34106b3c53489b4ec63a71d0dd67e5046baff586
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28107966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5f8df5591bf442efc2dd206cba7f6d01c217476c97f0f758abd515935566de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:06:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:12 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:06:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:06:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:26 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de78e4f730cf83f3f03ca96a7f7531a6372d67935eb2637f2f3230b1c83fb6c`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 4.3 MB (4263826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b39acb592654a8c7c01dc37815f993a6304d931d7bfe43ab7d1f7f2fe942b5`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 1.6 KB (1643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4d447e4c8e7333c968cb129edb84c2f689db4d8485500970c619ffc579b3b9`  
		Last Modified: Tue, 02 Aug 2022 04:10:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca0c608f502516035d83cf6fb13c86c462da71d47f8d1373dccb0a18f6183b7`  
		Last Modified: Tue, 02 Aug 2022 04:11:01 GMT  
		Size: 107.3 KB (107283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c136ff57d30f443e379cc670f3087bbacddb3a39822586734a72d633d9c009`  
		Last Modified: Tue, 02 Aug 2022 04:11:15 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04`

```console
$ docker pull neurodebian@sha256:014012d14722450c1ecf31613399158a79a2f4fb5499f813ace8af368ead8a4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd20.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:aa21cd8266ee48dba8c14bc51bbe83426cddd8e7b7f306752d7f4a3aa6a490a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a261e9ccff37779edee41b9e36e03bdedee1b6fb7493f9f50dfd861f030147e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:11:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:11:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:11:40 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:11:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18eb2a1e33744cf455dc8e5b43ca272348d2bb06277f449482526acd9dd2e3c7`  
		Last Modified: Tue, 02 Aug 2022 05:14:48 GMT  
		Size: 5.5 MB (5488986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718aa848cdd79073ccfb03cb65426e6111aa4a1f53798d583a2708c905adb45e`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f054786ccdc81eeb880c3863b74c837c0af9adf50199142610bbfe5517bd0e65`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8854b477ce6477f7c67f2e8049fff57e239bbd197771d9b0f02860a53a993f73`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 238.5 KB (238546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd20.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:ea57ba9779c6719381851e9a0473064767de43873042272c4994ba3d3b320bb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32620836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b13a4b9dc8246a71c988392a50f49a49b582f6b175ac7456916e0febdfe183b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:06:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:06:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:06:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebefee5e1b9da86fcbbca29d2c03f5892fe9486f9f8f0eaa8bcf500a5b8156d3`  
		Last Modified: Tue, 02 Aug 2022 04:11:28 GMT  
		Size: 5.3 MB (5321730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6168a75c411fa9792f31df8a0462fd6eaece0c841e490727350664b64bbfaae`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb09a7a9597120a18a94eb0a6f5c3b7163a468b75d1ab5ae6d6a98140aa1222`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dce270fac0448b9538b37ff41ebbabef4503fb776a81d633757dbb19b7ad036`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 105.3 KB (105316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04-non-free`

```console
$ docker pull neurodebian@sha256:50870fcb7cd3675d44c36f2afeef868dbbce409f4044c7dcc445bba538f5c5d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd20.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:97cd25161a5b8497ff6ee41bb32435e07376d482165a3ea9d4f5d1d6c1c364c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4e1e85d7f13b5a1992aef372fbb4c6aef09d36913adf036c0cedd027206335`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:11:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:11:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:11:40 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:11:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:11:48 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18eb2a1e33744cf455dc8e5b43ca272348d2bb06277f449482526acd9dd2e3c7`  
		Last Modified: Tue, 02 Aug 2022 05:14:48 GMT  
		Size: 5.5 MB (5488986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718aa848cdd79073ccfb03cb65426e6111aa4a1f53798d583a2708c905adb45e`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f054786ccdc81eeb880c3863b74c837c0af9adf50199142610bbfe5517bd0e65`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8854b477ce6477f7c67f2e8049fff57e239bbd197771d9b0f02860a53a993f73`  
		Last Modified: Tue, 02 Aug 2022 05:14:47 GMT  
		Size: 238.5 KB (238546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006b63a9e6c106d97accf1f8d76d620462cb5aa6b149073bfe32766d8b53f8d1`  
		Last Modified: Tue, 02 Aug 2022 05:14:57 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd20.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:ebc00ba3160adf4d00847f33e7f816eacd6cdf76f45b97bf741445e94757cb2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32621093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c84b2f66e72fd17572486826218e08d29359280850d1577b61dcb60b7b0b00b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:06:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:06:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:06:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:06:58 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebefee5e1b9da86fcbbca29d2c03f5892fe9486f9f8f0eaa8bcf500a5b8156d3`  
		Last Modified: Tue, 02 Aug 2022 04:11:28 GMT  
		Size: 5.3 MB (5321730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6168a75c411fa9792f31df8a0462fd6eaece0c841e490727350664b64bbfaae`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb09a7a9597120a18a94eb0a6f5c3b7163a468b75d1ab5ae6d6a98140aa1222`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dce270fac0448b9538b37ff41ebbabef4503fb776a81d633757dbb19b7ad036`  
		Last Modified: Tue, 02 Aug 2022 04:11:27 GMT  
		Size: 105.3 KB (105316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0afab03236a5302ef8495cdca5dc8d773b3a75c13cc5e54d8deca5901f9a6`  
		Last Modified: Tue, 02 Aug 2022 04:11:39 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd21.10`

```console
$ docker pull neurodebian@sha256:bb234b796f7d12aa085bfd99ec7b3653453c9ca31f39c7ae8b73d78761c30561
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd21.10` - linux; amd64

```console
$ docker pull neurodebian@sha256:db1963ee159e0dca0159562742ad532d2a086a988b9354057ed8d77647b5e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34384580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e017fc712553f899766998fdb9db30eee355df9033c23dd72ba12b43aa47eb`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:38:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:38:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:38:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4222215fe5bb0924cc9cbcbbb6d524fc181c91b66bd31430a258a78ebce2c519`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 3.8 MB (3752244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983039d4e1a2415f0f809ddd83bcc60a90fe40cf2e2c3a4f93ded36ac4cab37a`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d378c9cd6485d098e5bcf609a3e34edc5c31a424035a4bd61de01eadbab71c6`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e2ecd075adf7f432e69fbe49ea1b42a7c15c0cf6114789b57ffa534f851834`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 250.0 KB (250036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd21.10` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:e1fc2dc1b64614617f8ce4060fb2907481ab2353c8bf21c3050761a267fbd9d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32856492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3c14d270240a3fa26a0147e6dc5bb70a299f8c8e8a0b9caf2a3d0c5f8d2551`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:24 GMT
ADD file:d1932d13ea73e26ad39647db09c23895cf0644ba34851cb87e777778d59b6730 in / 
# Tue, 07 Jun 2022 01:25:24 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:09:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:09:26 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:09:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:10:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:166e0294b8df947d819744f38e21281ed5f29a2a3b19d191deee511cbfb0e473`  
		Last Modified: Tue, 07 Jun 2022 01:27:26 GMT  
		Size: 29.0 MB (29018061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fd390207922789eacc8378770b82705bf3ef6a8ee15ff29c896c4c7b3a8737`  
		Last Modified: Tue, 19 Jul 2022 20:15:09 GMT  
		Size: 3.7 MB (3726896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41123559e445d7fd43518edd8d4445a77c75c6fed0745b660394be39800e2e06`  
		Last Modified: Tue, 19 Jul 2022 20:15:07 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3949fbe2cfc1efed7983069b8e05e484d5bbe3334f54d1142a5bbb1dff8d3f`  
		Last Modified: Tue, 19 Jul 2022 20:15:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7168a0a709927f8d07cdd160accd5040d26e868fb92cc598d965c3654d28c3f`  
		Last Modified: Tue, 19 Jul 2022 20:15:08 GMT  
		Size: 109.5 KB (109547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd21.10-non-free`

```console
$ docker pull neurodebian@sha256:d8dd2cc8165345590b62af26fc7a2e0df2f5060d4450b4610e7b6b23517f1535
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd21.10-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:fa54f734923cf3bc814f9ca42375869480681699d414e88acb6e22b84dc40570
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34384840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a47ecb4e0e0a6f4fa722091c451eb400637d32dcf1bb57d808dcb0e1b55c994`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:38:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:38:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:38:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:53:52 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4222215fe5bb0924cc9cbcbbb6d524fc181c91b66bd31430a258a78ebce2c519`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 3.8 MB (3752244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983039d4e1a2415f0f809ddd83bcc60a90fe40cf2e2c3a4f93ded36ac4cab37a`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d378c9cd6485d098e5bcf609a3e34edc5c31a424035a4bd61de01eadbab71c6`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e2ecd075adf7f432e69fbe49ea1b42a7c15c0cf6114789b57ffa534f851834`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 250.0 KB (250036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cf61727686c8d90437ef15476fa41e9fb4a62ac20103873c80d2c3a11c3f3b`  
		Last Modified: Tue, 19 Jul 2022 19:57:02 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd21.10-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:d4317d75f7993f1c0989813fb01ddb8c37b2c45f469d348b3f06cf10fb4fc29e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32856749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2014687e1f50bb858f914f8177891ca3949ae87fc8fbbd65b7b1a140b43d7e70`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:24 GMT
ADD file:d1932d13ea73e26ad39647db09c23895cf0644ba34851cb87e777778d59b6730 in / 
# Tue, 07 Jun 2022 01:25:24 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:09:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:09:26 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:09:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:10:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:10:16 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:166e0294b8df947d819744f38e21281ed5f29a2a3b19d191deee511cbfb0e473`  
		Last Modified: Tue, 07 Jun 2022 01:27:26 GMT  
		Size: 29.0 MB (29018061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fd390207922789eacc8378770b82705bf3ef6a8ee15ff29c896c4c7b3a8737`  
		Last Modified: Tue, 19 Jul 2022 20:15:09 GMT  
		Size: 3.7 MB (3726896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41123559e445d7fd43518edd8d4445a77c75c6fed0745b660394be39800e2e06`  
		Last Modified: Tue, 19 Jul 2022 20:15:07 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3949fbe2cfc1efed7983069b8e05e484d5bbe3334f54d1142a5bbb1dff8d3f`  
		Last Modified: Tue, 19 Jul 2022 20:15:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7168a0a709927f8d07cdd160accd5040d26e868fb92cc598d965c3654d28c3f`  
		Last Modified: Tue, 19 Jul 2022 20:15:08 GMT  
		Size: 109.5 KB (109547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2bd7e7df381379f1dde19c12b40e93e765871170afe519be5f19b996972af`  
		Last Modified: Tue, 19 Jul 2022 20:15:19 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd22.04`

```console
$ docker pull neurodebian@sha256:baf5f59d711b96b68a32075b8acbeb2ccab8964532f1d6537dfaab6a8899735d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd22.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:0480f6ae6d663b07a1099780dffd6e89cbabe10c12d526384d7da32d9a3acb9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34450999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fbc15d724c59441a6cd3beebd6bc516023144076e4f2a61123c1eeb5af96d4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:12:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:12:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:12:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:12:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09202f1c776958afd50a2a64423fea360c253b75477dcbc34d89bf93966c518a`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 3.8 MB (3765806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf0688d1300705116dbdedfac9df50b6133cedc3be665079dd77c7fcaf9e30d`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b9676b9f1dd5a78ad2195a513b7ff19c199b163eb36941a029e7e754a42b87`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce8c95cde21ecb9062feba61921aa4ba04124489e73edf7e98f51b8ecbc1c54`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 257.0 KB (257045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd22.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:71239ac11306e9df0dbc7f92f518661747844c5608c9d3f2cd20013b1ec5ce3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32092016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23503e08ad9a81606e7046f475b9563b32b59225ee4d6f26a039393879847e11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:07:21 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:23 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:07:24 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:07:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d10adfa05511ba6785d83dd0cbc9965a3bfa7c2e5f66b36bd9582dd28efae2`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 3.6 MB (3594085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6664f868aa1787343b46632fc0210a72d96f7f15e81c9bd46911630d2bfe64`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb6881b552e541f1b15a6156fd149417746a8d62945e4c1f4e7541577d4ba58`  
		Last Modified: Tue, 02 Aug 2022 04:11:53 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8b558fcf3bbee7daa5e75d734cddf9f5b7de2ef3952381ce23ec576ffdbf5f`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 114.8 KB (114788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd22.04-non-free`

```console
$ docker pull neurodebian@sha256:1197e00ad522be0d59bfddceb65477790419e5d78f28ef45d891f5f4ba34326e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd22.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:1e9be3aca705fffeec64d28b6887fa5e0dbd257ae13855191ca0daddb31a98b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34451255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bd4d70243f871994419f7aa9747bbcaa5d4fdd8961d5023641181d6119f3a4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:12:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:12:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 05:12:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 05:12:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:12:28 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09202f1c776958afd50a2a64423fea360c253b75477dcbc34d89bf93966c518a`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 3.8 MB (3765806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf0688d1300705116dbdedfac9df50b6133cedc3be665079dd77c7fcaf9e30d`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b9676b9f1dd5a78ad2195a513b7ff19c199b163eb36941a029e7e754a42b87`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce8c95cde21ecb9062feba61921aa4ba04124489e73edf7e98f51b8ecbc1c54`  
		Last Modified: Tue, 02 Aug 2022 05:15:09 GMT  
		Size: 257.0 KB (257045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0892b7c65de090a7c4cc54770df7517af33e780fffae00e6d582aa47a3732131`  
		Last Modified: Tue, 02 Aug 2022 05:15:19 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd22.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:ee35cfb6932ff887193402b97dad1e76561d53ca7e38327ec00ca1ad1c2e9b3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32092275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41c6c08826d3bb3d12a952ab5fed7db31727ef5be49e8cd9a9dcf2c9c9d896a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:07:21 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:23 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:07:24 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:07:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:07:38 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d10adfa05511ba6785d83dd0cbc9965a3bfa7c2e5f66b36bd9582dd28efae2`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 3.6 MB (3594085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6664f868aa1787343b46632fc0210a72d96f7f15e81c9bd46911630d2bfe64`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb6881b552e541f1b15a6156fd149417746a8d62945e4c1f4e7541577d4ba58`  
		Last Modified: Tue, 02 Aug 2022 04:11:53 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8b558fcf3bbee7daa5e75d734cddf9f5b7de2ef3952381ce23ec576ffdbf5f`  
		Last Modified: Tue, 02 Aug 2022 04:11:54 GMT  
		Size: 114.8 KB (114788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507e338e8285a94cc9f44eaccf411f4ec3a6ca2e09e4814bf97f8119e2dda481`  
		Last Modified: Tue, 02 Aug 2022 04:12:05 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:non-free`

```console
$ docker pull neurodebian@sha256:8f46a81df71a6fd6eb3e8743319ce935638ff7d4f4ba25f48c5c796651410246
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:f865df23569ce8d81cc0f8ccd3e8b33d6ccc250ae34a26352f9161e0a074215a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66632140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b60780d8b2d8dd6b19f7afa2f9602864ccf2d9aa4ceb546623604bbbfb470b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:55:34 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:35 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:55:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:55:39 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:55:43 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da4c47f93a29385c466f0b8d06c34810d3c2fcf6a9fd424a039d0a9dd5ba91a`  
		Last Modified: Tue, 23 Aug 2022 03:57:33 GMT  
		Size: 11.3 MB (11310656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baadeaeeef9ec92fffddaf3f7991f97f2852ce3310c7e7115279778ce1b60c23`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6357f4e4c8211177f51c1526a9d04ce62e0dd0ed3eeb6745feda9f395463d`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb160502891152d59ef71771495e79282a1d437e3a848021655e73ad1c5e6e48`  
		Last Modified: Tue, 23 Aug 2022 03:57:32 GMT  
		Size: 311.6 KB (311560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d754d80adef35e288ba8c81b0c1d43a68a7a9e9ea44bc4c28954e7006e4c2ec9`  
		Last Modified: Tue, 23 Aug 2022 03:57:44 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:4a4b0248eac44e958218d5cc595b06a281d5ec394de57a48e127631d166842f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64895258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fd53427e1b819b7fefedba74bd470e4361c2d66d6458836639fd8820cfb41d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:08:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:08:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:08:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:08:26 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff40e6a469794f9119b4074673af50f6e14202e8140c999b2934d90e5d334532`  
		Last Modified: Tue, 02 Aug 2022 04:12:56 GMT  
		Size: 11.1 MB (11104729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2a776b73fedde99a37ad1a5b4225e4cbc0b571fca2183b5ed2f22eb8808108`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28656afe730c0967736477f5ec1ed6f2366700ed354642dc492275fe287e71cb`  
		Last Modified: Tue, 02 Aug 2022 04:12:54 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee0dbec7c4163720ac1f0d28a757f4e31c98305ec91f34c9e15dc034a6ad6b`  
		Last Modified: Tue, 02 Aug 2022 04:12:55 GMT  
		Size: 105.2 KB (105171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c0342191d269718b61134e36c597d1f0c21655afbd52d6ad48fdf07054b7e`  
		Last Modified: Tue, 02 Aug 2022 04:13:10 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:e98da7e376fde4c546e16b52735e663eb876819b1795a560666f1ee80330b929
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67609277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2aa7047da75911beb318e8f6a833147b12b661ba5dae09517fd3a378231cd6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:05 GMT
ADD file:ade7fe80dd06354b3eab9283f6c354047be2b94806dbe1dedee8d5a0f658f7be in / 
# Tue, 02 Aug 2022 00:39:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:19:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:19:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:19:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:19:32 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:84601b97875630e4b14ebdb276bc4c68f89eafe6d12dec64b54dbcaed7c0c802`  
		Last Modified: Tue, 02 Aug 2022 00:44:40 GMT  
		Size: 56.0 MB (56002231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27896781078532c6ddb430224d3c48f834d093e2ab3ae5ff4805af3597860da1`  
		Last Modified: Tue, 02 Aug 2022 16:21:46 GMT  
		Size: 11.5 MB (11499635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f1ce447767d12a4c29740ef298c72902b324eecc4f8f0f0c763e38c98bab6d`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a522090ef6aa533a52810a47e789f07e4c7ff1a06cd9c5191eb0feebd0fb5a`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b003d4600f8668923f8466f8795c15318ecc94ee07d7631411f57e6a5cb9e8b`  
		Last Modified: Tue, 02 Aug 2022 16:21:45 GMT  
		Size: 105.1 KB (105064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b434f1dc0af5922193126a834695fe056c58896604f9207fe6f1224461fb59c`  
		Last Modified: Tue, 02 Aug 2022 16:22:01 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:d2a2ae1159e5e98fab23316b1c87251ab3148fa02bd8dc35e0b4fec3425b510c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:7273039834b88053ebeca3c10c991a96e3c9527884c5b2327829dccf9327a076
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64714411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a8a2facbac503153a56869752b3dc14c8ef1ea00d9f784e8e6720fdd67336b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:56:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:56:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:56:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:56:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154f30b7649dd9ff36175e6592055cf8360c6e985876034a2272424287be1cd7`  
		Last Modified: Tue, 23 Aug 2022 03:58:18 GMT  
		Size: 11.7 MB (11650922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c00af28db2666c58eba10693268b55f170ca7e71d33f6cfe0d665fca65b1b7`  
		Last Modified: Tue, 23 Aug 2022 03:58:16 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f335f65a3d201956ff81ba9ecd2c1f5355df35fc67a4b449123d4d0d3dbf09`  
		Last Modified: Tue, 23 Aug 2022 03:58:17 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4abb7659ae1e8863abcaf9faf27843788a20b3d8a6ab97236c67a4ab6ae8e3`  
		Last Modified: Tue, 23 Aug 2022 03:58:17 GMT  
		Size: 292.7 KB (292697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:298d06f9fede57c37c75a2a15c45e367cfc4bf149b6b161348973624740271ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64856469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3ba2c11ffb710e401d30c92bd6e56a7d6169bb48780f8039be0ce102939a6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:38 GMT
ADD file:477966410dd9e274b01740d7af857db5c024b4c4e53a5e83b5da6854d5b0c209 in / 
# Tue, 02 Aug 2022 00:41:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:09:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:09:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:09:09 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:09:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17bcb8e39c7f35480d4c2e5b46b6c0a58dac180206453cc49052707aa8053632`  
		Last Modified: Tue, 02 Aug 2022 00:48:00 GMT  
		Size: 53.3 MB (53311787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b23f22c8c00046bbf67cd59cd4f2af07dce5c5fa7a24ab5543ae0bb3564f4aa`  
		Last Modified: Tue, 02 Aug 2022 04:13:49 GMT  
		Size: 11.4 MB (11445839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155e679260259d507584bee8d944d898d1181db2db8ee4e81b619ee20fe55dd0`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe48f40923db8199277d01e875d32310e9fc5ebbf9e02ea16c1397f9c07f2479`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707dc6bc4aa4606f4136b46e3735effc8020caaff4770ef7e70e7cfdc6946bd2`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 96.9 KB (96860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; 386

```console
$ docker pull neurodebian@sha256:376dad16c227357a26b95fa5af0a5b8386173d1e79fd72c29b8796d920a58823
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66173823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91aabef4df60debd2a22d26ff5f4e921904afa674132f60afb2577aa2996cdf9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:23 GMT
ADD file:40a2042e14b22d803da216af628cd6e8603c923c4fe79ca3c4c79c95c1c1e878 in / 
# Tue, 02 Aug 2022 00:40:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:20:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:20:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:20:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:20:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ef86b631f45587b4b6d1c16b80732997a4895ae8df072b14d68c25aeff8b901e`  
		Last Modified: Tue, 02 Aug 2022 00:47:20 GMT  
		Size: 54.2 MB (54195066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad56ce46d52bfd83905b2ba1001b937d0d384c2e9f52223b216e0205c495152`  
		Last Modified: Tue, 02 Aug 2022 16:22:42 GMT  
		Size: 11.9 MB (11879907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1643e5b63805dccebfbcaa3e8093baf3557f5e2d535c490c03e1dc32589240a`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e09ccea7ebbf3f00dff13f17b94a50a8828ca7a220bc06fca82b09fd996b414`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54f18cb63a52981a30664a1778e0a688a3aa900a519ae5ca7ec36351fd2ef6`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 96.9 KB (96869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:564e706b881a6f8c317ed565e2cba68aa39a2c67520e0e57a3d1fa33f8f1c3b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:fc0676b486d9fb81a658bfb0437aad832de7cc1bd4fdb3921f046ba0a0b19e06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64714808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d38f7230946bb568bd5d6c13c5575905fb3170262c5dbe4cf23af7a0e2e6c9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:56:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:56:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 Aug 2022 03:56:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 Aug 2022 03:56:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:56:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154f30b7649dd9ff36175e6592055cf8360c6e985876034a2272424287be1cd7`  
		Last Modified: Tue, 23 Aug 2022 03:58:18 GMT  
		Size: 11.7 MB (11650922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c00af28db2666c58eba10693268b55f170ca7e71d33f6cfe0d665fca65b1b7`  
		Last Modified: Tue, 23 Aug 2022 03:58:16 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f335f65a3d201956ff81ba9ecd2c1f5355df35fc67a4b449123d4d0d3dbf09`  
		Last Modified: Tue, 23 Aug 2022 03:58:17 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4abb7659ae1e8863abcaf9faf27843788a20b3d8a6ab97236c67a4ab6ae8e3`  
		Last Modified: Tue, 23 Aug 2022 03:58:17 GMT  
		Size: 292.7 KB (292697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e31bea2350446c52f2efeef74112da2d2a9bb4c743a40f71aeb2974c793b3e9`  
		Last Modified: Tue, 23 Aug 2022 03:58:27 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:d6da1355fb08035ff6642e9a44a2c50f2a930512694c14d72d7730689036a5f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64856868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2239bfedc0b0b09064acc7d3944ea0e2c0af6eb2f5de108b4d1b2c6015b9469`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:38 GMT
ADD file:477966410dd9e274b01740d7af857db5c024b4c4e53a5e83b5da6854d5b0c209 in / 
# Tue, 02 Aug 2022 00:41:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:09:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:09:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 04:09:09 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 04:09:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:09:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:17bcb8e39c7f35480d4c2e5b46b6c0a58dac180206453cc49052707aa8053632`  
		Last Modified: Tue, 02 Aug 2022 00:48:00 GMT  
		Size: 53.3 MB (53311787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b23f22c8c00046bbf67cd59cd4f2af07dce5c5fa7a24ab5543ae0bb3564f4aa`  
		Last Modified: Tue, 02 Aug 2022 04:13:49 GMT  
		Size: 11.4 MB (11445839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155e679260259d507584bee8d944d898d1181db2db8ee4e81b619ee20fe55dd0`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe48f40923db8199277d01e875d32310e9fc5ebbf9e02ea16c1397f9c07f2479`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707dc6bc4aa4606f4136b46e3735effc8020caaff4770ef7e70e7cfdc6946bd2`  
		Last Modified: Tue, 02 Aug 2022 04:13:48 GMT  
		Size: 96.9 KB (96860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939008275e6fc63ae497488f2dd00411fc6aebe348e916c5aa4cf8740460deee`  
		Last Modified: Tue, 02 Aug 2022 04:14:00 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:2664ba2001554b4c81910197606dbd5210149e9217d543f6b543217451c8f202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66174221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7288077efa30d1f51895d8e4c18f4f3f0de8fb4bfbc5acb06bfff49e038cc3d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:23 GMT
ADD file:40a2042e14b22d803da216af628cd6e8603c923c4fe79ca3c4c79c95c1c1e878 in / 
# Tue, 02 Aug 2022 00:40:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:20:19 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:20:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 02 Aug 2022 16:20:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 02 Aug 2022 16:20:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:20:31 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ef86b631f45587b4b6d1c16b80732997a4895ae8df072b14d68c25aeff8b901e`  
		Last Modified: Tue, 02 Aug 2022 00:47:20 GMT  
		Size: 54.2 MB (54195066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad56ce46d52bfd83905b2ba1001b937d0d384c2e9f52223b216e0205c495152`  
		Last Modified: Tue, 02 Aug 2022 16:22:42 GMT  
		Size: 11.9 MB (11879907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1643e5b63805dccebfbcaa3e8093baf3557f5e2d535c490c03e1dc32589240a`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e09ccea7ebbf3f00dff13f17b94a50a8828ca7a220bc06fca82b09fd996b414`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54f18cb63a52981a30664a1778e0a688a3aa900a519ae5ca7ec36351fd2ef6`  
		Last Modified: Tue, 02 Aug 2022 16:22:41 GMT  
		Size: 96.9 KB (96869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b198f0f40db6b4de8cb7252ebc6718942cb14b2fbd559aebb205f5dc5301217`  
		Last Modified: Tue, 02 Aug 2022 16:22:53 GMT  
		Size: 398.0 B  
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
