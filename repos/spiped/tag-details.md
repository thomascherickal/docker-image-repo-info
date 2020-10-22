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
$ docker pull spiped@sha256:6be7b82d1d47a84533f91062e33a9fd4312f88a2a99c992321376fe725fc6211
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
$ docker pull spiped@sha256:cbcdcae2145e7f1c5b4c4e2ec9926e8f7cf2741c2edd41e74eb1a5ca85431c6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a3a8321db5126e2cfa970d9cabeafcbc493ae611c56ac1b7f3bc9c1877287`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:36:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:36:35 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:37:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:37:06 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:37:06 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:37:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7e552308a9a7e56787eb8f2ee2cd0e5ae1bcd3e6e70767a3f1f63d04df1043`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae3cfef5f840d90ca6a31c452db1ff437bc80f30c34bfe95e60a73d26faa39a`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 2.1 MB (2128094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b92b058cf5a162f3e9e9c1b57e6ea521b98cfbdfe95c64e96543614c0aa889`  
		Last Modified: Tue, 13 Oct 2020 02:37:26 GMT  
		Size: 7.0 MB (7037515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e07e79b0faf86dec01bde507101fa39b284b027b0a16dcc2e0385b2711b7d7`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774b42f92e50846c6909f7c57a4559f4e39365596961f3cc60c181fd5ff02f7`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:672edee7237da76ba6de9367e734a27d7f8f8562c11afcb03f3b145d6d260015
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e88bd24524f59d6103fec000e35dde5b823055a634e55e935d247d8ac5444a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:19:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 03:20:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 03:20:03 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 03:20:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 03:20:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 03:21:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 03:21:10 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 03:21:11 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 03:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 03:21:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 03:21:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfc2a4609d9b5232a9e51a28b5db91ffc8c66f8660df9bcf2f5d1e3bceccec0`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bc9c2699c25d745dbdf0cb778c6194789b2d87ee75581c62527cc53f62a01`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 1.8 MB (1839142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23ff5b2f49dbf01bbcabfe3c39e09035f01987cdb3987c44dd29b8e562c9c79`  
		Last Modified: Tue, 13 Oct 2020 03:21:38 GMT  
		Size: 5.5 MB (5479959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6783146d326266ff3b29ec06b968d70f4c9d910ed3b3d4b90a52adce04f6a4f2`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71a40b93164b5b86c29eae7931a993d7a6b035139e1d330fcaa7bb9f1663d30`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4fd41c2f819eef9269d59418b5ce1e3de747483dce1115198a335f89e2ed4d68
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29747018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:658bc4237c326801c100d892ffd6332d3700b40b758e022496ab15cc980d5611`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:48:29 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 13:49:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 13:49:19 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 13:49:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 13:49:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 13:51:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 13:51:46 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 13:51:56 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 13:52:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 13:52:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 13:52:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde5382cfe32b8a2ce4b9cdf92405a6dba376d0285fea8da1ce0df092c106b0f`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b24458fbcd75ae1275e13e295793e32245eae23c6e64c87ce033b8dce798f4`  
		Last Modified: Tue, 13 Oct 2020 13:53:27 GMT  
		Size: 1.8 MB (1759463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98181d1b9eef07f40ca6a9b777ede47649c44dca09f867fc5fe82c03b079bc5`  
		Last Modified: Tue, 13 Oct 2020 13:53:27 GMT  
		Size: 5.3 MB (5285500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1606280683a6cf7f09675ec62cfa4d2ee9b2751073e7ec412ea7233dc8a5f666`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97dd80032d12155f389234a1adadb4f5a8b908e08ee379f119408a302853281`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:bd8c013e18d70ea795869cd67cc4c91cd12a4a46c99e81a6265b730a8c714ed9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ef4e8f5b127720ba9505de9ed04ecd332a825b084c225f9cc7ff42b6149a2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 21:06:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 21:06:37 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:06:39 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 21:06:41 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 21:06:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 21:07:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 21:07:41 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 21:07:42 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 21:07:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 21:07:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 21:07:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a84f6f016cb9d510c26fe73828e975a9f6fc50997854f8118cb145c074d5ae`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b87b1c6722e9ec22dc49bb335ce8db2bd481ed351a6ddb5c82f6eb6efd0158`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 2.0 MB (2007865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2397a6f08399786b9b34edfa9dba1ef35efd220a5be1e3bf7f0c703afd2852`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 5.9 MB (5905487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454768d2d9825793660ef493926e3a9571a410a33bd15033af0ad860c1a7decd`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc56fbfab291b081b0371559eab32497a05458b34889aa47c4cbfcad16d058`  
		Last Modified: Tue, 13 Oct 2020 21:08:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:020927c2bce85e0a6153b9e3fba53483f1ca59bec55e71c09bfb448087264273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa5ea3e409fa66afb6ac2267b51c0db7a950a67d5efd32aa7094a082bd8ac57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:08:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 07:08:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 07:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 07:09:14 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 07:09:14 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 07:09:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:09:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:09:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745fb22bef9b177604b68c486de51931377440e01812132d536beb88d70a5d21`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d19eade6c6a313dc1c60e86222d6bafb19b6a105b28092bbd0cc98b4c0070f`  
		Last Modified: Tue, 13 Oct 2020 07:09:33 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cde1db9018cf5bdfd3b40054c0ad417b669d165c66aca9a994bc452d3c4fa`  
		Last Modified: Tue, 13 Oct 2020 07:09:36 GMT  
		Size: 11.6 MB (11633161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dca20ce2d893f37dacd76615c6eacb8d643d74c3989b598ab4e4158b6bfc4e`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216b5ffd9d325d221945ae36ab00beed34a9aaea74f6118052db2fcba2c563ea`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:bfe5c974767b865a68adb72cce4848ecaa36cab8992abfaff529176fc18ed961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f86dfdfdd1df8f189c47811b193797f1bd21f709ec9849d5b71fb83d64fc0f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:30:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:30:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:30:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:31:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:31:24 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:31:24 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:31:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:31:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:31:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be50d34e573637b833f398c4bb03213fdc0e39948eb67673d4e6090fd69a86b`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56986f62a854f267f51d23dcdfce8ed543e5c3f7ecaa67057a60aeba849366ae`  
		Last Modified: Tue, 13 Oct 2020 02:31:51 GMT  
		Size: 1.7 MB (1712061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8827c190f0eb33937717d762d6cd11a35e2a49ba62d7af225998650be849266d`  
		Last Modified: Tue, 13 Oct 2020 02:31:56 GMT  
		Size: 6.4 MB (6416237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38c49421fb63af5186fbe4e32552de9ad359f4d9611ca42956e2bce8ce49a98`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f89d8674f8700037b86df03ef1fd4e5e40b04138c1deb95601e7e1723050bb`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:11f9c1dbc68d2bcdd7a7f524027219a963ce523b201e71ae83c7052e635b27c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc337b8be5274e46ce4e2892582058be9fe426dc646660aa407e845573321c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:32:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 08:33:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:33:18 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 08:33:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 08:33:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 08:40:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 08:40:16 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 08:40:29 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 08:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:40:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1d07b98a86b2674f96635104e41916c1e547434cb7d561cd85492408607281`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2c21d3c72f09a47ee5eaa7be57ecda6468c5095c72c0ae090abfab50a53f17`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 2.2 MB (2225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4a219f1f2d5be3ad0b26293fc2b817c1bb804bb21197d100b7dd072101f007`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 6.7 MB (6743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cacc68fbff4f9b9f07d0bb78c5b34216d92ff73ee186cbac165f8ee0cc552`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6e602fa91081254fd3482a446e8d14916d389cda086023515709324d584b`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:3feac6ba4263f960d8481dee734f70e1f4b0daea3436dcc444e6d37616e90f81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33475004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239e569a133e1fb83824c9c12873d8c897d84bc87265b777b3b39e179c31d516`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:29:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 06:29:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 06:29:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 06:29:48 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 06:29:49 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 06:29:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:29:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0e34331f0b780854c48224e0de248e8951e70d8846ff0fe303e83d4425c38`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4244b6ed8088d52ab38a21af88c52cfb32af480c91f3ebb8b84cdb807fe209`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.8 MB (1821803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbf619e3fe12a6407295c6f4a1cd8379ef1e9b588b41999d1fd99578395bf09`  
		Last Modified: Tue, 13 Oct 2020 06:30:08 GMT  
		Size: 5.9 MB (5943472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daaafe9626c1495df1df7db30d89e5f7a3e3e451f17cfe519a205fcd9e900c9`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ebfbb7e7b045ea63889ea6b91bf081c0ba9ac7d0e7b7ca274a841059f6b31`  
		Last Modified: Tue, 13 Oct 2020 06:30:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:6be7b82d1d47a84533f91062e33a9fd4312f88a2a99c992321376fe725fc6211
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
$ docker pull spiped@sha256:cbcdcae2145e7f1c5b4c4e2ec9926e8f7cf2741c2edd41e74eb1a5ca85431c6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a3a8321db5126e2cfa970d9cabeafcbc493ae611c56ac1b7f3bc9c1877287`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:36:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:36:35 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:37:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:37:06 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:37:06 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:37:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7e552308a9a7e56787eb8f2ee2cd0e5ae1bcd3e6e70767a3f1f63d04df1043`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae3cfef5f840d90ca6a31c452db1ff437bc80f30c34bfe95e60a73d26faa39a`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 2.1 MB (2128094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b92b058cf5a162f3e9e9c1b57e6ea521b98cfbdfe95c64e96543614c0aa889`  
		Last Modified: Tue, 13 Oct 2020 02:37:26 GMT  
		Size: 7.0 MB (7037515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e07e79b0faf86dec01bde507101fa39b284b027b0a16dcc2e0385b2711b7d7`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774b42f92e50846c6909f7c57a4559f4e39365596961f3cc60c181fd5ff02f7`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:672edee7237da76ba6de9367e734a27d7f8f8562c11afcb03f3b145d6d260015
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e88bd24524f59d6103fec000e35dde5b823055a634e55e935d247d8ac5444a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:19:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 03:20:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 03:20:03 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 03:20:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 03:20:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 03:21:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 03:21:10 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 03:21:11 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 03:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 03:21:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 03:21:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfc2a4609d9b5232a9e51a28b5db91ffc8c66f8660df9bcf2f5d1e3bceccec0`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bc9c2699c25d745dbdf0cb778c6194789b2d87ee75581c62527cc53f62a01`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 1.8 MB (1839142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23ff5b2f49dbf01bbcabfe3c39e09035f01987cdb3987c44dd29b8e562c9c79`  
		Last Modified: Tue, 13 Oct 2020 03:21:38 GMT  
		Size: 5.5 MB (5479959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6783146d326266ff3b29ec06b968d70f4c9d910ed3b3d4b90a52adce04f6a4f2`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71a40b93164b5b86c29eae7931a993d7a6b035139e1d330fcaa7bb9f1663d30`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4fd41c2f819eef9269d59418b5ce1e3de747483dce1115198a335f89e2ed4d68
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29747018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:658bc4237c326801c100d892ffd6332d3700b40b758e022496ab15cc980d5611`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:48:29 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 13:49:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 13:49:19 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 13:49:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 13:49:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 13:51:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 13:51:46 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 13:51:56 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 13:52:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 13:52:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 13:52:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde5382cfe32b8a2ce4b9cdf92405a6dba376d0285fea8da1ce0df092c106b0f`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b24458fbcd75ae1275e13e295793e32245eae23c6e64c87ce033b8dce798f4`  
		Last Modified: Tue, 13 Oct 2020 13:53:27 GMT  
		Size: 1.8 MB (1759463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98181d1b9eef07f40ca6a9b777ede47649c44dca09f867fc5fe82c03b079bc5`  
		Last Modified: Tue, 13 Oct 2020 13:53:27 GMT  
		Size: 5.3 MB (5285500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1606280683a6cf7f09675ec62cfa4d2ee9b2751073e7ec412ea7233dc8a5f666`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97dd80032d12155f389234a1adadb4f5a8b908e08ee379f119408a302853281`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:bd8c013e18d70ea795869cd67cc4c91cd12a4a46c99e81a6265b730a8c714ed9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ef4e8f5b127720ba9505de9ed04ecd332a825b084c225f9cc7ff42b6149a2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 21:06:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 21:06:37 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:06:39 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 21:06:41 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 21:06:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 21:07:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 21:07:41 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 21:07:42 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 21:07:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 21:07:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 21:07:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a84f6f016cb9d510c26fe73828e975a9f6fc50997854f8118cb145c074d5ae`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b87b1c6722e9ec22dc49bb335ce8db2bd481ed351a6ddb5c82f6eb6efd0158`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 2.0 MB (2007865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2397a6f08399786b9b34edfa9dba1ef35efd220a5be1e3bf7f0c703afd2852`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 5.9 MB (5905487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454768d2d9825793660ef493926e3a9571a410a33bd15033af0ad860c1a7decd`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc56fbfab291b081b0371559eab32497a05458b34889aa47c4cbfcad16d058`  
		Last Modified: Tue, 13 Oct 2020 21:08:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:020927c2bce85e0a6153b9e3fba53483f1ca59bec55e71c09bfb448087264273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa5ea3e409fa66afb6ac2267b51c0db7a950a67d5efd32aa7094a082bd8ac57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:08:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 07:08:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 07:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 07:09:14 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 07:09:14 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 07:09:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:09:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:09:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745fb22bef9b177604b68c486de51931377440e01812132d536beb88d70a5d21`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d19eade6c6a313dc1c60e86222d6bafb19b6a105b28092bbd0cc98b4c0070f`  
		Last Modified: Tue, 13 Oct 2020 07:09:33 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cde1db9018cf5bdfd3b40054c0ad417b669d165c66aca9a994bc452d3c4fa`  
		Last Modified: Tue, 13 Oct 2020 07:09:36 GMT  
		Size: 11.6 MB (11633161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dca20ce2d893f37dacd76615c6eacb8d643d74c3989b598ab4e4158b6bfc4e`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216b5ffd9d325d221945ae36ab00beed34a9aaea74f6118052db2fcba2c563ea`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:bfe5c974767b865a68adb72cce4848ecaa36cab8992abfaff529176fc18ed961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f86dfdfdd1df8f189c47811b193797f1bd21f709ec9849d5b71fb83d64fc0f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:30:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:30:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:30:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:31:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:31:24 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:31:24 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:31:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:31:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:31:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be50d34e573637b833f398c4bb03213fdc0e39948eb67673d4e6090fd69a86b`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56986f62a854f267f51d23dcdfce8ed543e5c3f7ecaa67057a60aeba849366ae`  
		Last Modified: Tue, 13 Oct 2020 02:31:51 GMT  
		Size: 1.7 MB (1712061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8827c190f0eb33937717d762d6cd11a35e2a49ba62d7af225998650be849266d`  
		Last Modified: Tue, 13 Oct 2020 02:31:56 GMT  
		Size: 6.4 MB (6416237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38c49421fb63af5186fbe4e32552de9ad359f4d9611ca42956e2bce8ce49a98`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f89d8674f8700037b86df03ef1fd4e5e40b04138c1deb95601e7e1723050bb`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:11f9c1dbc68d2bcdd7a7f524027219a963ce523b201e71ae83c7052e635b27c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc337b8be5274e46ce4e2892582058be9fe426dc646660aa407e845573321c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:32:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 08:33:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:33:18 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 08:33:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 08:33:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 08:40:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 08:40:16 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 08:40:29 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 08:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:40:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1d07b98a86b2674f96635104e41916c1e547434cb7d561cd85492408607281`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2c21d3c72f09a47ee5eaa7be57ecda6468c5095c72c0ae090abfab50a53f17`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 2.2 MB (2225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4a219f1f2d5be3ad0b26293fc2b817c1bb804bb21197d100b7dd072101f007`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 6.7 MB (6743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cacc68fbff4f9b9f07d0bb78c5b34216d92ff73ee186cbac165f8ee0cc552`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6e602fa91081254fd3482a446e8d14916d389cda086023515709324d584b`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:3feac6ba4263f960d8481dee734f70e1f4b0daea3436dcc444e6d37616e90f81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33475004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239e569a133e1fb83824c9c12873d8c897d84bc87265b777b3b39e179c31d516`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:29:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 06:29:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 06:29:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 06:29:48 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 06:29:49 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 06:29:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:29:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0e34331f0b780854c48224e0de248e8951e70d8846ff0fe303e83d4425c38`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4244b6ed8088d52ab38a21af88c52cfb32af480c91f3ebb8b84cdb807fe209`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.8 MB (1821803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbf619e3fe12a6407295c6f4a1cd8379ef1e9b588b41999d1fd99578395bf09`  
		Last Modified: Tue, 13 Oct 2020 06:30:08 GMT  
		Size: 5.9 MB (5943472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daaafe9626c1495df1df7db30d89e5f7a3e3e451f17cfe519a205fcd9e900c9`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ebfbb7e7b045ea63889ea6b91bf081c0ba9ac7d0e7b7ca274a841059f6b31`  
		Last Modified: Tue, 13 Oct 2020 06:30:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:6be7b82d1d47a84533f91062e33a9fd4312f88a2a99c992321376fe725fc6211
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
$ docker pull spiped@sha256:cbcdcae2145e7f1c5b4c4e2ec9926e8f7cf2741c2edd41e74eb1a5ca85431c6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a3a8321db5126e2cfa970d9cabeafcbc493ae611c56ac1b7f3bc9c1877287`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:36:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:36:35 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:37:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:37:06 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:37:06 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:37:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7e552308a9a7e56787eb8f2ee2cd0e5ae1bcd3e6e70767a3f1f63d04df1043`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae3cfef5f840d90ca6a31c452db1ff437bc80f30c34bfe95e60a73d26faa39a`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 2.1 MB (2128094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b92b058cf5a162f3e9e9c1b57e6ea521b98cfbdfe95c64e96543614c0aa889`  
		Last Modified: Tue, 13 Oct 2020 02:37:26 GMT  
		Size: 7.0 MB (7037515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e07e79b0faf86dec01bde507101fa39b284b027b0a16dcc2e0385b2711b7d7`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774b42f92e50846c6909f7c57a4559f4e39365596961f3cc60c181fd5ff02f7`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:672edee7237da76ba6de9367e734a27d7f8f8562c11afcb03f3b145d6d260015
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e88bd24524f59d6103fec000e35dde5b823055a634e55e935d247d8ac5444a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:19:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 03:20:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 03:20:03 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 03:20:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 03:20:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 03:21:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 03:21:10 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 03:21:11 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 03:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 03:21:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 03:21:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfc2a4609d9b5232a9e51a28b5db91ffc8c66f8660df9bcf2f5d1e3bceccec0`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bc9c2699c25d745dbdf0cb778c6194789b2d87ee75581c62527cc53f62a01`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 1.8 MB (1839142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23ff5b2f49dbf01bbcabfe3c39e09035f01987cdb3987c44dd29b8e562c9c79`  
		Last Modified: Tue, 13 Oct 2020 03:21:38 GMT  
		Size: 5.5 MB (5479959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6783146d326266ff3b29ec06b968d70f4c9d910ed3b3d4b90a52adce04f6a4f2`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71a40b93164b5b86c29eae7931a993d7a6b035139e1d330fcaa7bb9f1663d30`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4fd41c2f819eef9269d59418b5ce1e3de747483dce1115198a335f89e2ed4d68
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29747018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:658bc4237c326801c100d892ffd6332d3700b40b758e022496ab15cc980d5611`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:48:29 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 13:49:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 13:49:19 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 13:49:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 13:49:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 13:51:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 13:51:46 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 13:51:56 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 13:52:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 13:52:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 13:52:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde5382cfe32b8a2ce4b9cdf92405a6dba376d0285fea8da1ce0df092c106b0f`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b24458fbcd75ae1275e13e295793e32245eae23c6e64c87ce033b8dce798f4`  
		Last Modified: Tue, 13 Oct 2020 13:53:27 GMT  
		Size: 1.8 MB (1759463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98181d1b9eef07f40ca6a9b777ede47649c44dca09f867fc5fe82c03b079bc5`  
		Last Modified: Tue, 13 Oct 2020 13:53:27 GMT  
		Size: 5.3 MB (5285500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1606280683a6cf7f09675ec62cfa4d2ee9b2751073e7ec412ea7233dc8a5f666`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97dd80032d12155f389234a1adadb4f5a8b908e08ee379f119408a302853281`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:bd8c013e18d70ea795869cd67cc4c91cd12a4a46c99e81a6265b730a8c714ed9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ef4e8f5b127720ba9505de9ed04ecd332a825b084c225f9cc7ff42b6149a2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 21:06:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 21:06:37 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:06:39 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 21:06:41 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 21:06:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 21:07:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 21:07:41 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 21:07:42 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 21:07:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 21:07:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 21:07:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a84f6f016cb9d510c26fe73828e975a9f6fc50997854f8118cb145c074d5ae`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b87b1c6722e9ec22dc49bb335ce8db2bd481ed351a6ddb5c82f6eb6efd0158`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 2.0 MB (2007865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2397a6f08399786b9b34edfa9dba1ef35efd220a5be1e3bf7f0c703afd2852`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 5.9 MB (5905487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454768d2d9825793660ef493926e3a9571a410a33bd15033af0ad860c1a7decd`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc56fbfab291b081b0371559eab32497a05458b34889aa47c4cbfcad16d058`  
		Last Modified: Tue, 13 Oct 2020 21:08:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:020927c2bce85e0a6153b9e3fba53483f1ca59bec55e71c09bfb448087264273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa5ea3e409fa66afb6ac2267b51c0db7a950a67d5efd32aa7094a082bd8ac57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:08:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 07:08:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 07:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 07:09:14 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 07:09:14 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 07:09:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:09:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:09:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745fb22bef9b177604b68c486de51931377440e01812132d536beb88d70a5d21`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d19eade6c6a313dc1c60e86222d6bafb19b6a105b28092bbd0cc98b4c0070f`  
		Last Modified: Tue, 13 Oct 2020 07:09:33 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cde1db9018cf5bdfd3b40054c0ad417b669d165c66aca9a994bc452d3c4fa`  
		Last Modified: Tue, 13 Oct 2020 07:09:36 GMT  
		Size: 11.6 MB (11633161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dca20ce2d893f37dacd76615c6eacb8d643d74c3989b598ab4e4158b6bfc4e`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216b5ffd9d325d221945ae36ab00beed34a9aaea74f6118052db2fcba2c563ea`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:bfe5c974767b865a68adb72cce4848ecaa36cab8992abfaff529176fc18ed961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f86dfdfdd1df8f189c47811b193797f1bd21f709ec9849d5b71fb83d64fc0f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:30:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:30:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:30:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:31:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:31:24 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:31:24 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:31:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:31:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:31:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be50d34e573637b833f398c4bb03213fdc0e39948eb67673d4e6090fd69a86b`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56986f62a854f267f51d23dcdfce8ed543e5c3f7ecaa67057a60aeba849366ae`  
		Last Modified: Tue, 13 Oct 2020 02:31:51 GMT  
		Size: 1.7 MB (1712061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8827c190f0eb33937717d762d6cd11a35e2a49ba62d7af225998650be849266d`  
		Last Modified: Tue, 13 Oct 2020 02:31:56 GMT  
		Size: 6.4 MB (6416237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38c49421fb63af5186fbe4e32552de9ad359f4d9611ca42956e2bce8ce49a98`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f89d8674f8700037b86df03ef1fd4e5e40b04138c1deb95601e7e1723050bb`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:11f9c1dbc68d2bcdd7a7f524027219a963ce523b201e71ae83c7052e635b27c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc337b8be5274e46ce4e2892582058be9fe426dc646660aa407e845573321c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:32:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 08:33:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:33:18 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 08:33:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 08:33:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 08:40:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 08:40:16 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 08:40:29 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 08:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:40:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1d07b98a86b2674f96635104e41916c1e547434cb7d561cd85492408607281`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2c21d3c72f09a47ee5eaa7be57ecda6468c5095c72c0ae090abfab50a53f17`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 2.2 MB (2225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4a219f1f2d5be3ad0b26293fc2b817c1bb804bb21197d100b7dd072101f007`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 6.7 MB (6743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cacc68fbff4f9b9f07d0bb78c5b34216d92ff73ee186cbac165f8ee0cc552`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6e602fa91081254fd3482a446e8d14916d389cda086023515709324d584b`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:3feac6ba4263f960d8481dee734f70e1f4b0daea3436dcc444e6d37616e90f81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33475004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239e569a133e1fb83824c9c12873d8c897d84bc87265b777b3b39e179c31d516`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:29:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 06:29:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 06:29:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 06:29:48 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 06:29:49 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 06:29:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:29:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0e34331f0b780854c48224e0de248e8951e70d8846ff0fe303e83d4425c38`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4244b6ed8088d52ab38a21af88c52cfb32af480c91f3ebb8b84cdb807fe209`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.8 MB (1821803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbf619e3fe12a6407295c6f4a1cd8379ef1e9b588b41999d1fd99578395bf09`  
		Last Modified: Tue, 13 Oct 2020 06:30:08 GMT  
		Size: 5.9 MB (5943472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daaafe9626c1495df1df7db30d89e5f7a3e3e451f17cfe519a205fcd9e900c9`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ebfbb7e7b045ea63889ea6b91bf081c0ba9ac7d0e7b7ca274a841059f6b31`  
		Last Modified: Tue, 13 Oct 2020 06:30:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:e5f247d6c429f155f34a5c004ff0498fbe5f98906d4be2776b992e3261b51b4d
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1913a59773cf295dd8d96f26cc0ba23e5325c4b318f2e48b1668736a9a5ae532
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648a07e74593903bb0b5a422c8c3f677102d278b79b31a76cba4b51e1be16af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:59:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:59:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:59:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 03:00:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 03:00:11 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 03:00:12 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 03:00:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 03:00:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:00:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d19d74400f766b7b4a9239a805587a1523517a166d14ed12a1bc5435fcca7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a534ce800d06acec8b2e639d97798306f250838441b482b3dba8a16bc6ff45f`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194e2e34702b51562d461ab44982ea3720b4edf6bcf81e135005398c1f9bdc7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 191.6 KB (191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d152e941e8212f73f472183f3c9742b6a5c8670c44519dd69234bc46428dcc04`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41531b30548b2b91cc5b6563486356d5a291b1e56c550ce60fa95fcd766c25`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:ed00bdf5d77410d087603e844f75c7b1f252bdc798d7ec5848d671dd194c0b13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d72ee5b0edc357b741d48d1b0f08ba0520a023b027a598d1ba0b935750a0c0b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:40:20 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 02:40:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 02:40:31 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 02:40:32 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 02:40:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 02:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:40:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8abed0ed8c01bd2270afd6e719193df68ecfb17beb92641dd15d668c89df23`  
		Last Modified: Thu, 22 Oct 2020 02:40:46 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6319807f270dfddcc07a169d0fe827f25eafb418323c89afa7d3a4ae0c82e3be`  
		Last Modified: Thu, 22 Oct 2020 02:40:46 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b35c08f2d3cbdc83eba1b5ebcb4916904a66e951c723a170126decf35dc389`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 203.0 KB (203015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7dbf2bbee620d5da2ff8f2a9e9c2ceddc95dc46b67026512d55fbfc2d8193ac`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6f6fa3f62a953de92893da3b06c551a1249a13fc03c083d980d304ef68f07e`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:e5f247d6c429f155f34a5c004ff0498fbe5f98906d4be2776b992e3261b51b4d
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1913a59773cf295dd8d96f26cc0ba23e5325c4b318f2e48b1668736a9a5ae532
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648a07e74593903bb0b5a422c8c3f677102d278b79b31a76cba4b51e1be16af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:59:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:59:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:59:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 03:00:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 03:00:11 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 03:00:12 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 03:00:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 03:00:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:00:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d19d74400f766b7b4a9239a805587a1523517a166d14ed12a1bc5435fcca7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a534ce800d06acec8b2e639d97798306f250838441b482b3dba8a16bc6ff45f`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194e2e34702b51562d461ab44982ea3720b4edf6bcf81e135005398c1f9bdc7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 191.6 KB (191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d152e941e8212f73f472183f3c9742b6a5c8670c44519dd69234bc46428dcc04`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41531b30548b2b91cc5b6563486356d5a291b1e56c550ce60fa95fcd766c25`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:ed00bdf5d77410d087603e844f75c7b1f252bdc798d7ec5848d671dd194c0b13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d72ee5b0edc357b741d48d1b0f08ba0520a023b027a598d1ba0b935750a0c0b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:40:20 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 02:40:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 02:40:31 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 02:40:32 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 02:40:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 02:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:40:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8abed0ed8c01bd2270afd6e719193df68ecfb17beb92641dd15d668c89df23`  
		Last Modified: Thu, 22 Oct 2020 02:40:46 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6319807f270dfddcc07a169d0fe827f25eafb418323c89afa7d3a4ae0c82e3be`  
		Last Modified: Thu, 22 Oct 2020 02:40:46 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b35c08f2d3cbdc83eba1b5ebcb4916904a66e951c723a170126decf35dc389`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 203.0 KB (203015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7dbf2bbee620d5da2ff8f2a9e9c2ceddc95dc46b67026512d55fbfc2d8193ac`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6f6fa3f62a953de92893da3b06c551a1249a13fc03c083d980d304ef68f07e`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:e5f247d6c429f155f34a5c004ff0498fbe5f98906d4be2776b992e3261b51b4d
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1913a59773cf295dd8d96f26cc0ba23e5325c4b318f2e48b1668736a9a5ae532
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648a07e74593903bb0b5a422c8c3f677102d278b79b31a76cba4b51e1be16af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:59:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:59:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:59:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 03:00:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 03:00:11 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 03:00:12 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 03:00:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 03:00:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:00:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d19d74400f766b7b4a9239a805587a1523517a166d14ed12a1bc5435fcca7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a534ce800d06acec8b2e639d97798306f250838441b482b3dba8a16bc6ff45f`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194e2e34702b51562d461ab44982ea3720b4edf6bcf81e135005398c1f9bdc7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 191.6 KB (191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d152e941e8212f73f472183f3c9742b6a5c8670c44519dd69234bc46428dcc04`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41531b30548b2b91cc5b6563486356d5a291b1e56c550ce60fa95fcd766c25`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:ed00bdf5d77410d087603e844f75c7b1f252bdc798d7ec5848d671dd194c0b13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d72ee5b0edc357b741d48d1b0f08ba0520a023b027a598d1ba0b935750a0c0b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:40:20 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 02:40:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 02:40:31 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 02:40:32 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 02:40:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 02:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:40:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8abed0ed8c01bd2270afd6e719193df68ecfb17beb92641dd15d668c89df23`  
		Last Modified: Thu, 22 Oct 2020 02:40:46 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6319807f270dfddcc07a169d0fe827f25eafb418323c89afa7d3a4ae0c82e3be`  
		Last Modified: Thu, 22 Oct 2020 02:40:46 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b35c08f2d3cbdc83eba1b5ebcb4916904a66e951c723a170126decf35dc389`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 203.0 KB (203015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7dbf2bbee620d5da2ff8f2a9e9c2ceddc95dc46b67026512d55fbfc2d8193ac`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6f6fa3f62a953de92893da3b06c551a1249a13fc03c083d980d304ef68f07e`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:e5f247d6c429f155f34a5c004ff0498fbe5f98906d4be2776b992e3261b51b4d
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1913a59773cf295dd8d96f26cc0ba23e5325c4b318f2e48b1668736a9a5ae532
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648a07e74593903bb0b5a422c8c3f677102d278b79b31a76cba4b51e1be16af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:59:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:59:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:59:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 03:00:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 03:00:11 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 03:00:12 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 03:00:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 03:00:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:00:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d19d74400f766b7b4a9239a805587a1523517a166d14ed12a1bc5435fcca7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a534ce800d06acec8b2e639d97798306f250838441b482b3dba8a16bc6ff45f`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194e2e34702b51562d461ab44982ea3720b4edf6bcf81e135005398c1f9bdc7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 191.6 KB (191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d152e941e8212f73f472183f3c9742b6a5c8670c44519dd69234bc46428dcc04`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41531b30548b2b91cc5b6563486356d5a291b1e56c550ce60fa95fcd766c25`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:ed00bdf5d77410d087603e844f75c7b1f252bdc798d7ec5848d671dd194c0b13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d72ee5b0edc357b741d48d1b0f08ba0520a023b027a598d1ba0b935750a0c0b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:40:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:40:20 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:40:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 02:40:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 02:40:31 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 02:40:32 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 02:40:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 02:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:40:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8abed0ed8c01bd2270afd6e719193df68ecfb17beb92641dd15d668c89df23`  
		Last Modified: Thu, 22 Oct 2020 02:40:46 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6319807f270dfddcc07a169d0fe827f25eafb418323c89afa7d3a4ae0c82e3be`  
		Last Modified: Thu, 22 Oct 2020 02:40:46 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b35c08f2d3cbdc83eba1b5ebcb4916904a66e951c723a170126decf35dc389`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 203.0 KB (203015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7dbf2bbee620d5da2ff8f2a9e9c2ceddc95dc46b67026512d55fbfc2d8193ac`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6f6fa3f62a953de92893da3b06c551a1249a13fc03c083d980d304ef68f07e`  
		Last Modified: Thu, 22 Oct 2020 02:40:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:6be7b82d1d47a84533f91062e33a9fd4312f88a2a99c992321376fe725fc6211
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
$ docker pull spiped@sha256:cbcdcae2145e7f1c5b4c4e2ec9926e8f7cf2741c2edd41e74eb1a5ca85431c6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a3a8321db5126e2cfa970d9cabeafcbc493ae611c56ac1b7f3bc9c1877287`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:36:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:36:35 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:37:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:37:06 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:37:06 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:37:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7e552308a9a7e56787eb8f2ee2cd0e5ae1bcd3e6e70767a3f1f63d04df1043`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae3cfef5f840d90ca6a31c452db1ff437bc80f30c34bfe95e60a73d26faa39a`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 2.1 MB (2128094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b92b058cf5a162f3e9e9c1b57e6ea521b98cfbdfe95c64e96543614c0aa889`  
		Last Modified: Tue, 13 Oct 2020 02:37:26 GMT  
		Size: 7.0 MB (7037515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e07e79b0faf86dec01bde507101fa39b284b027b0a16dcc2e0385b2711b7d7`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774b42f92e50846c6909f7c57a4559f4e39365596961f3cc60c181fd5ff02f7`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:672edee7237da76ba6de9367e734a27d7f8f8562c11afcb03f3b145d6d260015
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e88bd24524f59d6103fec000e35dde5b823055a634e55e935d247d8ac5444a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:19:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 03:20:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 03:20:03 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 03:20:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 03:20:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 03:21:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 03:21:10 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 03:21:11 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 03:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 03:21:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 03:21:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfc2a4609d9b5232a9e51a28b5db91ffc8c66f8660df9bcf2f5d1e3bceccec0`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bc9c2699c25d745dbdf0cb778c6194789b2d87ee75581c62527cc53f62a01`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 1.8 MB (1839142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23ff5b2f49dbf01bbcabfe3c39e09035f01987cdb3987c44dd29b8e562c9c79`  
		Last Modified: Tue, 13 Oct 2020 03:21:38 GMT  
		Size: 5.5 MB (5479959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6783146d326266ff3b29ec06b968d70f4c9d910ed3b3d4b90a52adce04f6a4f2`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71a40b93164b5b86c29eae7931a993d7a6b035139e1d330fcaa7bb9f1663d30`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4fd41c2f819eef9269d59418b5ce1e3de747483dce1115198a335f89e2ed4d68
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29747018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:658bc4237c326801c100d892ffd6332d3700b40b758e022496ab15cc980d5611`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:48:29 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 13:49:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 13:49:19 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 13:49:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 13:49:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 13:51:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 13:51:46 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 13:51:56 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 13:52:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 13:52:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 13:52:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde5382cfe32b8a2ce4b9cdf92405a6dba376d0285fea8da1ce0df092c106b0f`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b24458fbcd75ae1275e13e295793e32245eae23c6e64c87ce033b8dce798f4`  
		Last Modified: Tue, 13 Oct 2020 13:53:27 GMT  
		Size: 1.8 MB (1759463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98181d1b9eef07f40ca6a9b777ede47649c44dca09f867fc5fe82c03b079bc5`  
		Last Modified: Tue, 13 Oct 2020 13:53:27 GMT  
		Size: 5.3 MB (5285500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1606280683a6cf7f09675ec62cfa4d2ee9b2751073e7ec412ea7233dc8a5f666`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97dd80032d12155f389234a1adadb4f5a8b908e08ee379f119408a302853281`  
		Last Modified: Tue, 13 Oct 2020 13:53:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:bd8c013e18d70ea795869cd67cc4c91cd12a4a46c99e81a6265b730a8c714ed9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ef4e8f5b127720ba9505de9ed04ecd332a825b084c225f9cc7ff42b6149a2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 21:06:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 21:06:37 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:06:39 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 21:06:41 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 21:06:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 21:07:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 21:07:41 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 21:07:42 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 21:07:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 21:07:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 21:07:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a84f6f016cb9d510c26fe73828e975a9f6fc50997854f8118cb145c074d5ae`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b87b1c6722e9ec22dc49bb335ce8db2bd481ed351a6ddb5c82f6eb6efd0158`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 2.0 MB (2007865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2397a6f08399786b9b34edfa9dba1ef35efd220a5be1e3bf7f0c703afd2852`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 5.9 MB (5905487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454768d2d9825793660ef493926e3a9571a410a33bd15033af0ad860c1a7decd`  
		Last Modified: Tue, 13 Oct 2020 21:08:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bc56fbfab291b081b0371559eab32497a05458b34889aa47c4cbfcad16d058`  
		Last Modified: Tue, 13 Oct 2020 21:08:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:020927c2bce85e0a6153b9e3fba53483f1ca59bec55e71c09bfb448087264273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa5ea3e409fa66afb6ac2267b51c0db7a950a67d5efd32aa7094a082bd8ac57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:08:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 07:08:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 07:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 07:09:14 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 07:09:14 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 07:09:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:09:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:09:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745fb22bef9b177604b68c486de51931377440e01812132d536beb88d70a5d21`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d19eade6c6a313dc1c60e86222d6bafb19b6a105b28092bbd0cc98b4c0070f`  
		Last Modified: Tue, 13 Oct 2020 07:09:33 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cde1db9018cf5bdfd3b40054c0ad417b669d165c66aca9a994bc452d3c4fa`  
		Last Modified: Tue, 13 Oct 2020 07:09:36 GMT  
		Size: 11.6 MB (11633161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dca20ce2d893f37dacd76615c6eacb8d643d74c3989b598ab4e4158b6bfc4e`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216b5ffd9d325d221945ae36ab00beed34a9aaea74f6118052db2fcba2c563ea`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:bfe5c974767b865a68adb72cce4848ecaa36cab8992abfaff529176fc18ed961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f86dfdfdd1df8f189c47811b193797f1bd21f709ec9849d5b71fb83d64fc0f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:30:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:30:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:30:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:31:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:31:24 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:31:24 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:31:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:31:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:31:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be50d34e573637b833f398c4bb03213fdc0e39948eb67673d4e6090fd69a86b`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56986f62a854f267f51d23dcdfce8ed543e5c3f7ecaa67057a60aeba849366ae`  
		Last Modified: Tue, 13 Oct 2020 02:31:51 GMT  
		Size: 1.7 MB (1712061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8827c190f0eb33937717d762d6cd11a35e2a49ba62d7af225998650be849266d`  
		Last Modified: Tue, 13 Oct 2020 02:31:56 GMT  
		Size: 6.4 MB (6416237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38c49421fb63af5186fbe4e32552de9ad359f4d9611ca42956e2bce8ce49a98`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f89d8674f8700037b86df03ef1fd4e5e40b04138c1deb95601e7e1723050bb`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:11f9c1dbc68d2bcdd7a7f524027219a963ce523b201e71ae83c7052e635b27c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc337b8be5274e46ce4e2892582058be9fe426dc646660aa407e845573321c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:32:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 08:33:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:33:18 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 08:33:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 08:33:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 08:40:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 08:40:16 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 08:40:29 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 08:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:40:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1d07b98a86b2674f96635104e41916c1e547434cb7d561cd85492408607281`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2c21d3c72f09a47ee5eaa7be57ecda6468c5095c72c0ae090abfab50a53f17`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 2.2 MB (2225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4a219f1f2d5be3ad0b26293fc2b817c1bb804bb21197d100b7dd072101f007`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 6.7 MB (6743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cacc68fbff4f9b9f07d0bb78c5b34216d92ff73ee186cbac165f8ee0cc552`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6e602fa91081254fd3482a446e8d14916d389cda086023515709324d584b`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:3feac6ba4263f960d8481dee734f70e1f4b0daea3436dcc444e6d37616e90f81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33475004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239e569a133e1fb83824c9c12873d8c897d84bc87265b777b3b39e179c31d516`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:29:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 06:29:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 06:29:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 06:29:48 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 06:29:49 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 06:29:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:29:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0e34331f0b780854c48224e0de248e8951e70d8846ff0fe303e83d4425c38`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4244b6ed8088d52ab38a21af88c52cfb32af480c91f3ebb8b84cdb807fe209`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.8 MB (1821803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbf619e3fe12a6407295c6f4a1cd8379ef1e9b588b41999d1fd99578395bf09`  
		Last Modified: Tue, 13 Oct 2020 06:30:08 GMT  
		Size: 5.9 MB (5943472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daaafe9626c1495df1df7db30d89e5f7a3e3e451f17cfe519a205fcd9e900c9`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ebfbb7e7b045ea63889ea6b91bf081c0ba9ac7d0e7b7ca274a841059f6b31`  
		Last Modified: Tue, 13 Oct 2020 06:30:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
