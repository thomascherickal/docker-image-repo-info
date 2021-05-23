<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1.6.1`](#spiped161)
-	[`spiped:1.6.1-alpine`](#spiped161-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:e7b696fd86c235eb96fb948d3ca260c9e80e416b43bb9be3a0597947f56ea431
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

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:bcaed8de930b8832a40873acf6861bf984e70edf571e971f372f24da4f008b1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36313953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8da550658c999941253a73bc835fb7a71f6af0881ad9610d662638086f2c833a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:27:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 17:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:27:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 17:28:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 17:28:06 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 17:28:06 GMT
WORKDIR /spiped
# Wed, 12 May 2021 17:28:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 17:28:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 17:28:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80866732d602112cb309734d5fdb453f07a1e00ff5eebb449821148acbe03ee9`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5c28b22404235df98f9f542c8393d1694d19406863a5f7b1b8bfb2079a9477`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 2.1 MB (2128505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2da39cf8d05feb934e294e041fa92e75f5f1071abf10b086c21bfeca751164`  
		Last Modified: Wed, 12 May 2021 17:28:28 GMT  
		Size: 7.0 MB (7037329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaaa5bc95b1a83402d28c94b0e297cbc4dbdcd89c127a71d41700fc5d67ff64`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb6ca2836a313b7d46ad352635e75d68ad5297f638713a4bad872abba008f8a`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3f9e7be1ab568265c3dd6fa509c7c114c1879a02c3bded42f54fd11289735e1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32201133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:563fe344ab3950b18fe739f7280a4ceee978289d27c277c471a187c606fcb931`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:10:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 02:11:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:11:14 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 02:12:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 02:12:13 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 02:12:14 GMT
WORKDIR /spiped
# Wed, 12 May 2021 02:12:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 02:12:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:12:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93994a565732f80afb936f17eea4a465d85e20d35c345d8a882fdeae92f0d59c`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d836928393044684b89355c1804a6258f852af61457a0915ae433c3406eed`  
		Last Modified: Wed, 12 May 2021 02:12:44 GMT  
		Size: 1.8 MB (1839342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d98e02b46e64902855f44d27903de22548a6800fbcba76c18a2aa89fa538ec`  
		Last Modified: Wed, 12 May 2021 02:12:45 GMT  
		Size: 5.5 MB (5479993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4cf9810da7adb24dae3073d41ef246afb43ba96eb5565f9f0508b31872735f`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd46064d587a7a824767f89a11f12af984145bc88a9d042bc0b83a34ad8dcbdf`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:182834a86cf1b16639e086952aa1628bfe56c89d0539d1e239fc09c7ae3481aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6e06b72812b074a05d2ed74589ec9a23a1529a74f73c3aa00941c8ce50cc14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 20:08:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 20:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 20:09:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 20:10:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 20:10:22 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 20:10:24 GMT
WORKDIR /spiped
# Wed, 12 May 2021 20:10:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 20:10:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 20:10:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b39d1ef66a2842eb5175ad816ce0160e49aea4e5cd37db71923a26983f63800`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b1cea5297efcedcf7f3656dd7ad9811a22abf743c8799650421f5c5b2ca521`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 1.8 MB (1759508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b338f8510b528b02e5e16346ae09c6f9a04a1782956218d76b3b9d3eb7747`  
		Last Modified: Wed, 12 May 2021 20:10:57 GMT  
		Size: 5.3 MB (5285697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5268698aa228237d459083f95292fb3950668af1bc423300458662d6817006a`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71724157a7a130d88d6f3b3a62bcea37b4d6ef8e4c22799062a9949e1ae2294e`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:425d6efb65a0998268928f8d111c668cdb5bcc03a7a192b8ccf8d78e243d6ead
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33826685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff8a61fb95849a75c077007d48124a0e3aac5e00aa38c6850739bd6bcbbdb6cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 19:37:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 19:37:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 19:37:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 19:38:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 19:38:46 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 19:38:47 GMT
WORKDIR /spiped
# Wed, 12 May 2021 19:38:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 19:38:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 19:38:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55234c1dc3b0ed681bb0d6a515ee5325aa51350f28c96d9a835a08212f3ae83`  
		Last Modified: Wed, 12 May 2021 19:39:14 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4168bd2eacc4c8ba8aece3c064ea6727359406a6703c4736efc637e5d4c4b6bd`  
		Last Modified: Wed, 12 May 2021 19:39:14 GMT  
		Size: 2.0 MB (2007869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2f082f7dff3900e083123b15beb36bd2ec579a47204d92a40ffb22fa1b419d`  
		Last Modified: Wed, 12 May 2021 19:39:19 GMT  
		Size: 5.9 MB (5905354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d99e2ad24406eebd6451cc38a11a0395e83e86e58f59996b83364ec0e18e8`  
		Last Modified: Wed, 12 May 2021 19:39:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbf9d011ac895e52be82c5b195bc46de056831c6dd9f466584c655343f44a1b`  
		Last Modified: Wed, 12 May 2021 19:39:13 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:5e319479936eee4e789629c4b79d1720b52145a0ad529631647e842929a59996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41563204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76bac7e630d8ae86f4f836f8b090a8b003a681f6fd732d20f57d8662f9a02b3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:13:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 06:13:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:13:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 06:14:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 06:14:36 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 06:14:37 GMT
WORKDIR /spiped
# Wed, 12 May 2021 06:14:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 06:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:14:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a0f277245dd1b05ccbb1a6029229f7be99e59698537883010bc0a870700d5f`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daaa7f59c14ccc73a3a4cb78bb6c51185771bf7111f3985ba136a1f9fbdc683f`  
		Last Modified: Wed, 12 May 2021 06:15:19 GMT  
		Size: 2.1 MB (2132666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d5ae3e2d54344fa0d2eb0524dd0cfbd766ecef2ba8f16f933fbf8da5effb68`  
		Last Modified: Wed, 12 May 2021 06:15:21 GMT  
		Size: 11.6 MB (11633257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac63635bbb761f615b705a65a48368ae2f6530cbfaca13e0181713ca9eb752f`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ab0dac9585b965c6c6e54fb3b6d2784bc55b3749398040d858c1c282dc8d16`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:73b842b8648de250441f111a069985f2658d1cdb8e1bd091142cd013915805a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33943918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2703c88777e1bfbb7b151bdc9dff69d41d67e7ea4768c37d1a548605f4610a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:48:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 14:48:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:48:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 14:49:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 14:49:40 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 14:49:40 GMT
WORKDIR /spiped
# Wed, 12 May 2021 14:49:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 14:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 14:49:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d5ab1a7dfe229c365eac985c9888e5f9bd91a6f8b4827091c3beee0c3f4a8`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0b5f59d5c13ed0c6d4c539ff5e99f2458f180cb92cb90b933b7c1e5c69b643`  
		Last Modified: Wed, 12 May 2021 14:49:53 GMT  
		Size: 1.7 MB (1712452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b55c4319acfe89be8d0d190fa408f54c45acc0465a688cd810b672c862c004`  
		Last Modified: Wed, 12 May 2021 14:49:58 GMT  
		Size: 6.4 MB (6416412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df4593d00b37d8751d7acfcf1b4af789ea345b2d2ea1e43d91c0fe7fb2172a`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1527a275f222e2422b8469037f83cd67d8b47483dc6918befa20cf7ddada0816`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:cf18d0e1655d3071d9806a421f1978146647484cb65f745f60c9bb7155406fdf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39523409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787b7006873b0ca19028e9c0be65eefbc1f23f6bfcc47b8aa79d409644f5f14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:40:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 17:41:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:41:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 17:45:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 17:45:39 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 17:45:48 GMT
WORKDIR /spiped
# Wed, 12 May 2021 17:45:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 17:46:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 17:46:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e30106e0e567258ac9bdbf04a32f01e2871897e38e976f7b42537aa7f28c11a`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9021ed50e6c78d34322b096accc9e0778308ce19e73029ede0aa9b092b5f1`  
		Last Modified: Wed, 12 May 2021 17:46:40 GMT  
		Size: 2.2 MB (2225153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89585b290c82da4f3557bb03c9087ff570f0c41c2ba06240c70764097e8f59c`  
		Last Modified: Wed, 12 May 2021 17:46:41 GMT  
		Size: 6.7 MB (6743645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b15eb96c19d3049851885d6982137106dcf9e88720cecdbb0bc2bf9ce242480`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e4d8c0ffcd6ca31bc463f47c6e1cf1cd37f90c812f3471d57fbbb1cf98a99d`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:a45845a753efd776e495cdb7b19748e4d154bcae83ed61b0641dc7cb146e3df2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33527924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f554f74e1771a0e9e02db5ae99425227fa0c23048966969766356b2c739a28fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:52:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 07:52:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:52:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 07:53:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 07:53:32 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 07:53:33 GMT
WORKDIR /spiped
# Wed, 12 May 2021 07:53:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 07:53:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:53:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9965773f77d64c76e62f6586a8cc5ce4f21370e94b4ee2028598f65afc8fc8`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15772499dfa1ca6b51b5b6e1b62806ec4acd57f17f3458b41d33081dc9e5d3e7`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 1.8 MB (1821984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194ab3d8921fd77cf4980b3c52e6fa22d84e0f594ce5ed27c0d31323e12c1410`  
		Last Modified: Wed, 12 May 2021 07:54:01 GMT  
		Size: 5.9 MB (5943554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611dbc6789f5a10002010baf68d43e363fb7ce6c5b13b6f0517bfd6bfbdeec47`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db4fbf3d77db5a2cdb97512d17d9f46b3b5e82bcbd7a3eaac273a979f07ebc0`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:cb1ebb91215d457fba717379a9b2a39415b33fc337468ca1e81a1d9920ee431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:c21bef0140d90218ac109935fb4800c498f43c180f4ef1b10bde2642880be2a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbdf08613600d4c931da69207d9120e5ed8613c25036007e69cb1601a3e8f772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:43:02 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 03:43:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 03:43:05 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 03:43:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 03:43:32 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 03:43:33 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 03:43:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:43:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 03:43:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbdc5fa8a3b40bca444e39933121d87e99aab35af8b484d33aff845dc9223dc`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa32c269d5d00d85d7899e4eacf26aaba16e1172161bbf98004432c88ed2a5d8`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 7.0 KB (7043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60da1f1e01411c7d0f98a00b95e704a5e48286ab9625f96f051b85dd593d8e0`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 212.3 KB (212302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f836cc7647fd0c009041eafa0c5d574e4b5b58b6dc0918744c3c00cedeef407`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6dbf788a05da46939128eed6640869c6cd0ac3b637549bc7a664148c1d27cf`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:750e4a3e2b269c49615e43d6e3699988889b406b0c536a97f01713538717f8a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a6f4c383515708ecc75ec2c2164878f9c74553e6927b9614c53355f96bd64ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:12:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 06:12:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 06:12:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 06:13:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 06:13:02 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 06:13:03 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 06:13:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 06:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 06:13:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05304d4235002a8177d88a9a370a4001b168e9562193801a5939dcb96d98b928`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11429747878607e1935e81d7c9bf1da46083ab17322cfb24cdd9756402bf9eb`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6b2ca69864f244fd48c69f52a2aacb2cd2c1252a8c344bfda821704c3bb45c`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 202.3 KB (202275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd931a38883a95739ed26193356b8fa3a119d0971dc2de02eea8268fcb8d53d`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fd7e5e7757c92528d5a3fba0796309aca6a4e0e8a8ef9a0c9a8326f210bfa1`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:efce446ba8870e78476a9d75dcb1e52c175534d2b7ade2a215d811f2394fc147
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f48264b8ddafa8e951f93dc62b494ff4c0702ad2ed5d97967abeb08eca761330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:35:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 06:35:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 06:35:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 06:36:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 06:36:13 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 06:36:15 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 06:36:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 06:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 06:36:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498ba0cc83ce00b13dfa2f2b0f032008609655b0256c5050ef42ac51b4ac118a`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afde2e53b89bdc9bd82427372b10450afed8a06f7c059c1026a36d942d3ce4e9`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b9dc4c988b74b93e18af14d3edbf234cbb4c959d0ec118f1f35c4b93ec8d19`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a6650f750be3485d508aa8a969ee6542ea8f7c77318469b7276e9376e5037`  
		Last Modified: Thu, 15 Apr 2021 06:36:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514661aafe8081d75ec940a2e1e4fcbfecc2361f2a487ee7cadab8e66f187275`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:60db9b182fdba945554959c75b1bd2444da970be31220e2d374615effdef25ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e0fcfe18621392baf2b43c0bdebc4a5d06f004fe9bc9fffe47df640345b6c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:59:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:59:55 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:59:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 08:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 08:00:26 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 08:00:27 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 08:00:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 08:00:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:00:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71d2a4e9c8536bf553bccdfc5bd248d9d19fbed4f75e83dbe15d3d6ecfe5efd`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284753921e8453f385a71c0fe6cb527f691a28c3b968fbbd1352c7858a6f2915`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4dd4b0d19a431b27428bb2593842bdbcc8d064f50481e75d2c89ed75e42744`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 204.4 KB (204446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572e402105d138be04ffa652557707b95411f7e6845bcfd0f7fd6bf2c9588f80`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98458310d7c2648c532d1d5c331ea217dc4d80ad2467eb566702faf3d897d13`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d1f976abe7dc36865966c36ace3442df28cc760cfbc4325a00a692997a8bf0f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc0614ad90a95b7cd1f85bb13128b580a0c2f29ed00db4f65e968730c4f04440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:28:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:28:08 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:28:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:28:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:28:26 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:28:26 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:28:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:28:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:28:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a4072559715dd3774427ca5bfad06c46001c1d90638f2010ecca1cecb9435`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6417969d29e4f1c0fa56959b290e90527faca258d4dc8f876d5781b5a1d2ee7a`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08261970831fa426d9408c0c3cf638ab7d1ff006feef591eb4b6481ec2714464`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 223.3 KB (223281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dc16c21bb57966882a6696907c801efc77eccc10a5ad026e9bbb1e5316a800`  
		Last Modified: Thu, 15 Apr 2021 07:28:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff154aa157546b5d51db233328ebbed740e8854de199b27d502820e45e65bbad`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9d383336851f89b74885b174acf82891ef2bf8c945a6373dec31ca6676fd1107
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fd56c4b0659f3c04e8bff71019d31b85529f0f9a53b88c69fb81d0bfe3351c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:03:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:03:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:03:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:04:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:04:28 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:04:35 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:04:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:04:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:04:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602add23d4a6d2eadfe98b28abe912c5fcac90dbe9c2a51a54f428ad33d692ee`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451504af2e04d8b41445eedc1f1f9c76a59c85eb2be170be0d8aa078d0aa93e9`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 7.1 KB (7065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd1d09b1e4f40662048b2b792797406a48e2cb33e7e0c06a3b60ff7f189ee3e`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 221.0 KB (220986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38387eb6968cbda04a7e8b097378ba4eba871862d73839fa97fc66d70f606c32`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b42ba1d6389eba3e53edf2210a840a60b804cc8e51a81a4f42bcc86848d85a`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:e7b696fd86c235eb96fb948d3ca260c9e80e416b43bb9be3a0597947f56ea431
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

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:bcaed8de930b8832a40873acf6861bf984e70edf571e971f372f24da4f008b1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36313953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8da550658c999941253a73bc835fb7a71f6af0881ad9610d662638086f2c833a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:27:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 17:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:27:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 17:28:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 17:28:06 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 17:28:06 GMT
WORKDIR /spiped
# Wed, 12 May 2021 17:28:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 17:28:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 17:28:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80866732d602112cb309734d5fdb453f07a1e00ff5eebb449821148acbe03ee9`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5c28b22404235df98f9f542c8393d1694d19406863a5f7b1b8bfb2079a9477`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 2.1 MB (2128505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2da39cf8d05feb934e294e041fa92e75f5f1071abf10b086c21bfeca751164`  
		Last Modified: Wed, 12 May 2021 17:28:28 GMT  
		Size: 7.0 MB (7037329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaaa5bc95b1a83402d28c94b0e297cbc4dbdcd89c127a71d41700fc5d67ff64`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb6ca2836a313b7d46ad352635e75d68ad5297f638713a4bad872abba008f8a`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3f9e7be1ab568265c3dd6fa509c7c114c1879a02c3bded42f54fd11289735e1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32201133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:563fe344ab3950b18fe739f7280a4ceee978289d27c277c471a187c606fcb931`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:10:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 02:11:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:11:14 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 02:12:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 02:12:13 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 02:12:14 GMT
WORKDIR /spiped
# Wed, 12 May 2021 02:12:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 02:12:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:12:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93994a565732f80afb936f17eea4a465d85e20d35c345d8a882fdeae92f0d59c`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d836928393044684b89355c1804a6258f852af61457a0915ae433c3406eed`  
		Last Modified: Wed, 12 May 2021 02:12:44 GMT  
		Size: 1.8 MB (1839342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d98e02b46e64902855f44d27903de22548a6800fbcba76c18a2aa89fa538ec`  
		Last Modified: Wed, 12 May 2021 02:12:45 GMT  
		Size: 5.5 MB (5479993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4cf9810da7adb24dae3073d41ef246afb43ba96eb5565f9f0508b31872735f`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd46064d587a7a824767f89a11f12af984145bc88a9d042bc0b83a34ad8dcbdf`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:182834a86cf1b16639e086952aa1628bfe56c89d0539d1e239fc09c7ae3481aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6e06b72812b074a05d2ed74589ec9a23a1529a74f73c3aa00941c8ce50cc14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 20:08:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 20:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 20:09:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 20:10:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 20:10:22 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 20:10:24 GMT
WORKDIR /spiped
# Wed, 12 May 2021 20:10:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 20:10:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 20:10:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b39d1ef66a2842eb5175ad816ce0160e49aea4e5cd37db71923a26983f63800`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b1cea5297efcedcf7f3656dd7ad9811a22abf743c8799650421f5c5b2ca521`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 1.8 MB (1759508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b338f8510b528b02e5e16346ae09c6f9a04a1782956218d76b3b9d3eb7747`  
		Last Modified: Wed, 12 May 2021 20:10:57 GMT  
		Size: 5.3 MB (5285697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5268698aa228237d459083f95292fb3950668af1bc423300458662d6817006a`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71724157a7a130d88d6f3b3a62bcea37b4d6ef8e4c22799062a9949e1ae2294e`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:425d6efb65a0998268928f8d111c668cdb5bcc03a7a192b8ccf8d78e243d6ead
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33826685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff8a61fb95849a75c077007d48124a0e3aac5e00aa38c6850739bd6bcbbdb6cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 19:37:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 19:37:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 19:37:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 19:38:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 19:38:46 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 19:38:47 GMT
WORKDIR /spiped
# Wed, 12 May 2021 19:38:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 19:38:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 19:38:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55234c1dc3b0ed681bb0d6a515ee5325aa51350f28c96d9a835a08212f3ae83`  
		Last Modified: Wed, 12 May 2021 19:39:14 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4168bd2eacc4c8ba8aece3c064ea6727359406a6703c4736efc637e5d4c4b6bd`  
		Last Modified: Wed, 12 May 2021 19:39:14 GMT  
		Size: 2.0 MB (2007869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2f082f7dff3900e083123b15beb36bd2ec579a47204d92a40ffb22fa1b419d`  
		Last Modified: Wed, 12 May 2021 19:39:19 GMT  
		Size: 5.9 MB (5905354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d99e2ad24406eebd6451cc38a11a0395e83e86e58f59996b83364ec0e18e8`  
		Last Modified: Wed, 12 May 2021 19:39:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbf9d011ac895e52be82c5b195bc46de056831c6dd9f466584c655343f44a1b`  
		Last Modified: Wed, 12 May 2021 19:39:13 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:5e319479936eee4e789629c4b79d1720b52145a0ad529631647e842929a59996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41563204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76bac7e630d8ae86f4f836f8b090a8b003a681f6fd732d20f57d8662f9a02b3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:13:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 06:13:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:13:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 06:14:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 06:14:36 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 06:14:37 GMT
WORKDIR /spiped
# Wed, 12 May 2021 06:14:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 06:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:14:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a0f277245dd1b05ccbb1a6029229f7be99e59698537883010bc0a870700d5f`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daaa7f59c14ccc73a3a4cb78bb6c51185771bf7111f3985ba136a1f9fbdc683f`  
		Last Modified: Wed, 12 May 2021 06:15:19 GMT  
		Size: 2.1 MB (2132666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d5ae3e2d54344fa0d2eb0524dd0cfbd766ecef2ba8f16f933fbf8da5effb68`  
		Last Modified: Wed, 12 May 2021 06:15:21 GMT  
		Size: 11.6 MB (11633257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac63635bbb761f615b705a65a48368ae2f6530cbfaca13e0181713ca9eb752f`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ab0dac9585b965c6c6e54fb3b6d2784bc55b3749398040d858c1c282dc8d16`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:73b842b8648de250441f111a069985f2658d1cdb8e1bd091142cd013915805a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33943918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2703c88777e1bfbb7b151bdc9dff69d41d67e7ea4768c37d1a548605f4610a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:48:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 14:48:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:48:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 14:49:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 14:49:40 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 14:49:40 GMT
WORKDIR /spiped
# Wed, 12 May 2021 14:49:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 14:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 14:49:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d5ab1a7dfe229c365eac985c9888e5f9bd91a6f8b4827091c3beee0c3f4a8`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0b5f59d5c13ed0c6d4c539ff5e99f2458f180cb92cb90b933b7c1e5c69b643`  
		Last Modified: Wed, 12 May 2021 14:49:53 GMT  
		Size: 1.7 MB (1712452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b55c4319acfe89be8d0d190fa408f54c45acc0465a688cd810b672c862c004`  
		Last Modified: Wed, 12 May 2021 14:49:58 GMT  
		Size: 6.4 MB (6416412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df4593d00b37d8751d7acfcf1b4af789ea345b2d2ea1e43d91c0fe7fb2172a`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1527a275f222e2422b8469037f83cd67d8b47483dc6918befa20cf7ddada0816`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:cf18d0e1655d3071d9806a421f1978146647484cb65f745f60c9bb7155406fdf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39523409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787b7006873b0ca19028e9c0be65eefbc1f23f6bfcc47b8aa79d409644f5f14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:40:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 17:41:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:41:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 17:45:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 17:45:39 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 17:45:48 GMT
WORKDIR /spiped
# Wed, 12 May 2021 17:45:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 17:46:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 17:46:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e30106e0e567258ac9bdbf04a32f01e2871897e38e976f7b42537aa7f28c11a`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9021ed50e6c78d34322b096accc9e0778308ce19e73029ede0aa9b092b5f1`  
		Last Modified: Wed, 12 May 2021 17:46:40 GMT  
		Size: 2.2 MB (2225153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89585b290c82da4f3557bb03c9087ff570f0c41c2ba06240c70764097e8f59c`  
		Last Modified: Wed, 12 May 2021 17:46:41 GMT  
		Size: 6.7 MB (6743645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b15eb96c19d3049851885d6982137106dcf9e88720cecdbb0bc2bf9ce242480`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e4d8c0ffcd6ca31bc463f47c6e1cf1cd37f90c812f3471d57fbbb1cf98a99d`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:a45845a753efd776e495cdb7b19748e4d154bcae83ed61b0641dc7cb146e3df2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33527924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f554f74e1771a0e9e02db5ae99425227fa0c23048966969766356b2c739a28fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:52:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 07:52:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:52:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 07:53:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 07:53:32 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 07:53:33 GMT
WORKDIR /spiped
# Wed, 12 May 2021 07:53:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 07:53:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:53:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9965773f77d64c76e62f6586a8cc5ce4f21370e94b4ee2028598f65afc8fc8`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15772499dfa1ca6b51b5b6e1b62806ec4acd57f17f3458b41d33081dc9e5d3e7`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 1.8 MB (1821984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194ab3d8921fd77cf4980b3c52e6fa22d84e0f594ce5ed27c0d31323e12c1410`  
		Last Modified: Wed, 12 May 2021 07:54:01 GMT  
		Size: 5.9 MB (5943554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611dbc6789f5a10002010baf68d43e363fb7ce6c5b13b6f0517bfd6bfbdeec47`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db4fbf3d77db5a2cdb97512d17d9f46b3b5e82bcbd7a3eaac273a979f07ebc0`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:cb1ebb91215d457fba717379a9b2a39415b33fc337468ca1e81a1d9920ee431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:c21bef0140d90218ac109935fb4800c498f43c180f4ef1b10bde2642880be2a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbdf08613600d4c931da69207d9120e5ed8613c25036007e69cb1601a3e8f772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:43:02 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 03:43:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 03:43:05 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 03:43:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 03:43:32 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 03:43:33 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 03:43:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:43:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 03:43:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbdc5fa8a3b40bca444e39933121d87e99aab35af8b484d33aff845dc9223dc`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa32c269d5d00d85d7899e4eacf26aaba16e1172161bbf98004432c88ed2a5d8`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 7.0 KB (7043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60da1f1e01411c7d0f98a00b95e704a5e48286ab9625f96f051b85dd593d8e0`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 212.3 KB (212302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f836cc7647fd0c009041eafa0c5d574e4b5b58b6dc0918744c3c00cedeef407`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6dbf788a05da46939128eed6640869c6cd0ac3b637549bc7a664148c1d27cf`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:750e4a3e2b269c49615e43d6e3699988889b406b0c536a97f01713538717f8a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a6f4c383515708ecc75ec2c2164878f9c74553e6927b9614c53355f96bd64ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:12:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 06:12:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 06:12:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 06:13:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 06:13:02 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 06:13:03 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 06:13:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 06:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 06:13:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05304d4235002a8177d88a9a370a4001b168e9562193801a5939dcb96d98b928`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11429747878607e1935e81d7c9bf1da46083ab17322cfb24cdd9756402bf9eb`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6b2ca69864f244fd48c69f52a2aacb2cd2c1252a8c344bfda821704c3bb45c`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 202.3 KB (202275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd931a38883a95739ed26193356b8fa3a119d0971dc2de02eea8268fcb8d53d`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fd7e5e7757c92528d5a3fba0796309aca6a4e0e8a8ef9a0c9a8326f210bfa1`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:efce446ba8870e78476a9d75dcb1e52c175534d2b7ade2a215d811f2394fc147
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f48264b8ddafa8e951f93dc62b494ff4c0702ad2ed5d97967abeb08eca761330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:35:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 06:35:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 06:35:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 06:36:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 06:36:13 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 06:36:15 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 06:36:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 06:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 06:36:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498ba0cc83ce00b13dfa2f2b0f032008609655b0256c5050ef42ac51b4ac118a`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afde2e53b89bdc9bd82427372b10450afed8a06f7c059c1026a36d942d3ce4e9`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b9dc4c988b74b93e18af14d3edbf234cbb4c959d0ec118f1f35c4b93ec8d19`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a6650f750be3485d508aa8a969ee6542ea8f7c77318469b7276e9376e5037`  
		Last Modified: Thu, 15 Apr 2021 06:36:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514661aafe8081d75ec940a2e1e4fcbfecc2361f2a487ee7cadab8e66f187275`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:60db9b182fdba945554959c75b1bd2444da970be31220e2d374615effdef25ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e0fcfe18621392baf2b43c0bdebc4a5d06f004fe9bc9fffe47df640345b6c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:59:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:59:55 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:59:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 08:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 08:00:26 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 08:00:27 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 08:00:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 08:00:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:00:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71d2a4e9c8536bf553bccdfc5bd248d9d19fbed4f75e83dbe15d3d6ecfe5efd`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284753921e8453f385a71c0fe6cb527f691a28c3b968fbbd1352c7858a6f2915`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4dd4b0d19a431b27428bb2593842bdbcc8d064f50481e75d2c89ed75e42744`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 204.4 KB (204446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572e402105d138be04ffa652557707b95411f7e6845bcfd0f7fd6bf2c9588f80`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98458310d7c2648c532d1d5c331ea217dc4d80ad2467eb566702faf3d897d13`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d1f976abe7dc36865966c36ace3442df28cc760cfbc4325a00a692997a8bf0f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc0614ad90a95b7cd1f85bb13128b580a0c2f29ed00db4f65e968730c4f04440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:28:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:28:08 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:28:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:28:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:28:26 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:28:26 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:28:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:28:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:28:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a4072559715dd3774427ca5bfad06c46001c1d90638f2010ecca1cecb9435`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6417969d29e4f1c0fa56959b290e90527faca258d4dc8f876d5781b5a1d2ee7a`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08261970831fa426d9408c0c3cf638ab7d1ff006feef591eb4b6481ec2714464`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 223.3 KB (223281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dc16c21bb57966882a6696907c801efc77eccc10a5ad026e9bbb1e5316a800`  
		Last Modified: Thu, 15 Apr 2021 07:28:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff154aa157546b5d51db233328ebbed740e8854de199b27d502820e45e65bbad`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9d383336851f89b74885b174acf82891ef2bf8c945a6373dec31ca6676fd1107
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fd56c4b0659f3c04e8bff71019d31b85529f0f9a53b88c69fb81d0bfe3351c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:03:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:03:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:03:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:04:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:04:28 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:04:35 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:04:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:04:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:04:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602add23d4a6d2eadfe98b28abe912c5fcac90dbe9c2a51a54f428ad33d692ee`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451504af2e04d8b41445eedc1f1f9c76a59c85eb2be170be0d8aa078d0aa93e9`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 7.1 KB (7065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd1d09b1e4f40662048b2b792797406a48e2cb33e7e0c06a3b60ff7f189ee3e`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 221.0 KB (220986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38387eb6968cbda04a7e8b097378ba4eba871862d73839fa97fc66d70f606c32`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b42ba1d6389eba3e53edf2210a840a60b804cc8e51a81a4f42bcc86848d85a`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:e7b696fd86c235eb96fb948d3ca260c9e80e416b43bb9be3a0597947f56ea431
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

### `spiped:1.6.1` - linux; amd64

```console
$ docker pull spiped@sha256:bcaed8de930b8832a40873acf6861bf984e70edf571e971f372f24da4f008b1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36313953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8da550658c999941253a73bc835fb7a71f6af0881ad9610d662638086f2c833a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:27:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 17:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:27:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 17:28:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 17:28:06 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 17:28:06 GMT
WORKDIR /spiped
# Wed, 12 May 2021 17:28:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 17:28:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 17:28:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80866732d602112cb309734d5fdb453f07a1e00ff5eebb449821148acbe03ee9`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5c28b22404235df98f9f542c8393d1694d19406863a5f7b1b8bfb2079a9477`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 2.1 MB (2128505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2da39cf8d05feb934e294e041fa92e75f5f1071abf10b086c21bfeca751164`  
		Last Modified: Wed, 12 May 2021 17:28:28 GMT  
		Size: 7.0 MB (7037329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaaa5bc95b1a83402d28c94b0e297cbc4dbdcd89c127a71d41700fc5d67ff64`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb6ca2836a313b7d46ad352635e75d68ad5297f638713a4bad872abba008f8a`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3f9e7be1ab568265c3dd6fa509c7c114c1879a02c3bded42f54fd11289735e1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32201133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:563fe344ab3950b18fe739f7280a4ceee978289d27c277c471a187c606fcb931`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:10:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 02:11:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:11:14 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 02:12:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 02:12:13 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 02:12:14 GMT
WORKDIR /spiped
# Wed, 12 May 2021 02:12:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 02:12:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:12:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93994a565732f80afb936f17eea4a465d85e20d35c345d8a882fdeae92f0d59c`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d836928393044684b89355c1804a6258f852af61457a0915ae433c3406eed`  
		Last Modified: Wed, 12 May 2021 02:12:44 GMT  
		Size: 1.8 MB (1839342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d98e02b46e64902855f44d27903de22548a6800fbcba76c18a2aa89fa538ec`  
		Last Modified: Wed, 12 May 2021 02:12:45 GMT  
		Size: 5.5 MB (5479993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4cf9810da7adb24dae3073d41ef246afb43ba96eb5565f9f0508b31872735f`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd46064d587a7a824767f89a11f12af984145bc88a9d042bc0b83a34ad8dcbdf`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:182834a86cf1b16639e086952aa1628bfe56c89d0539d1e239fc09c7ae3481aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6e06b72812b074a05d2ed74589ec9a23a1529a74f73c3aa00941c8ce50cc14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 20:08:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 20:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 20:09:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 20:10:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 20:10:22 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 20:10:24 GMT
WORKDIR /spiped
# Wed, 12 May 2021 20:10:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 20:10:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 20:10:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b39d1ef66a2842eb5175ad816ce0160e49aea4e5cd37db71923a26983f63800`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b1cea5297efcedcf7f3656dd7ad9811a22abf743c8799650421f5c5b2ca521`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 1.8 MB (1759508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b338f8510b528b02e5e16346ae09c6f9a04a1782956218d76b3b9d3eb7747`  
		Last Modified: Wed, 12 May 2021 20:10:57 GMT  
		Size: 5.3 MB (5285697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5268698aa228237d459083f95292fb3950668af1bc423300458662d6817006a`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71724157a7a130d88d6f3b3a62bcea37b4d6ef8e4c22799062a9949e1ae2294e`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:425d6efb65a0998268928f8d111c668cdb5bcc03a7a192b8ccf8d78e243d6ead
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33826685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff8a61fb95849a75c077007d48124a0e3aac5e00aa38c6850739bd6bcbbdb6cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 19:37:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 19:37:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 19:37:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 19:38:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 19:38:46 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 19:38:47 GMT
WORKDIR /spiped
# Wed, 12 May 2021 19:38:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 19:38:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 19:38:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55234c1dc3b0ed681bb0d6a515ee5325aa51350f28c96d9a835a08212f3ae83`  
		Last Modified: Wed, 12 May 2021 19:39:14 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4168bd2eacc4c8ba8aece3c064ea6727359406a6703c4736efc637e5d4c4b6bd`  
		Last Modified: Wed, 12 May 2021 19:39:14 GMT  
		Size: 2.0 MB (2007869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2f082f7dff3900e083123b15beb36bd2ec579a47204d92a40ffb22fa1b419d`  
		Last Modified: Wed, 12 May 2021 19:39:19 GMT  
		Size: 5.9 MB (5905354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d99e2ad24406eebd6451cc38a11a0395e83e86e58f59996b83364ec0e18e8`  
		Last Modified: Wed, 12 May 2021 19:39:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbf9d011ac895e52be82c5b195bc46de056831c6dd9f466584c655343f44a1b`  
		Last Modified: Wed, 12 May 2021 19:39:13 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:5e319479936eee4e789629c4b79d1720b52145a0ad529631647e842929a59996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41563204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76bac7e630d8ae86f4f836f8b090a8b003a681f6fd732d20f57d8662f9a02b3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:13:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 06:13:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:13:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 06:14:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 06:14:36 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 06:14:37 GMT
WORKDIR /spiped
# Wed, 12 May 2021 06:14:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 06:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:14:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a0f277245dd1b05ccbb1a6029229f7be99e59698537883010bc0a870700d5f`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daaa7f59c14ccc73a3a4cb78bb6c51185771bf7111f3985ba136a1f9fbdc683f`  
		Last Modified: Wed, 12 May 2021 06:15:19 GMT  
		Size: 2.1 MB (2132666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d5ae3e2d54344fa0d2eb0524dd0cfbd766ecef2ba8f16f933fbf8da5effb68`  
		Last Modified: Wed, 12 May 2021 06:15:21 GMT  
		Size: 11.6 MB (11633257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac63635bbb761f615b705a65a48368ae2f6530cbfaca13e0181713ca9eb752f`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ab0dac9585b965c6c6e54fb3b6d2784bc55b3749398040d858c1c282dc8d16`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:73b842b8648de250441f111a069985f2658d1cdb8e1bd091142cd013915805a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33943918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2703c88777e1bfbb7b151bdc9dff69d41d67e7ea4768c37d1a548605f4610a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:48:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 14:48:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:48:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 14:49:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 14:49:40 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 14:49:40 GMT
WORKDIR /spiped
# Wed, 12 May 2021 14:49:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 14:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 14:49:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d5ab1a7dfe229c365eac985c9888e5f9bd91a6f8b4827091c3beee0c3f4a8`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0b5f59d5c13ed0c6d4c539ff5e99f2458f180cb92cb90b933b7c1e5c69b643`  
		Last Modified: Wed, 12 May 2021 14:49:53 GMT  
		Size: 1.7 MB (1712452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b55c4319acfe89be8d0d190fa408f54c45acc0465a688cd810b672c862c004`  
		Last Modified: Wed, 12 May 2021 14:49:58 GMT  
		Size: 6.4 MB (6416412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df4593d00b37d8751d7acfcf1b4af789ea345b2d2ea1e43d91c0fe7fb2172a`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1527a275f222e2422b8469037f83cd67d8b47483dc6918befa20cf7ddada0816`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:cf18d0e1655d3071d9806a421f1978146647484cb65f745f60c9bb7155406fdf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39523409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787b7006873b0ca19028e9c0be65eefbc1f23f6bfcc47b8aa79d409644f5f14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:40:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 17:41:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:41:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 17:45:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 17:45:39 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 17:45:48 GMT
WORKDIR /spiped
# Wed, 12 May 2021 17:45:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 17:46:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 17:46:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e30106e0e567258ac9bdbf04a32f01e2871897e38e976f7b42537aa7f28c11a`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9021ed50e6c78d34322b096accc9e0778308ce19e73029ede0aa9b092b5f1`  
		Last Modified: Wed, 12 May 2021 17:46:40 GMT  
		Size: 2.2 MB (2225153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89585b290c82da4f3557bb03c9087ff570f0c41c2ba06240c70764097e8f59c`  
		Last Modified: Wed, 12 May 2021 17:46:41 GMT  
		Size: 6.7 MB (6743645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b15eb96c19d3049851885d6982137106dcf9e88720cecdbb0bc2bf9ce242480`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e4d8c0ffcd6ca31bc463f47c6e1cf1cd37f90c812f3471d57fbbb1cf98a99d`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:a45845a753efd776e495cdb7b19748e4d154bcae83ed61b0641dc7cb146e3df2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33527924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f554f74e1771a0e9e02db5ae99425227fa0c23048966969766356b2c739a28fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:52:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 07:52:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:52:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 07:53:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 07:53:32 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 07:53:33 GMT
WORKDIR /spiped
# Wed, 12 May 2021 07:53:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 07:53:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:53:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9965773f77d64c76e62f6586a8cc5ce4f21370e94b4ee2028598f65afc8fc8`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15772499dfa1ca6b51b5b6e1b62806ec4acd57f17f3458b41d33081dc9e5d3e7`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 1.8 MB (1821984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194ab3d8921fd77cf4980b3c52e6fa22d84e0f594ce5ed27c0d31323e12c1410`  
		Last Modified: Wed, 12 May 2021 07:54:01 GMT  
		Size: 5.9 MB (5943554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611dbc6789f5a10002010baf68d43e363fb7ce6c5b13b6f0517bfd6bfbdeec47`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db4fbf3d77db5a2cdb97512d17d9f46b3b5e82bcbd7a3eaac273a979f07ebc0`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:cb1ebb91215d457fba717379a9b2a39415b33fc337468ca1e81a1d9920ee431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:c21bef0140d90218ac109935fb4800c498f43c180f4ef1b10bde2642880be2a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbdf08613600d4c931da69207d9120e5ed8613c25036007e69cb1601a3e8f772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:43:02 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 03:43:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 03:43:05 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 03:43:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 03:43:32 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 03:43:33 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 03:43:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:43:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 03:43:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbdc5fa8a3b40bca444e39933121d87e99aab35af8b484d33aff845dc9223dc`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa32c269d5d00d85d7899e4eacf26aaba16e1172161bbf98004432c88ed2a5d8`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 7.0 KB (7043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60da1f1e01411c7d0f98a00b95e704a5e48286ab9625f96f051b85dd593d8e0`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 212.3 KB (212302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f836cc7647fd0c009041eafa0c5d574e4b5b58b6dc0918744c3c00cedeef407`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6dbf788a05da46939128eed6640869c6cd0ac3b637549bc7a664148c1d27cf`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:750e4a3e2b269c49615e43d6e3699988889b406b0c536a97f01713538717f8a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a6f4c383515708ecc75ec2c2164878f9c74553e6927b9614c53355f96bd64ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:12:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 06:12:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 06:12:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 06:13:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 06:13:02 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 06:13:03 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 06:13:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 06:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 06:13:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05304d4235002a8177d88a9a370a4001b168e9562193801a5939dcb96d98b928`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11429747878607e1935e81d7c9bf1da46083ab17322cfb24cdd9756402bf9eb`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6b2ca69864f244fd48c69f52a2aacb2cd2c1252a8c344bfda821704c3bb45c`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 202.3 KB (202275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd931a38883a95739ed26193356b8fa3a119d0971dc2de02eea8268fcb8d53d`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fd7e5e7757c92528d5a3fba0796309aca6a4e0e8a8ef9a0c9a8326f210bfa1`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:efce446ba8870e78476a9d75dcb1e52c175534d2b7ade2a215d811f2394fc147
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f48264b8ddafa8e951f93dc62b494ff4c0702ad2ed5d97967abeb08eca761330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:35:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 06:35:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 06:35:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 06:36:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 06:36:13 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 06:36:15 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 06:36:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 06:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 06:36:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498ba0cc83ce00b13dfa2f2b0f032008609655b0256c5050ef42ac51b4ac118a`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afde2e53b89bdc9bd82427372b10450afed8a06f7c059c1026a36d942d3ce4e9`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b9dc4c988b74b93e18af14d3edbf234cbb4c959d0ec118f1f35c4b93ec8d19`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a6650f750be3485d508aa8a969ee6542ea8f7c77318469b7276e9376e5037`  
		Last Modified: Thu, 15 Apr 2021 06:36:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514661aafe8081d75ec940a2e1e4fcbfecc2361f2a487ee7cadab8e66f187275`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:60db9b182fdba945554959c75b1bd2444da970be31220e2d374615effdef25ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e0fcfe18621392baf2b43c0bdebc4a5d06f004fe9bc9fffe47df640345b6c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:59:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:59:55 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:59:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 08:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 08:00:26 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 08:00:27 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 08:00:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 08:00:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:00:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71d2a4e9c8536bf553bccdfc5bd248d9d19fbed4f75e83dbe15d3d6ecfe5efd`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284753921e8453f385a71c0fe6cb527f691a28c3b968fbbd1352c7858a6f2915`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4dd4b0d19a431b27428bb2593842bdbcc8d064f50481e75d2c89ed75e42744`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 204.4 KB (204446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572e402105d138be04ffa652557707b95411f7e6845bcfd0f7fd6bf2c9588f80`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98458310d7c2648c532d1d5c331ea217dc4d80ad2467eb566702faf3d897d13`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d1f976abe7dc36865966c36ace3442df28cc760cfbc4325a00a692997a8bf0f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc0614ad90a95b7cd1f85bb13128b580a0c2f29ed00db4f65e968730c4f04440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:28:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:28:08 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:28:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:28:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:28:26 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:28:26 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:28:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:28:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:28:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a4072559715dd3774427ca5bfad06c46001c1d90638f2010ecca1cecb9435`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6417969d29e4f1c0fa56959b290e90527faca258d4dc8f876d5781b5a1d2ee7a`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08261970831fa426d9408c0c3cf638ab7d1ff006feef591eb4b6481ec2714464`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 223.3 KB (223281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dc16c21bb57966882a6696907c801efc77eccc10a5ad026e9bbb1e5316a800`  
		Last Modified: Thu, 15 Apr 2021 07:28:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff154aa157546b5d51db233328ebbed740e8854de199b27d502820e45e65bbad`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9d383336851f89b74885b174acf82891ef2bf8c945a6373dec31ca6676fd1107
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fd56c4b0659f3c04e8bff71019d31b85529f0f9a53b88c69fb81d0bfe3351c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:03:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:03:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:03:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:04:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:04:28 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:04:35 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:04:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:04:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:04:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602add23d4a6d2eadfe98b28abe912c5fcac90dbe9c2a51a54f428ad33d692ee`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451504af2e04d8b41445eedc1f1f9c76a59c85eb2be170be0d8aa078d0aa93e9`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 7.1 KB (7065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd1d09b1e4f40662048b2b792797406a48e2cb33e7e0c06a3b60ff7f189ee3e`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 221.0 KB (220986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38387eb6968cbda04a7e8b097378ba4eba871862d73839fa97fc66d70f606c32`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b42ba1d6389eba3e53edf2210a840a60b804cc8e51a81a4f42bcc86848d85a`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:cb1ebb91215d457fba717379a9b2a39415b33fc337468ca1e81a1d9920ee431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:c21bef0140d90218ac109935fb4800c498f43c180f4ef1b10bde2642880be2a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbdf08613600d4c931da69207d9120e5ed8613c25036007e69cb1601a3e8f772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:43:02 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 03:43:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 03:43:05 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 03:43:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 03:43:32 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 03:43:33 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 03:43:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:43:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 03:43:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbdc5fa8a3b40bca444e39933121d87e99aab35af8b484d33aff845dc9223dc`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa32c269d5d00d85d7899e4eacf26aaba16e1172161bbf98004432c88ed2a5d8`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 7.0 KB (7043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60da1f1e01411c7d0f98a00b95e704a5e48286ab9625f96f051b85dd593d8e0`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 212.3 KB (212302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f836cc7647fd0c009041eafa0c5d574e4b5b58b6dc0918744c3c00cedeef407`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6dbf788a05da46939128eed6640869c6cd0ac3b637549bc7a664148c1d27cf`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:750e4a3e2b269c49615e43d6e3699988889b406b0c536a97f01713538717f8a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a6f4c383515708ecc75ec2c2164878f9c74553e6927b9614c53355f96bd64ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:12:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 06:12:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 06:12:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 06:13:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 06:13:02 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 06:13:03 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 06:13:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 06:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 06:13:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05304d4235002a8177d88a9a370a4001b168e9562193801a5939dcb96d98b928`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11429747878607e1935e81d7c9bf1da46083ab17322cfb24cdd9756402bf9eb`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6b2ca69864f244fd48c69f52a2aacb2cd2c1252a8c344bfda821704c3bb45c`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 202.3 KB (202275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd931a38883a95739ed26193356b8fa3a119d0971dc2de02eea8268fcb8d53d`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fd7e5e7757c92528d5a3fba0796309aca6a4e0e8a8ef9a0c9a8326f210bfa1`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:efce446ba8870e78476a9d75dcb1e52c175534d2b7ade2a215d811f2394fc147
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f48264b8ddafa8e951f93dc62b494ff4c0702ad2ed5d97967abeb08eca761330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:35:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 06:35:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 06:35:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 06:36:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 06:36:13 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 06:36:15 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 06:36:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 06:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 06:36:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498ba0cc83ce00b13dfa2f2b0f032008609655b0256c5050ef42ac51b4ac118a`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afde2e53b89bdc9bd82427372b10450afed8a06f7c059c1026a36d942d3ce4e9`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b9dc4c988b74b93e18af14d3edbf234cbb4c959d0ec118f1f35c4b93ec8d19`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a6650f750be3485d508aa8a969ee6542ea8f7c77318469b7276e9376e5037`  
		Last Modified: Thu, 15 Apr 2021 06:36:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514661aafe8081d75ec940a2e1e4fcbfecc2361f2a487ee7cadab8e66f187275`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:60db9b182fdba945554959c75b1bd2444da970be31220e2d374615effdef25ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e0fcfe18621392baf2b43c0bdebc4a5d06f004fe9bc9fffe47df640345b6c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:59:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:59:55 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:59:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 08:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 08:00:26 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 08:00:27 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 08:00:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 08:00:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:00:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71d2a4e9c8536bf553bccdfc5bd248d9d19fbed4f75e83dbe15d3d6ecfe5efd`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284753921e8453f385a71c0fe6cb527f691a28c3b968fbbd1352c7858a6f2915`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4dd4b0d19a431b27428bb2593842bdbcc8d064f50481e75d2c89ed75e42744`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 204.4 KB (204446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572e402105d138be04ffa652557707b95411f7e6845bcfd0f7fd6bf2c9588f80`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98458310d7c2648c532d1d5c331ea217dc4d80ad2467eb566702faf3d897d13`  
		Last Modified: Thu, 15 Apr 2021 08:00:51 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:d1f976abe7dc36865966c36ace3442df28cc760cfbc4325a00a692997a8bf0f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc0614ad90a95b7cd1f85bb13128b580a0c2f29ed00db4f65e968730c4f04440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:28:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:28:08 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:28:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:28:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:28:26 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:28:26 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:28:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:28:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:28:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a4072559715dd3774427ca5bfad06c46001c1d90638f2010ecca1cecb9435`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6417969d29e4f1c0fa56959b290e90527faca258d4dc8f876d5781b5a1d2ee7a`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08261970831fa426d9408c0c3cf638ab7d1ff006feef591eb4b6481ec2714464`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 223.3 KB (223281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dc16c21bb57966882a6696907c801efc77eccc10a5ad026e9bbb1e5316a800`  
		Last Modified: Thu, 15 Apr 2021 07:28:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff154aa157546b5d51db233328ebbed740e8854de199b27d502820e45e65bbad`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9d383336851f89b74885b174acf82891ef2bf8c945a6373dec31ca6676fd1107
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fd56c4b0659f3c04e8bff71019d31b85529f0f9a53b88c69fb81d0bfe3351c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:03:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:03:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:03:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:04:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:04:28 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:04:35 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:04:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:04:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:04:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602add23d4a6d2eadfe98b28abe912c5fcac90dbe9c2a51a54f428ad33d692ee`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451504af2e04d8b41445eedc1f1f9c76a59c85eb2be170be0d8aa078d0aa93e9`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 7.1 KB (7065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd1d09b1e4f40662048b2b792797406a48e2cb33e7e0c06a3b60ff7f189ee3e`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 221.0 KB (220986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38387eb6968cbda04a7e8b097378ba4eba871862d73839fa97fc66d70f606c32`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b42ba1d6389eba3e53edf2210a840a60b804cc8e51a81a4f42bcc86848d85a`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:e7b696fd86c235eb96fb948d3ca260c9e80e416b43bb9be3a0597947f56ea431
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

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:bcaed8de930b8832a40873acf6861bf984e70edf571e971f372f24da4f008b1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36313953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8da550658c999941253a73bc835fb7a71f6af0881ad9610d662638086f2c833a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:27:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 17:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:27:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 17:28:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 17:28:06 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 17:28:06 GMT
WORKDIR /spiped
# Wed, 12 May 2021 17:28:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 17:28:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 17:28:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80866732d602112cb309734d5fdb453f07a1e00ff5eebb449821148acbe03ee9`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5c28b22404235df98f9f542c8393d1694d19406863a5f7b1b8bfb2079a9477`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 2.1 MB (2128505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2da39cf8d05feb934e294e041fa92e75f5f1071abf10b086c21bfeca751164`  
		Last Modified: Wed, 12 May 2021 17:28:28 GMT  
		Size: 7.0 MB (7037329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaaa5bc95b1a83402d28c94b0e297cbc4dbdcd89c127a71d41700fc5d67ff64`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb6ca2836a313b7d46ad352635e75d68ad5297f638713a4bad872abba008f8a`  
		Last Modified: Wed, 12 May 2021 17:28:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3f9e7be1ab568265c3dd6fa509c7c114c1879a02c3bded42f54fd11289735e1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32201133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:563fe344ab3950b18fe739f7280a4ceee978289d27c277c471a187c606fcb931`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:10:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 02:11:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:11:14 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 02:12:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 02:12:13 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 02:12:14 GMT
WORKDIR /spiped
# Wed, 12 May 2021 02:12:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 02:12:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:12:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93994a565732f80afb936f17eea4a465d85e20d35c345d8a882fdeae92f0d59c`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d836928393044684b89355c1804a6258f852af61457a0915ae433c3406eed`  
		Last Modified: Wed, 12 May 2021 02:12:44 GMT  
		Size: 1.8 MB (1839342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d98e02b46e64902855f44d27903de22548a6800fbcba76c18a2aa89fa538ec`  
		Last Modified: Wed, 12 May 2021 02:12:45 GMT  
		Size: 5.5 MB (5479993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4cf9810da7adb24dae3073d41ef246afb43ba96eb5565f9f0508b31872735f`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd46064d587a7a824767f89a11f12af984145bc88a9d042bc0b83a34ad8dcbdf`  
		Last Modified: Wed, 12 May 2021 02:12:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:182834a86cf1b16639e086952aa1628bfe56c89d0539d1e239fc09c7ae3481aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6e06b72812b074a05d2ed74589ec9a23a1529a74f73c3aa00941c8ce50cc14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 20:08:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 20:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 20:09:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 20:10:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 20:10:22 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 20:10:24 GMT
WORKDIR /spiped
# Wed, 12 May 2021 20:10:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 20:10:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 20:10:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b39d1ef66a2842eb5175ad816ce0160e49aea4e5cd37db71923a26983f63800`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b1cea5297efcedcf7f3656dd7ad9811a22abf743c8799650421f5c5b2ca521`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 1.8 MB (1759508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b338f8510b528b02e5e16346ae09c6f9a04a1782956218d76b3b9d3eb7747`  
		Last Modified: Wed, 12 May 2021 20:10:57 GMT  
		Size: 5.3 MB (5285697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5268698aa228237d459083f95292fb3950668af1bc423300458662d6817006a`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71724157a7a130d88d6f3b3a62bcea37b4d6ef8e4c22799062a9949e1ae2294e`  
		Last Modified: Wed, 12 May 2021 20:10:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:425d6efb65a0998268928f8d111c668cdb5bcc03a7a192b8ccf8d78e243d6ead
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33826685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff8a61fb95849a75c077007d48124a0e3aac5e00aa38c6850739bd6bcbbdb6cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 19:37:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 19:37:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 19:37:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 19:38:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 19:38:46 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 19:38:47 GMT
WORKDIR /spiped
# Wed, 12 May 2021 19:38:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 19:38:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 19:38:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55234c1dc3b0ed681bb0d6a515ee5325aa51350f28c96d9a835a08212f3ae83`  
		Last Modified: Wed, 12 May 2021 19:39:14 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4168bd2eacc4c8ba8aece3c064ea6727359406a6703c4736efc637e5d4c4b6bd`  
		Last Modified: Wed, 12 May 2021 19:39:14 GMT  
		Size: 2.0 MB (2007869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2f082f7dff3900e083123b15beb36bd2ec579a47204d92a40ffb22fa1b419d`  
		Last Modified: Wed, 12 May 2021 19:39:19 GMT  
		Size: 5.9 MB (5905354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d99e2ad24406eebd6451cc38a11a0395e83e86e58f59996b83364ec0e18e8`  
		Last Modified: Wed, 12 May 2021 19:39:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbf9d011ac895e52be82c5b195bc46de056831c6dd9f466584c655343f44a1b`  
		Last Modified: Wed, 12 May 2021 19:39:13 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:5e319479936eee4e789629c4b79d1720b52145a0ad529631647e842929a59996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41563204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76bac7e630d8ae86f4f836f8b090a8b003a681f6fd732d20f57d8662f9a02b3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:13:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 06:13:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:13:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 06:14:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 06:14:36 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 06:14:37 GMT
WORKDIR /spiped
# Wed, 12 May 2021 06:14:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 06:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:14:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a0f277245dd1b05ccbb1a6029229f7be99e59698537883010bc0a870700d5f`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daaa7f59c14ccc73a3a4cb78bb6c51185771bf7111f3985ba136a1f9fbdc683f`  
		Last Modified: Wed, 12 May 2021 06:15:19 GMT  
		Size: 2.1 MB (2132666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d5ae3e2d54344fa0d2eb0524dd0cfbd766ecef2ba8f16f933fbf8da5effb68`  
		Last Modified: Wed, 12 May 2021 06:15:21 GMT  
		Size: 11.6 MB (11633257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac63635bbb761f615b705a65a48368ae2f6530cbfaca13e0181713ca9eb752f`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ab0dac9585b965c6c6e54fb3b6d2784bc55b3749398040d858c1c282dc8d16`  
		Last Modified: Wed, 12 May 2021 06:15:18 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:73b842b8648de250441f111a069985f2658d1cdb8e1bd091142cd013915805a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33943918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2703c88777e1bfbb7b151bdc9dff69d41d67e7ea4768c37d1a548605f4610a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:48:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 14:48:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:48:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 14:49:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 14:49:40 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 14:49:40 GMT
WORKDIR /spiped
# Wed, 12 May 2021 14:49:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 14:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 14:49:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d5ab1a7dfe229c365eac985c9888e5f9bd91a6f8b4827091c3beee0c3f4a8`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0b5f59d5c13ed0c6d4c539ff5e99f2458f180cb92cb90b933b7c1e5c69b643`  
		Last Modified: Wed, 12 May 2021 14:49:53 GMT  
		Size: 1.7 MB (1712452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b55c4319acfe89be8d0d190fa408f54c45acc0465a688cd810b672c862c004`  
		Last Modified: Wed, 12 May 2021 14:49:58 GMT  
		Size: 6.4 MB (6416412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df4593d00b37d8751d7acfcf1b4af789ea345b2d2ea1e43d91c0fe7fb2172a`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1527a275f222e2422b8469037f83cd67d8b47483dc6918befa20cf7ddada0816`  
		Last Modified: Wed, 12 May 2021 14:49:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:cf18d0e1655d3071d9806a421f1978146647484cb65f745f60c9bb7155406fdf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39523409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787b7006873b0ca19028e9c0be65eefbc1f23f6bfcc47b8aa79d409644f5f14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:40:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 17:41:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:41:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 17:45:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 17:45:39 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 17:45:48 GMT
WORKDIR /spiped
# Wed, 12 May 2021 17:45:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 17:46:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 17:46:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e30106e0e567258ac9bdbf04a32f01e2871897e38e976f7b42537aa7f28c11a`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9021ed50e6c78d34322b096accc9e0778308ce19e73029ede0aa9b092b5f1`  
		Last Modified: Wed, 12 May 2021 17:46:40 GMT  
		Size: 2.2 MB (2225153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89585b290c82da4f3557bb03c9087ff570f0c41c2ba06240c70764097e8f59c`  
		Last Modified: Wed, 12 May 2021 17:46:41 GMT  
		Size: 6.7 MB (6743645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b15eb96c19d3049851885d6982137106dcf9e88720cecdbb0bc2bf9ce242480`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e4d8c0ffcd6ca31bc463f47c6e1cf1cd37f90c812f3471d57fbbb1cf98a99d`  
		Last Modified: Wed, 12 May 2021 17:46:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:a45845a753efd776e495cdb7b19748e4d154bcae83ed61b0641dc7cb146e3df2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33527924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f554f74e1771a0e9e02db5ae99425227fa0c23048966969766356b2c739a28fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:52:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 May 2021 07:52:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:52:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 12 May 2021 07:53:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 May 2021 07:53:32 GMT
VOLUME [/spiped]
# Wed, 12 May 2021 07:53:33 GMT
WORKDIR /spiped
# Wed, 12 May 2021 07:53:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 May 2021 07:53:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:53:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9965773f77d64c76e62f6586a8cc5ce4f21370e94b4ee2028598f65afc8fc8`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15772499dfa1ca6b51b5b6e1b62806ec4acd57f17f3458b41d33081dc9e5d3e7`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 1.8 MB (1821984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194ab3d8921fd77cf4980b3c52e6fa22d84e0f594ce5ed27c0d31323e12c1410`  
		Last Modified: Wed, 12 May 2021 07:54:01 GMT  
		Size: 5.9 MB (5943554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611dbc6789f5a10002010baf68d43e363fb7ce6c5b13b6f0517bfd6bfbdeec47`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db4fbf3d77db5a2cdb97512d17d9f46b3b5e82bcbd7a3eaac273a979f07ebc0`  
		Last Modified: Wed, 12 May 2021 07:54:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
