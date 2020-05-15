<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6.1`](#spiped161)
-	[`spiped:1.6.1-alpine`](#spiped161-alpine)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:0974779f94eefdaceee919a3fa3a13f276c511df256f137122f6c92321ba1ec1
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
$ docker pull spiped@sha256:7210ee044384bbf33b10cb67ac7553d668f7153c33d585d44f0f094802211935
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36265955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe93473ad7fbf7cfe45ec029c8e6ecceb7d566ee348606465258b48d44fb7a74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 20:03:27 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 20:03:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 20:03:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 20:03:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 20:03:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 20:04:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 20:04:04 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 20:04:04 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 20:04:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 20:04:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 20:04:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eddd5e303f5c1f7165d495e17bddc0f2de7f6a442bed4aa5ac459a6ac611b1c`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1abc5f67f536b64df626692b5282ca4c22723857a6aeac95cd33d3f4e308953`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 2.1 MB (2128047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ea5550680d87a6bc6b46386fee970f0570d3f04daaa7bae1d430dc370df4e`  
		Last Modified: Thu, 23 Apr 2020 20:04:25 GMT  
		Size: 7.0 MB (7037480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011c1a0f8d8f204ab1ffc14fbf98193e3b50980b4eb88e30498b32aba5327dc2`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ce919881dee3bbed53f0207ca6833b9a955ea08c97e3556207898ed438b880`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:684ff0c8dfb3841271f5206b43eb09bf67b7ce4ed227991695b458ef2c433378
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32159776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58bbf4cfd7f41654132e8864655fe8c89653e455477752eca0c0f8f6fefb701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:17:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 03:17:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:17:30 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 03:17:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 03:17:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 03:18:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 03:18:40 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 03:18:41 GMT
WORKDIR /spiped
# Fri, 15 May 2020 03:18:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 03:18:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 03:18:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b0bb0a243296a03a7eb3d5685e105963e7740f828fe89200768b8b03d8c145`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355ea8b47d3eb64e79c3ff6b960d39905709329fc410b679ed67fb6a046e11b6`  
		Last Modified: Fri, 15 May 2020 03:19:08 GMT  
		Size: 1.8 MB (1839134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508622f07ba3c6a59ea9a8bafcc356fe7a02e3cef578e40fc352ddc9936f49e6`  
		Last Modified: Fri, 15 May 2020 03:19:10 GMT  
		Size: 5.5 MB (5479971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f8b3d25b951be8ffd5d1b88cdd703030efd6b6e389fa2fbb55bb0897b9d88c`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf14b5beaa983bb77e805228142604932caf4aedd9c3056e4e4a369791d06f1b`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:87e594e6c297ab32b63899e657c1a54a8d1100d3b615aba3110b9c83af034bf4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3762d7fbd521ea9dd741d0c9728f84de283ec800689749f6154163ac375146ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:37:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 06:37:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 06:37:12 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 06:37:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 06:37:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 06:38:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 06:38:07 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 06:38:07 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 06:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 06:38:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c245760c54fc8d94586399ec9055355e4c3366a9bbb2fa8adfc6f906feb4be2e`  
		Last Modified: Thu, 23 Apr 2020 06:38:30 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e881f703761ee378af97245f067193b18a2e259c6960350af6bd58c50c17c9`  
		Last Modified: Thu, 23 Apr 2020 06:38:31 GMT  
		Size: 1.8 MB (1759439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff85ebb091bd4c189eb2fbb13813d47c9bb4a87981d5e5e7f024ba3a70413717`  
		Last Modified: Thu, 23 Apr 2020 06:38:33 GMT  
		Size: 5.3 MB (5285357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe372689bc3dcd9f9fcc3170419cbe8cdf8289b8ab46d6658e6f9afdb311b92`  
		Last Modified: Thu, 23 Apr 2020 06:38:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a07c2d12354b78115b49045a435919c09508a793f325a501637f134f608c3`  
		Last Modified: Thu, 23 Apr 2020 06:38:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:3c11c283fe0418525bef456d87e13fb1eda7daa8405bd41f740174fa8f17ba86
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99399f5684ebefda91f2d63ec0d8e8ea2262734018b10b7294427a56aa48bbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 15:52:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 15:52:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 15:52:56 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 15:52:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 15:52:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 15:53:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 15:53:43 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 15:53:44 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 15:53:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 15:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 15:53:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f051cb3f93e2fc8f84af88b5348bb4e5564efe268c7bf30737a51930020ce20`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acb76815f3acb8380fabd0b384e5d8c0d0d24b43377a5303e1a728ffc889603`  
		Last Modified: Thu, 23 Apr 2020 15:54:06 GMT  
		Size: 2.0 MB (2007835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7416e68338caa33a66862b706aedddf6ce8d0e1b1593bac60972037f31976cc3`  
		Last Modified: Thu, 23 Apr 2020 15:54:07 GMT  
		Size: 5.9 MB (5905365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa733ad101743b9ec1f6839e5d8a3023ddd3c33b3eee6d7add03090b2a1cab50`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e420b18a7c4198011cfe992ee33846c873b9d0cb0c213db9abca52fbd6882fc2`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:e4a9485e20d5d048b6b1f7b89b8c012eed0af7819453eaabc6d6f254fd3b2887
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41515322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb32c32f38391ef1bb90e62abfec04f364d3b96a7cc093263674e101a2211ccb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 13 May 2020 21:39:26 GMT
ADD file:e92e4e13785400e1d0cbdfd2b1d0454f6e9b4e5db46a134c637427c1d521f5c5 in / 
# Wed, 13 May 2020 21:39:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:37:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 May 2020 23:38:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 13 May 2020 23:38:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 23:38:36 GMT
VOLUME [/spiped]
# Wed, 13 May 2020 23:38:36 GMT
WORKDIR /spiped
# Wed, 13 May 2020 23:38:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 May 2020 23:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 23:38:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:719e323d8af1942809d715e86b7671949520675686dd460851d76bf569d8a8e8`  
		Last Modified: Wed, 13 May 2020 21:46:32 GMT  
		Size: 27.7 MB (27747747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38da04e97bff2b7382e32582c068544dee5a1de632d7fc6263bb18db2df7af50`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85cfbc7a9caa11fadf3be0536728b3b89282a6860e435b27de7fa25be018687`  
		Last Modified: Wed, 13 May 2020 23:38:53 GMT  
		Size: 2.1 MB (2132299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b7c42331a3b53440bb958a32d8da453a87611e2178fcee5f5ed041ee029963`  
		Last Modified: Wed, 13 May 2020 23:38:56 GMT  
		Size: 11.6 MB (11633113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265e206e7f823ced40fd63ad3a1f5134005b867816c0e6669914cc1eaaa70dcc`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db274ebdb4f9d75f7f051bd7509efb9a6d4d6408b69c7d0406e72a0dd5e989f9`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:f91e47bbc5d31233784f17f5565a334606257d7e9a8693464e19e161ccf0ad55
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33892434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f619d07812967c4818dcd6cd9c058089617c714dd36691b599dddf20c7e80ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:03:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 06:03:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 06:03:51 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 06:03:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 06:03:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 06:05:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 06:05:01 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 06:05:01 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 06:05:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 06:05:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51904ae673f6205aeb18b4941b0b86dd612faf95ba48129549fb43f070abf2e6`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8a20e087a159fd2aeb1c2b68b7a8006cd0a9d69141c635cbe7100d4cb72547`  
		Last Modified: Thu, 23 Apr 2020 06:05:23 GMT  
		Size: 1.7 MB (1711985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbc1f20c1494ea8864c22058f6f84349cf689cdc791257665d01c137a543425`  
		Last Modified: Thu, 23 Apr 2020 06:05:29 GMT  
		Size: 6.4 MB (6416148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab5a2be89807e61f976284ab0b61756a179cb137a417fcd3284114bb22b515c`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fea47f48a62a2012edff72d4d4c401e085a93313a868c4b8861d4b98e77fa`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:43ba6e1d2334c0b0ee8fd98afb19e079abc63411a14c01b25b3addf0c3110e0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9f9a3d1352e69d53f6a278af1cb1668efb34ebc28158019b7c4ab6b0839597`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 13 May 2020 22:22:26 GMT
ADD file:53bd5d792aec2fc8af7c0c836e64979e003b2cecaaf5153bd456cb4e97ba5a0e in / 
# Wed, 13 May 2020 22:22:29 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:57:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 14 May 2020 00:58:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:58:14 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 14 May 2020 00:58:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 14 May 2020 00:58:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 14 May 2020 01:00:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 01:00:45 GMT
VOLUME [/spiped]
# Thu, 14 May 2020 01:00:51 GMT
WORKDIR /spiped
# Thu, 14 May 2020 01:00:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 14 May 2020 01:00:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 May 2020 01:00:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d23cb84f4d6399958c00ec4c457e9c302763ee7dd86a0fb5540f75ed550c17d6`  
		Last Modified: Wed, 13 May 2020 22:57:57 GMT  
		Size: 30.5 MB (30518701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca31312f1462a6de31b476e94f6ece01e96455fe8f8eb974acce547ef0006f`  
		Last Modified: Thu, 14 May 2020 01:01:25 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3471ced55a9c2947633a2046ac7a5f0ead06bf46c2c81f45cab3dd31ba7a9c`  
		Last Modified: Thu, 14 May 2020 01:01:27 GMT  
		Size: 2.2 MB (2224901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c049f05b45f5d83517a4fb7769b63aa007b82079c781b807beba0f74a34f2e37`  
		Last Modified: Thu, 14 May 2020 01:01:28 GMT  
		Size: 6.7 MB (6743174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af6e997510cefe731b7be15a92cd32eaf3f4b1862245080e0006810afaf80fc`  
		Last Modified: Thu, 14 May 2020 01:01:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d5b799c722c59bb1f55029f89256dbf8bf6f096e8e385459f386443d30af82`  
		Last Modified: Thu, 14 May 2020 01:01:26 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:d3b02a6f55588ee0b48e8381c875b1ebc582355f9ffcf31d4dcd4b407e89c5c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33480257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0d3eec114f0cb239d32dd4184656b9444d938a93d8dd413a994fadc8599f9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 14 May 2020 23:06:40 GMT
ADD file:a29e647b8dccf726d8610d8c599d6727d6145426f9374720b985fc9be9ac906c in / 
# Thu, 14 May 2020 23:06:41 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:39:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 03:39:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:39:24 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 03:39:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 03:39:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 03:39:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 03:39:40 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 03:39:41 GMT
WORKDIR /spiped
# Fri, 15 May 2020 03:39:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 03:39:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 03:39:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bdb298e230dde60bfce8a476ae8ea8988828f7ec9f5452f38f46102a609f57c1`  
		Last Modified: Thu, 14 May 2020 23:11:24 GMT  
		Size: 25.7 MB (25712933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef6fad20a12a37bf7ec2b3456d4cbda8584c39eb46e868d23d4ba1e0895aa6f`  
		Last Modified: Fri, 15 May 2020 03:40:00 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c387fca3d488181c18a26861d4c4ed0a06f37a3881847cb6dd2c7c4dfcfb78`  
		Last Modified: Fri, 15 May 2020 03:40:00 GMT  
		Size: 1.8 MB (1821765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828e45a1d42bba03691a76d62c88b01dec85bc970ab3904a96a1797db70f0752`  
		Last Modified: Fri, 15 May 2020 03:40:06 GMT  
		Size: 5.9 MB (5943352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1f48db4b32e85e463e04a88b629867f14f89c34c70003f91c14e7895d9fbaf`  
		Last Modified: Fri, 15 May 2020 03:40:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d995a72a4d343ecc1a86679843eacb30b33f0bd51fb81ed61cd74d75593098e`  
		Last Modified: Fri, 15 May 2020 03:40:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:0974779f94eefdaceee919a3fa3a13f276c511df256f137122f6c92321ba1ec1
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
$ docker pull spiped@sha256:7210ee044384bbf33b10cb67ac7553d668f7153c33d585d44f0f094802211935
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36265955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe93473ad7fbf7cfe45ec029c8e6ecceb7d566ee348606465258b48d44fb7a74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 20:03:27 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 20:03:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 20:03:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 20:03:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 20:03:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 20:04:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 20:04:04 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 20:04:04 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 20:04:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 20:04:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 20:04:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eddd5e303f5c1f7165d495e17bddc0f2de7f6a442bed4aa5ac459a6ac611b1c`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1abc5f67f536b64df626692b5282ca4c22723857a6aeac95cd33d3f4e308953`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 2.1 MB (2128047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ea5550680d87a6bc6b46386fee970f0570d3f04daaa7bae1d430dc370df4e`  
		Last Modified: Thu, 23 Apr 2020 20:04:25 GMT  
		Size: 7.0 MB (7037480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011c1a0f8d8f204ab1ffc14fbf98193e3b50980b4eb88e30498b32aba5327dc2`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ce919881dee3bbed53f0207ca6833b9a955ea08c97e3556207898ed438b880`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:684ff0c8dfb3841271f5206b43eb09bf67b7ce4ed227991695b458ef2c433378
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32159776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58bbf4cfd7f41654132e8864655fe8c89653e455477752eca0c0f8f6fefb701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:17:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 03:17:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:17:30 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 03:17:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 03:17:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 03:18:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 03:18:40 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 03:18:41 GMT
WORKDIR /spiped
# Fri, 15 May 2020 03:18:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 03:18:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 03:18:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b0bb0a243296a03a7eb3d5685e105963e7740f828fe89200768b8b03d8c145`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355ea8b47d3eb64e79c3ff6b960d39905709329fc410b679ed67fb6a046e11b6`  
		Last Modified: Fri, 15 May 2020 03:19:08 GMT  
		Size: 1.8 MB (1839134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508622f07ba3c6a59ea9a8bafcc356fe7a02e3cef578e40fc352ddc9936f49e6`  
		Last Modified: Fri, 15 May 2020 03:19:10 GMT  
		Size: 5.5 MB (5479971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f8b3d25b951be8ffd5d1b88cdd703030efd6b6e389fa2fbb55bb0897b9d88c`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf14b5beaa983bb77e805228142604932caf4aedd9c3056e4e4a369791d06f1b`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:87e594e6c297ab32b63899e657c1a54a8d1100d3b615aba3110b9c83af034bf4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3762d7fbd521ea9dd741d0c9728f84de283ec800689749f6154163ac375146ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:37:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 06:37:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 06:37:12 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 06:37:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 06:37:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 06:38:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 06:38:07 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 06:38:07 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 06:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 06:38:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c245760c54fc8d94586399ec9055355e4c3366a9bbb2fa8adfc6f906feb4be2e`  
		Last Modified: Thu, 23 Apr 2020 06:38:30 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e881f703761ee378af97245f067193b18a2e259c6960350af6bd58c50c17c9`  
		Last Modified: Thu, 23 Apr 2020 06:38:31 GMT  
		Size: 1.8 MB (1759439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff85ebb091bd4c189eb2fbb13813d47c9bb4a87981d5e5e7f024ba3a70413717`  
		Last Modified: Thu, 23 Apr 2020 06:38:33 GMT  
		Size: 5.3 MB (5285357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe372689bc3dcd9f9fcc3170419cbe8cdf8289b8ab46d6658e6f9afdb311b92`  
		Last Modified: Thu, 23 Apr 2020 06:38:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a07c2d12354b78115b49045a435919c09508a793f325a501637f134f608c3`  
		Last Modified: Thu, 23 Apr 2020 06:38:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:3c11c283fe0418525bef456d87e13fb1eda7daa8405bd41f740174fa8f17ba86
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99399f5684ebefda91f2d63ec0d8e8ea2262734018b10b7294427a56aa48bbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 15:52:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 15:52:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 15:52:56 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 15:52:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 15:52:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 15:53:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 15:53:43 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 15:53:44 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 15:53:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 15:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 15:53:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f051cb3f93e2fc8f84af88b5348bb4e5564efe268c7bf30737a51930020ce20`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acb76815f3acb8380fabd0b384e5d8c0d0d24b43377a5303e1a728ffc889603`  
		Last Modified: Thu, 23 Apr 2020 15:54:06 GMT  
		Size: 2.0 MB (2007835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7416e68338caa33a66862b706aedddf6ce8d0e1b1593bac60972037f31976cc3`  
		Last Modified: Thu, 23 Apr 2020 15:54:07 GMT  
		Size: 5.9 MB (5905365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa733ad101743b9ec1f6839e5d8a3023ddd3c33b3eee6d7add03090b2a1cab50`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e420b18a7c4198011cfe992ee33846c873b9d0cb0c213db9abca52fbd6882fc2`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:e4a9485e20d5d048b6b1f7b89b8c012eed0af7819453eaabc6d6f254fd3b2887
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41515322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb32c32f38391ef1bb90e62abfec04f364d3b96a7cc093263674e101a2211ccb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 13 May 2020 21:39:26 GMT
ADD file:e92e4e13785400e1d0cbdfd2b1d0454f6e9b4e5db46a134c637427c1d521f5c5 in / 
# Wed, 13 May 2020 21:39:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:37:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 May 2020 23:38:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 13 May 2020 23:38:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 23:38:36 GMT
VOLUME [/spiped]
# Wed, 13 May 2020 23:38:36 GMT
WORKDIR /spiped
# Wed, 13 May 2020 23:38:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 May 2020 23:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 23:38:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:719e323d8af1942809d715e86b7671949520675686dd460851d76bf569d8a8e8`  
		Last Modified: Wed, 13 May 2020 21:46:32 GMT  
		Size: 27.7 MB (27747747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38da04e97bff2b7382e32582c068544dee5a1de632d7fc6263bb18db2df7af50`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85cfbc7a9caa11fadf3be0536728b3b89282a6860e435b27de7fa25be018687`  
		Last Modified: Wed, 13 May 2020 23:38:53 GMT  
		Size: 2.1 MB (2132299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b7c42331a3b53440bb958a32d8da453a87611e2178fcee5f5ed041ee029963`  
		Last Modified: Wed, 13 May 2020 23:38:56 GMT  
		Size: 11.6 MB (11633113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265e206e7f823ced40fd63ad3a1f5134005b867816c0e6669914cc1eaaa70dcc`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db274ebdb4f9d75f7f051bd7509efb9a6d4d6408b69c7d0406e72a0dd5e989f9`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:f91e47bbc5d31233784f17f5565a334606257d7e9a8693464e19e161ccf0ad55
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33892434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f619d07812967c4818dcd6cd9c058089617c714dd36691b599dddf20c7e80ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:03:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 06:03:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 06:03:51 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 06:03:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 06:03:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 06:05:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 06:05:01 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 06:05:01 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 06:05:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 06:05:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51904ae673f6205aeb18b4941b0b86dd612faf95ba48129549fb43f070abf2e6`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8a20e087a159fd2aeb1c2b68b7a8006cd0a9d69141c635cbe7100d4cb72547`  
		Last Modified: Thu, 23 Apr 2020 06:05:23 GMT  
		Size: 1.7 MB (1711985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbc1f20c1494ea8864c22058f6f84349cf689cdc791257665d01c137a543425`  
		Last Modified: Thu, 23 Apr 2020 06:05:29 GMT  
		Size: 6.4 MB (6416148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab5a2be89807e61f976284ab0b61756a179cb137a417fcd3284114bb22b515c`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fea47f48a62a2012edff72d4d4c401e085a93313a868c4b8861d4b98e77fa`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:43ba6e1d2334c0b0ee8fd98afb19e079abc63411a14c01b25b3addf0c3110e0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9f9a3d1352e69d53f6a278af1cb1668efb34ebc28158019b7c4ab6b0839597`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 13 May 2020 22:22:26 GMT
ADD file:53bd5d792aec2fc8af7c0c836e64979e003b2cecaaf5153bd456cb4e97ba5a0e in / 
# Wed, 13 May 2020 22:22:29 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:57:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 14 May 2020 00:58:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:58:14 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 14 May 2020 00:58:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 14 May 2020 00:58:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 14 May 2020 01:00:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 01:00:45 GMT
VOLUME [/spiped]
# Thu, 14 May 2020 01:00:51 GMT
WORKDIR /spiped
# Thu, 14 May 2020 01:00:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 14 May 2020 01:00:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 May 2020 01:00:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d23cb84f4d6399958c00ec4c457e9c302763ee7dd86a0fb5540f75ed550c17d6`  
		Last Modified: Wed, 13 May 2020 22:57:57 GMT  
		Size: 30.5 MB (30518701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca31312f1462a6de31b476e94f6ece01e96455fe8f8eb974acce547ef0006f`  
		Last Modified: Thu, 14 May 2020 01:01:25 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3471ced55a9c2947633a2046ac7a5f0ead06bf46c2c81f45cab3dd31ba7a9c`  
		Last Modified: Thu, 14 May 2020 01:01:27 GMT  
		Size: 2.2 MB (2224901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c049f05b45f5d83517a4fb7769b63aa007b82079c781b807beba0f74a34f2e37`  
		Last Modified: Thu, 14 May 2020 01:01:28 GMT  
		Size: 6.7 MB (6743174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af6e997510cefe731b7be15a92cd32eaf3f4b1862245080e0006810afaf80fc`  
		Last Modified: Thu, 14 May 2020 01:01:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d5b799c722c59bb1f55029f89256dbf8bf6f096e8e385459f386443d30af82`  
		Last Modified: Thu, 14 May 2020 01:01:26 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:d3b02a6f55588ee0b48e8381c875b1ebc582355f9ffcf31d4dcd4b407e89c5c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33480257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0d3eec114f0cb239d32dd4184656b9444d938a93d8dd413a994fadc8599f9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 14 May 2020 23:06:40 GMT
ADD file:a29e647b8dccf726d8610d8c599d6727d6145426f9374720b985fc9be9ac906c in / 
# Thu, 14 May 2020 23:06:41 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:39:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 03:39:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:39:24 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 03:39:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 03:39:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 03:39:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 03:39:40 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 03:39:41 GMT
WORKDIR /spiped
# Fri, 15 May 2020 03:39:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 03:39:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 03:39:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bdb298e230dde60bfce8a476ae8ea8988828f7ec9f5452f38f46102a609f57c1`  
		Last Modified: Thu, 14 May 2020 23:11:24 GMT  
		Size: 25.7 MB (25712933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef6fad20a12a37bf7ec2b3456d4cbda8584c39eb46e868d23d4ba1e0895aa6f`  
		Last Modified: Fri, 15 May 2020 03:40:00 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c387fca3d488181c18a26861d4c4ed0a06f37a3881847cb6dd2c7c4dfcfb78`  
		Last Modified: Fri, 15 May 2020 03:40:00 GMT  
		Size: 1.8 MB (1821765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828e45a1d42bba03691a76d62c88b01dec85bc970ab3904a96a1797db70f0752`  
		Last Modified: Fri, 15 May 2020 03:40:06 GMT  
		Size: 5.9 MB (5943352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1f48db4b32e85e463e04a88b629867f14f89c34c70003f91c14e7895d9fbaf`  
		Last Modified: Fri, 15 May 2020 03:40:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d995a72a4d343ecc1a86679843eacb30b33f0bd51fb81ed61cd74d75593098e`  
		Last Modified: Fri, 15 May 2020 03:40:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:0974779f94eefdaceee919a3fa3a13f276c511df256f137122f6c92321ba1ec1
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
$ docker pull spiped@sha256:7210ee044384bbf33b10cb67ac7553d668f7153c33d585d44f0f094802211935
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36265955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe93473ad7fbf7cfe45ec029c8e6ecceb7d566ee348606465258b48d44fb7a74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 20:03:27 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 20:03:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 20:03:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 20:03:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 20:03:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 20:04:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 20:04:04 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 20:04:04 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 20:04:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 20:04:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 20:04:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eddd5e303f5c1f7165d495e17bddc0f2de7f6a442bed4aa5ac459a6ac611b1c`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1abc5f67f536b64df626692b5282ca4c22723857a6aeac95cd33d3f4e308953`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 2.1 MB (2128047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ea5550680d87a6bc6b46386fee970f0570d3f04daaa7bae1d430dc370df4e`  
		Last Modified: Thu, 23 Apr 2020 20:04:25 GMT  
		Size: 7.0 MB (7037480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011c1a0f8d8f204ab1ffc14fbf98193e3b50980b4eb88e30498b32aba5327dc2`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ce919881dee3bbed53f0207ca6833b9a955ea08c97e3556207898ed438b880`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:684ff0c8dfb3841271f5206b43eb09bf67b7ce4ed227991695b458ef2c433378
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32159776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58bbf4cfd7f41654132e8864655fe8c89653e455477752eca0c0f8f6fefb701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:17:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 03:17:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:17:30 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 03:17:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 03:17:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 03:18:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 03:18:40 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 03:18:41 GMT
WORKDIR /spiped
# Fri, 15 May 2020 03:18:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 03:18:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 03:18:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b0bb0a243296a03a7eb3d5685e105963e7740f828fe89200768b8b03d8c145`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355ea8b47d3eb64e79c3ff6b960d39905709329fc410b679ed67fb6a046e11b6`  
		Last Modified: Fri, 15 May 2020 03:19:08 GMT  
		Size: 1.8 MB (1839134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508622f07ba3c6a59ea9a8bafcc356fe7a02e3cef578e40fc352ddc9936f49e6`  
		Last Modified: Fri, 15 May 2020 03:19:10 GMT  
		Size: 5.5 MB (5479971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f8b3d25b951be8ffd5d1b88cdd703030efd6b6e389fa2fbb55bb0897b9d88c`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf14b5beaa983bb77e805228142604932caf4aedd9c3056e4e4a369791d06f1b`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:87e594e6c297ab32b63899e657c1a54a8d1100d3b615aba3110b9c83af034bf4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3762d7fbd521ea9dd741d0c9728f84de283ec800689749f6154163ac375146ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:37:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 06:37:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 06:37:12 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 06:37:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 06:37:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 06:38:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 06:38:07 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 06:38:07 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 06:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 06:38:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c245760c54fc8d94586399ec9055355e4c3366a9bbb2fa8adfc6f906feb4be2e`  
		Last Modified: Thu, 23 Apr 2020 06:38:30 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e881f703761ee378af97245f067193b18a2e259c6960350af6bd58c50c17c9`  
		Last Modified: Thu, 23 Apr 2020 06:38:31 GMT  
		Size: 1.8 MB (1759439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff85ebb091bd4c189eb2fbb13813d47c9bb4a87981d5e5e7f024ba3a70413717`  
		Last Modified: Thu, 23 Apr 2020 06:38:33 GMT  
		Size: 5.3 MB (5285357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe372689bc3dcd9f9fcc3170419cbe8cdf8289b8ab46d6658e6f9afdb311b92`  
		Last Modified: Thu, 23 Apr 2020 06:38:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a07c2d12354b78115b49045a435919c09508a793f325a501637f134f608c3`  
		Last Modified: Thu, 23 Apr 2020 06:38:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:3c11c283fe0418525bef456d87e13fb1eda7daa8405bd41f740174fa8f17ba86
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99399f5684ebefda91f2d63ec0d8e8ea2262734018b10b7294427a56aa48bbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 15:52:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 15:52:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 15:52:56 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 15:52:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 15:52:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 15:53:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 15:53:43 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 15:53:44 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 15:53:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 15:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 15:53:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f051cb3f93e2fc8f84af88b5348bb4e5564efe268c7bf30737a51930020ce20`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acb76815f3acb8380fabd0b384e5d8c0d0d24b43377a5303e1a728ffc889603`  
		Last Modified: Thu, 23 Apr 2020 15:54:06 GMT  
		Size: 2.0 MB (2007835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7416e68338caa33a66862b706aedddf6ce8d0e1b1593bac60972037f31976cc3`  
		Last Modified: Thu, 23 Apr 2020 15:54:07 GMT  
		Size: 5.9 MB (5905365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa733ad101743b9ec1f6839e5d8a3023ddd3c33b3eee6d7add03090b2a1cab50`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e420b18a7c4198011cfe992ee33846c873b9d0cb0c213db9abca52fbd6882fc2`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:e4a9485e20d5d048b6b1f7b89b8c012eed0af7819453eaabc6d6f254fd3b2887
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41515322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb32c32f38391ef1bb90e62abfec04f364d3b96a7cc093263674e101a2211ccb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 13 May 2020 21:39:26 GMT
ADD file:e92e4e13785400e1d0cbdfd2b1d0454f6e9b4e5db46a134c637427c1d521f5c5 in / 
# Wed, 13 May 2020 21:39:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:37:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 May 2020 23:38:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 13 May 2020 23:38:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 23:38:36 GMT
VOLUME [/spiped]
# Wed, 13 May 2020 23:38:36 GMT
WORKDIR /spiped
# Wed, 13 May 2020 23:38:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 May 2020 23:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 23:38:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:719e323d8af1942809d715e86b7671949520675686dd460851d76bf569d8a8e8`  
		Last Modified: Wed, 13 May 2020 21:46:32 GMT  
		Size: 27.7 MB (27747747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38da04e97bff2b7382e32582c068544dee5a1de632d7fc6263bb18db2df7af50`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85cfbc7a9caa11fadf3be0536728b3b89282a6860e435b27de7fa25be018687`  
		Last Modified: Wed, 13 May 2020 23:38:53 GMT  
		Size: 2.1 MB (2132299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b7c42331a3b53440bb958a32d8da453a87611e2178fcee5f5ed041ee029963`  
		Last Modified: Wed, 13 May 2020 23:38:56 GMT  
		Size: 11.6 MB (11633113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265e206e7f823ced40fd63ad3a1f5134005b867816c0e6669914cc1eaaa70dcc`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db274ebdb4f9d75f7f051bd7509efb9a6d4d6408b69c7d0406e72a0dd5e989f9`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:f91e47bbc5d31233784f17f5565a334606257d7e9a8693464e19e161ccf0ad55
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33892434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f619d07812967c4818dcd6cd9c058089617c714dd36691b599dddf20c7e80ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:03:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 06:03:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 06:03:51 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 06:03:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 06:03:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 06:05:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 06:05:01 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 06:05:01 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 06:05:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 06:05:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51904ae673f6205aeb18b4941b0b86dd612faf95ba48129549fb43f070abf2e6`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8a20e087a159fd2aeb1c2b68b7a8006cd0a9d69141c635cbe7100d4cb72547`  
		Last Modified: Thu, 23 Apr 2020 06:05:23 GMT  
		Size: 1.7 MB (1711985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbc1f20c1494ea8864c22058f6f84349cf689cdc791257665d01c137a543425`  
		Last Modified: Thu, 23 Apr 2020 06:05:29 GMT  
		Size: 6.4 MB (6416148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab5a2be89807e61f976284ab0b61756a179cb137a417fcd3284114bb22b515c`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fea47f48a62a2012edff72d4d4c401e085a93313a868c4b8861d4b98e77fa`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:43ba6e1d2334c0b0ee8fd98afb19e079abc63411a14c01b25b3addf0c3110e0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9f9a3d1352e69d53f6a278af1cb1668efb34ebc28158019b7c4ab6b0839597`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 13 May 2020 22:22:26 GMT
ADD file:53bd5d792aec2fc8af7c0c836e64979e003b2cecaaf5153bd456cb4e97ba5a0e in / 
# Wed, 13 May 2020 22:22:29 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:57:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 14 May 2020 00:58:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:58:14 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 14 May 2020 00:58:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 14 May 2020 00:58:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 14 May 2020 01:00:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 01:00:45 GMT
VOLUME [/spiped]
# Thu, 14 May 2020 01:00:51 GMT
WORKDIR /spiped
# Thu, 14 May 2020 01:00:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 14 May 2020 01:00:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 May 2020 01:00:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d23cb84f4d6399958c00ec4c457e9c302763ee7dd86a0fb5540f75ed550c17d6`  
		Last Modified: Wed, 13 May 2020 22:57:57 GMT  
		Size: 30.5 MB (30518701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca31312f1462a6de31b476e94f6ece01e96455fe8f8eb974acce547ef0006f`  
		Last Modified: Thu, 14 May 2020 01:01:25 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3471ced55a9c2947633a2046ac7a5f0ead06bf46c2c81f45cab3dd31ba7a9c`  
		Last Modified: Thu, 14 May 2020 01:01:27 GMT  
		Size: 2.2 MB (2224901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c049f05b45f5d83517a4fb7769b63aa007b82079c781b807beba0f74a34f2e37`  
		Last Modified: Thu, 14 May 2020 01:01:28 GMT  
		Size: 6.7 MB (6743174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af6e997510cefe731b7be15a92cd32eaf3f4b1862245080e0006810afaf80fc`  
		Last Modified: Thu, 14 May 2020 01:01:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d5b799c722c59bb1f55029f89256dbf8bf6f096e8e385459f386443d30af82`  
		Last Modified: Thu, 14 May 2020 01:01:26 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:d3b02a6f55588ee0b48e8381c875b1ebc582355f9ffcf31d4dcd4b407e89c5c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33480257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0d3eec114f0cb239d32dd4184656b9444d938a93d8dd413a994fadc8599f9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 14 May 2020 23:06:40 GMT
ADD file:a29e647b8dccf726d8610d8c599d6727d6145426f9374720b985fc9be9ac906c in / 
# Thu, 14 May 2020 23:06:41 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:39:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 03:39:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:39:24 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 03:39:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 03:39:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 03:39:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 03:39:40 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 03:39:41 GMT
WORKDIR /spiped
# Fri, 15 May 2020 03:39:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 03:39:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 03:39:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bdb298e230dde60bfce8a476ae8ea8988828f7ec9f5452f38f46102a609f57c1`  
		Last Modified: Thu, 14 May 2020 23:11:24 GMT  
		Size: 25.7 MB (25712933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef6fad20a12a37bf7ec2b3456d4cbda8584c39eb46e868d23d4ba1e0895aa6f`  
		Last Modified: Fri, 15 May 2020 03:40:00 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c387fca3d488181c18a26861d4c4ed0a06f37a3881847cb6dd2c7c4dfcfb78`  
		Last Modified: Fri, 15 May 2020 03:40:00 GMT  
		Size: 1.8 MB (1821765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828e45a1d42bba03691a76d62c88b01dec85bc970ab3904a96a1797db70f0752`  
		Last Modified: Fri, 15 May 2020 03:40:06 GMT  
		Size: 5.9 MB (5943352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1f48db4b32e85e463e04a88b629867f14f89c34c70003f91c14e7895d9fbaf`  
		Last Modified: Fri, 15 May 2020 03:40:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d995a72a4d343ecc1a86679843eacb30b33f0bd51fb81ed61cd74d75593098e`  
		Last Modified: Fri, 15 May 2020 03:40:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:0974779f94eefdaceee919a3fa3a13f276c511df256f137122f6c92321ba1ec1
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
$ docker pull spiped@sha256:7210ee044384bbf33b10cb67ac7553d668f7153c33d585d44f0f094802211935
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36265955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe93473ad7fbf7cfe45ec029c8e6ecceb7d566ee348606465258b48d44fb7a74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 20:03:27 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 20:03:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 20:03:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 20:03:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 20:03:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 20:04:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 20:04:04 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 20:04:04 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 20:04:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 20:04:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 20:04:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eddd5e303f5c1f7165d495e17bddc0f2de7f6a442bed4aa5ac459a6ac611b1c`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1abc5f67f536b64df626692b5282ca4c22723857a6aeac95cd33d3f4e308953`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 2.1 MB (2128047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ea5550680d87a6bc6b46386fee970f0570d3f04daaa7bae1d430dc370df4e`  
		Last Modified: Thu, 23 Apr 2020 20:04:25 GMT  
		Size: 7.0 MB (7037480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011c1a0f8d8f204ab1ffc14fbf98193e3b50980b4eb88e30498b32aba5327dc2`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ce919881dee3bbed53f0207ca6833b9a955ea08c97e3556207898ed438b880`  
		Last Modified: Thu, 23 Apr 2020 20:04:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:684ff0c8dfb3841271f5206b43eb09bf67b7ce4ed227991695b458ef2c433378
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32159776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58bbf4cfd7f41654132e8864655fe8c89653e455477752eca0c0f8f6fefb701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:17:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 03:17:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:17:30 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 03:17:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 03:17:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 03:18:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 03:18:40 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 03:18:41 GMT
WORKDIR /spiped
# Fri, 15 May 2020 03:18:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 03:18:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 03:18:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b0bb0a243296a03a7eb3d5685e105963e7740f828fe89200768b8b03d8c145`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355ea8b47d3eb64e79c3ff6b960d39905709329fc410b679ed67fb6a046e11b6`  
		Last Modified: Fri, 15 May 2020 03:19:08 GMT  
		Size: 1.8 MB (1839134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508622f07ba3c6a59ea9a8bafcc356fe7a02e3cef578e40fc352ddc9936f49e6`  
		Last Modified: Fri, 15 May 2020 03:19:10 GMT  
		Size: 5.5 MB (5479971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f8b3d25b951be8ffd5d1b88cdd703030efd6b6e389fa2fbb55bb0897b9d88c`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf14b5beaa983bb77e805228142604932caf4aedd9c3056e4e4a369791d06f1b`  
		Last Modified: Fri, 15 May 2020 03:19:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:87e594e6c297ab32b63899e657c1a54a8d1100d3b615aba3110b9c83af034bf4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3762d7fbd521ea9dd741d0c9728f84de283ec800689749f6154163ac375146ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:37:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 06:37:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 06:37:12 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 06:37:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 06:37:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 06:38:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 06:38:07 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 06:38:07 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 06:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 06:38:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c245760c54fc8d94586399ec9055355e4c3366a9bbb2fa8adfc6f906feb4be2e`  
		Last Modified: Thu, 23 Apr 2020 06:38:30 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e881f703761ee378af97245f067193b18a2e259c6960350af6bd58c50c17c9`  
		Last Modified: Thu, 23 Apr 2020 06:38:31 GMT  
		Size: 1.8 MB (1759439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff85ebb091bd4c189eb2fbb13813d47c9bb4a87981d5e5e7f024ba3a70413717`  
		Last Modified: Thu, 23 Apr 2020 06:38:33 GMT  
		Size: 5.3 MB (5285357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe372689bc3dcd9f9fcc3170419cbe8cdf8289b8ab46d6658e6f9afdb311b92`  
		Last Modified: Thu, 23 Apr 2020 06:38:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a07c2d12354b78115b49045a435919c09508a793f325a501637f134f608c3`  
		Last Modified: Thu, 23 Apr 2020 06:38:30 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:3c11c283fe0418525bef456d87e13fb1eda7daa8405bd41f740174fa8f17ba86
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99399f5684ebefda91f2d63ec0d8e8ea2262734018b10b7294427a56aa48bbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 15:52:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 15:52:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 15:52:56 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 15:52:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 15:52:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 15:53:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 15:53:43 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 15:53:44 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 15:53:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 15:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 15:53:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f051cb3f93e2fc8f84af88b5348bb4e5564efe268c7bf30737a51930020ce20`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acb76815f3acb8380fabd0b384e5d8c0d0d24b43377a5303e1a728ffc889603`  
		Last Modified: Thu, 23 Apr 2020 15:54:06 GMT  
		Size: 2.0 MB (2007835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7416e68338caa33a66862b706aedddf6ce8d0e1b1593bac60972037f31976cc3`  
		Last Modified: Thu, 23 Apr 2020 15:54:07 GMT  
		Size: 5.9 MB (5905365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa733ad101743b9ec1f6839e5d8a3023ddd3c33b3eee6d7add03090b2a1cab50`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e420b18a7c4198011cfe992ee33846c873b9d0cb0c213db9abca52fbd6882fc2`  
		Last Modified: Thu, 23 Apr 2020 15:54:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:e4a9485e20d5d048b6b1f7b89b8c012eed0af7819453eaabc6d6f254fd3b2887
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41515322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb32c32f38391ef1bb90e62abfec04f364d3b96a7cc093263674e101a2211ccb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 13 May 2020 21:39:26 GMT
ADD file:e92e4e13785400e1d0cbdfd2b1d0454f6e9b4e5db46a134c637427c1d521f5c5 in / 
# Wed, 13 May 2020 21:39:26 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:37:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 May 2020 23:38:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 13 May 2020 23:38:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 13 May 2020 23:38:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 May 2020 23:38:36 GMT
VOLUME [/spiped]
# Wed, 13 May 2020 23:38:36 GMT
WORKDIR /spiped
# Wed, 13 May 2020 23:38:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 May 2020 23:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 23:38:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:719e323d8af1942809d715e86b7671949520675686dd460851d76bf569d8a8e8`  
		Last Modified: Wed, 13 May 2020 21:46:32 GMT  
		Size: 27.7 MB (27747747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38da04e97bff2b7382e32582c068544dee5a1de632d7fc6263bb18db2df7af50`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85cfbc7a9caa11fadf3be0536728b3b89282a6860e435b27de7fa25be018687`  
		Last Modified: Wed, 13 May 2020 23:38:53 GMT  
		Size: 2.1 MB (2132299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b7c42331a3b53440bb958a32d8da453a87611e2178fcee5f5ed041ee029963`  
		Last Modified: Wed, 13 May 2020 23:38:56 GMT  
		Size: 11.6 MB (11633113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265e206e7f823ced40fd63ad3a1f5134005b867816c0e6669914cc1eaaa70dcc`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db274ebdb4f9d75f7f051bd7509efb9a6d4d6408b69c7d0406e72a0dd5e989f9`  
		Last Modified: Wed, 13 May 2020 23:38:52 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:f91e47bbc5d31233784f17f5565a334606257d7e9a8693464e19e161ccf0ad55
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33892434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f619d07812967c4818dcd6cd9c058089617c714dd36691b599dddf20c7e80ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:03:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 06:03:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 06:03:51 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 06:03:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 06:03:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 06:05:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 06:05:01 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 06:05:01 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 06:05:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 06:05:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51904ae673f6205aeb18b4941b0b86dd612faf95ba48129549fb43f070abf2e6`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8a20e087a159fd2aeb1c2b68b7a8006cd0a9d69141c635cbe7100d4cb72547`  
		Last Modified: Thu, 23 Apr 2020 06:05:23 GMT  
		Size: 1.7 MB (1711985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbc1f20c1494ea8864c22058f6f84349cf689cdc791257665d01c137a543425`  
		Last Modified: Thu, 23 Apr 2020 06:05:29 GMT  
		Size: 6.4 MB (6416148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab5a2be89807e61f976284ab0b61756a179cb137a417fcd3284114bb22b515c`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fea47f48a62a2012edff72d4d4c401e085a93313a868c4b8861d4b98e77fa`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:43ba6e1d2334c0b0ee8fd98afb19e079abc63411a14c01b25b3addf0c3110e0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9f9a3d1352e69d53f6a278af1cb1668efb34ebc28158019b7c4ab6b0839597`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 13 May 2020 22:22:26 GMT
ADD file:53bd5d792aec2fc8af7c0c836e64979e003b2cecaaf5153bd456cb4e97ba5a0e in / 
# Wed, 13 May 2020 22:22:29 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:57:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 14 May 2020 00:58:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:58:14 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 14 May 2020 00:58:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 14 May 2020 00:58:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 14 May 2020 01:00:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 14 May 2020 01:00:45 GMT
VOLUME [/spiped]
# Thu, 14 May 2020 01:00:51 GMT
WORKDIR /spiped
# Thu, 14 May 2020 01:00:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 14 May 2020 01:00:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 May 2020 01:00:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d23cb84f4d6399958c00ec4c457e9c302763ee7dd86a0fb5540f75ed550c17d6`  
		Last Modified: Wed, 13 May 2020 22:57:57 GMT  
		Size: 30.5 MB (30518701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca31312f1462a6de31b476e94f6ece01e96455fe8f8eb974acce547ef0006f`  
		Last Modified: Thu, 14 May 2020 01:01:25 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3471ced55a9c2947633a2046ac7a5f0ead06bf46c2c81f45cab3dd31ba7a9c`  
		Last Modified: Thu, 14 May 2020 01:01:27 GMT  
		Size: 2.2 MB (2224901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c049f05b45f5d83517a4fb7769b63aa007b82079c781b807beba0f74a34f2e37`  
		Last Modified: Thu, 14 May 2020 01:01:28 GMT  
		Size: 6.7 MB (6743174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af6e997510cefe731b7be15a92cd32eaf3f4b1862245080e0006810afaf80fc`  
		Last Modified: Thu, 14 May 2020 01:01:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d5b799c722c59bb1f55029f89256dbf8bf6f096e8e385459f386443d30af82`  
		Last Modified: Thu, 14 May 2020 01:01:26 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:d3b02a6f55588ee0b48e8381c875b1ebc582355f9ffcf31d4dcd4b407e89c5c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33480257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0d3eec114f0cb239d32dd4184656b9444d938a93d8dd413a994fadc8599f9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 14 May 2020 23:06:40 GMT
ADD file:a29e647b8dccf726d8610d8c599d6727d6145426f9374720b985fc9be9ac906c in / 
# Thu, 14 May 2020 23:06:41 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:39:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 03:39:24 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:39:24 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 03:39:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 03:39:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 03:39:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 03:39:40 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 03:39:41 GMT
WORKDIR /spiped
# Fri, 15 May 2020 03:39:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 03:39:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 03:39:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bdb298e230dde60bfce8a476ae8ea8988828f7ec9f5452f38f46102a609f57c1`  
		Last Modified: Thu, 14 May 2020 23:11:24 GMT  
		Size: 25.7 MB (25712933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef6fad20a12a37bf7ec2b3456d4cbda8584c39eb46e868d23d4ba1e0895aa6f`  
		Last Modified: Fri, 15 May 2020 03:40:00 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c387fca3d488181c18a26861d4c4ed0a06f37a3881847cb6dd2c7c4dfcfb78`  
		Last Modified: Fri, 15 May 2020 03:40:00 GMT  
		Size: 1.8 MB (1821765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828e45a1d42bba03691a76d62c88b01dec85bc970ab3904a96a1797db70f0752`  
		Last Modified: Fri, 15 May 2020 03:40:06 GMT  
		Size: 5.9 MB (5943352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1f48db4b32e85e463e04a88b629867f14f89c34c70003f91c14e7895d9fbaf`  
		Last Modified: Fri, 15 May 2020 03:40:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d995a72a4d343ecc1a86679843eacb30b33f0bd51fb81ed61cd74d75593098e`  
		Last Modified: Fri, 15 May 2020 03:40:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
