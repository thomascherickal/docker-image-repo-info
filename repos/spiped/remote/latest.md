## `spiped:latest`

```console
$ docker pull spiped@sha256:92554ea69af2516989f19878a3cd91bb9ac905a5d62f088ceaddedaaad218bc9
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
$ docker pull spiped@sha256:a73406b0627816d275ab28a8943632099ce2bfd1759fcead98420dffeb279527
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33826498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be85b88608bfb471363b133a6df71bfe20be26101251db56af10afbe0a98f4f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 11:13:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Jun 2021 11:13:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Jun 2021 11:13:14 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 16 Jun 2021 11:13:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Jun 2021 11:13:35 GMT
VOLUME [/spiped]
# Wed, 16 Jun 2021 11:13:36 GMT
WORKDIR /spiped
# Wed, 16 Jun 2021 11:13:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:13:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:13:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85048845245d74b01b78212d19011f49a8b3b6b4a2821fdf7382078e8c3df090`  
		Last Modified: Wed, 16 Jun 2021 11:14:30 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc80573002d17d67cc65f30971f765e28e0cab1649003a7d35798daad1d47b66`  
		Last Modified: Wed, 16 Jun 2021 11:14:30 GMT  
		Size: 2.0 MB (2007821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4949efce4254108152786f7b1c1fe0778a28cba8e3117e5dcd34c806dcb89`  
		Last Modified: Wed, 16 Jun 2021 11:14:31 GMT  
		Size: 5.9 MB (5905215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa36c815c53c7e21a40d3348012eb84ee0fba917f62c31abc30a77a15f4c3fd`  
		Last Modified: Wed, 16 Jun 2021 11:14:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57793fe0957ac2861206a809269317441db7c7481eaf091077c2af4152a6c0ea`  
		Last Modified: Wed, 16 Jun 2021 11:14:30 GMT  
		Size: 341.0 B  
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
