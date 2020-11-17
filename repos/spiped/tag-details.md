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
$ docker pull spiped@sha256:c78456708f62dbca9c7a7374b72b91c5dc039f5ae31eee00c529101049a18044
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
$ docker pull spiped@sha256:db61217a4053f03c05b983f7d2722530fd82d6735e721311d7f90b17be40b713
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33488732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b062dbf1be23d35f8fb2e20a863861f260daee06fb4b84c4e4f7a669a6ecdbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:00:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:00:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:00:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 22:01:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:01:22 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 22:01:22 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 22:01:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 22:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 22:01:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43806a3fd3d362292aa4489b61228dc530d6820323d12f115ae0c4736e1b8ea`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80774235907721c9cd1bfff884ac7b597fe103ccb597a2563894bbc9a60bbb7`  
		Last Modified: Tue, 17 Nov 2020 22:02:11 GMT  
		Size: 1.8 MB (1821805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af91886a196e09e46584c37d8e2a8b40ab99d06f7096b4bed331ab4a63609ee`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 5.9 MB (5943582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d47aa91c0fe928301af1785740dd8890de723dff4c762a9c290e2b85178a1b`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a66f51280aa12fc65c7a03ae1bc737a260e3eb12d0c742a80d2757c48ba6cc`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:c78456708f62dbca9c7a7374b72b91c5dc039f5ae31eee00c529101049a18044
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
$ docker pull spiped@sha256:db61217a4053f03c05b983f7d2722530fd82d6735e721311d7f90b17be40b713
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33488732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b062dbf1be23d35f8fb2e20a863861f260daee06fb4b84c4e4f7a669a6ecdbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:00:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:00:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:00:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 22:01:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:01:22 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 22:01:22 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 22:01:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 22:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 22:01:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43806a3fd3d362292aa4489b61228dc530d6820323d12f115ae0c4736e1b8ea`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80774235907721c9cd1bfff884ac7b597fe103ccb597a2563894bbc9a60bbb7`  
		Last Modified: Tue, 17 Nov 2020 22:02:11 GMT  
		Size: 1.8 MB (1821805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af91886a196e09e46584c37d8e2a8b40ab99d06f7096b4bed331ab4a63609ee`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 5.9 MB (5943582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d47aa91c0fe928301af1785740dd8890de723dff4c762a9c290e2b85178a1b`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a66f51280aa12fc65c7a03ae1bc737a260e3eb12d0c742a80d2757c48ba6cc`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:c78456708f62dbca9c7a7374b72b91c5dc039f5ae31eee00c529101049a18044
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
$ docker pull spiped@sha256:db61217a4053f03c05b983f7d2722530fd82d6735e721311d7f90b17be40b713
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33488732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b062dbf1be23d35f8fb2e20a863861f260daee06fb4b84c4e4f7a669a6ecdbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:00:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:00:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:00:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 22:01:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:01:22 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 22:01:22 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 22:01:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 22:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 22:01:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43806a3fd3d362292aa4489b61228dc530d6820323d12f115ae0c4736e1b8ea`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80774235907721c9cd1bfff884ac7b597fe103ccb597a2563894bbc9a60bbb7`  
		Last Modified: Tue, 17 Nov 2020 22:02:11 GMT  
		Size: 1.8 MB (1821805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af91886a196e09e46584c37d8e2a8b40ab99d06f7096b4bed331ab4a63609ee`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 5.9 MB (5943582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d47aa91c0fe928301af1785740dd8890de723dff4c762a9c290e2b85178a1b`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a66f51280aa12fc65c7a03ae1bc737a260e3eb12d0c742a80d2757c48ba6cc`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:e0204033165a1ac587658e4dc23de07011115408c0d73ad47437a3e936d6bfce
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
$ docker pull spiped@sha256:e72efc9006cc88e74da18f8909e9a6d6cb80c024bc171e1de9a3bfa8082c7e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cd33bc57ff09ba0929eb9a1846e003f8ab8d35ac7f715f376161a9209fb7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:23:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 08:23:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 08:24:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 08:24:10 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 08:24:10 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 08:24:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2cfe9f1210973e807f22612ef44f79fdf4e9f1871ceb24da9c470ff4c6934a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebdc509a836b5478bba964b2f5c1712aa349a3761854c4f1193f580d18193`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2055abf7179bbbbaca992858134f6d59becb2b5cb2f516330f97082d7f4d272`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 211.4 KB (211432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a723ed90b1f6fc5a4bc245ba955d04306500cc3613e897f36a9246cb119a856`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8823b92e870bcac9a4efd674a3b7605e55d9877e47bb6d81c8d47f8e80d12a4a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:14cace5958bfa120cbf111e0c63cbaac02c7ae08cca3a8608d7f65c150a693bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6468ae1c5552249820a405840a8ca1b3217dd186e61222ca1df5425eb4b2ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:31:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:31:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:31:51 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:31:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:31:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:32:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:32:27 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:32:29 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:32:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:32:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acaaa89a9c32df4571254fbd79384a49e286b69f02ab7809109be9e080ac036`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd43fc49572c6e21badb3a526db0c4230a27c474dd5d4462f06ccfc6a96c45dd`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b785525c1135d90a9f438736d288ad7466404c9fdcc1b3dddb49668e94d281ed`  
		Last Modified: Thu, 22 Oct 2020 09:32:54 GMT  
		Size: 198.4 KB (198362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aaf1b15d6e46104f6566df081782ed2ac537c416d74e2d8820c3375d4de796`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64314cf23e502ff1d541e21714ebf47fd1719c58368cfd56ee7fc9c2b75c1397`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:22e076d0704999df6954352a61322c7aff9e84102fb209dca8c67047f0f9ec55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12732fc9350260a757debfd45b04e105fa193198c820121c8fb104c75e4090e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:13:00 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:13:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:13:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:13:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:13:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:13:37 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:13:38 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:13:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ac12de1615c4fcf136e9caab1c56384e869fa371fb1aa91fa6a50584aede8`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49ab63c0d72d683d01704eb4d538cac06f6cccc649a32c793531090a507d758`  
		Last Modified: Thu, 22 Oct 2020 09:14:05 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7c72e8f699aad2c97e9e3116224f712f7a66a5bacec74cb4db459e9275f8d2`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 203.8 KB (203833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc60fd10df854316c0653b5c11cd733c7191a08efa7aa164d9d9e6cb76de12`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47396fd59d212f4a22fd40665e6647db1065fd9aebe2fe3394e3c973688ad64`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:69a8f9d0101fda57680f27c30ca9864f021d69a013d0d876c7f010296105365d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aeca41fe853b4af9d83ed356e1a338abb14a58e5645c3cb4a0756640886dc5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:58:32 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 05:58:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 05:58:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 05:58:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 05:58:53 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 05:58:53 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 05:58:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:58:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 05:58:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cf7cc4c20069210dbf0b03ab1fecd91e3d95b49c97e98cae7c670b28f0033`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf8eec65d1d720af4b0e901af92897e91841e174ac0414999f9174673879238`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca18ab8a4b82f11e9d159625a64a3b9923866ef0471b97f803fb09071405476`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 221.2 KB (221209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cce939bb90551e9a0f849ecdfad6c57fde68602a16c1a208154aaa6a5d2c49b`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230d405b698f37c531145e3d12d6c2db6858a39fb6b5bd2a61b1e6dec0a9f38f`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:c27d5fef225f76543118f6caa3acde60dc973cd24f4e33cb59090137381f2919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f1bbe21c527c03ef60714e2068bba645f66ce1506897d0529721db3b3db1262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 16:48:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 16:48:47 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 16:48:55 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 16:49:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 16:49:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 16:49:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 16:50:06 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 16:50:18 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 16:50:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 16:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 16:50:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942add97a5cb7e2c0420027c4ee428f7f8acc5c9ef7cf42145ae3e8d6169c280`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b04d7f19ebc8c84adc2f6cdf2f47f39edd6a40070b1a9fe013aa04bb19661`  
		Last Modified: Thu, 22 Oct 2020 16:51:11 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2284ab6cc6051b68486ca0c4ff330e9f9642af3f7edcb7b3f313e227c1dfbb81`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 219.0 KB (219035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d5eac542c6cee08a3a0540a86e200be7a8e7eacd50bfb2f6578d2dac35e894`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7c2df90d7b01b0207ff6e0e55de8177f67606a695437e5035e2c8b4e32a7ca`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:e0204033165a1ac587658e4dc23de07011115408c0d73ad47437a3e936d6bfce
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
$ docker pull spiped@sha256:e72efc9006cc88e74da18f8909e9a6d6cb80c024bc171e1de9a3bfa8082c7e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cd33bc57ff09ba0929eb9a1846e003f8ab8d35ac7f715f376161a9209fb7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:23:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 08:23:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 08:24:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 08:24:10 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 08:24:10 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 08:24:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2cfe9f1210973e807f22612ef44f79fdf4e9f1871ceb24da9c470ff4c6934a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebdc509a836b5478bba964b2f5c1712aa349a3761854c4f1193f580d18193`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2055abf7179bbbbaca992858134f6d59becb2b5cb2f516330f97082d7f4d272`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 211.4 KB (211432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a723ed90b1f6fc5a4bc245ba955d04306500cc3613e897f36a9246cb119a856`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8823b92e870bcac9a4efd674a3b7605e55d9877e47bb6d81c8d47f8e80d12a4a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:14cace5958bfa120cbf111e0c63cbaac02c7ae08cca3a8608d7f65c150a693bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6468ae1c5552249820a405840a8ca1b3217dd186e61222ca1df5425eb4b2ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:31:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:31:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:31:51 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:31:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:31:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:32:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:32:27 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:32:29 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:32:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:32:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acaaa89a9c32df4571254fbd79384a49e286b69f02ab7809109be9e080ac036`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd43fc49572c6e21badb3a526db0c4230a27c474dd5d4462f06ccfc6a96c45dd`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b785525c1135d90a9f438736d288ad7466404c9fdcc1b3dddb49668e94d281ed`  
		Last Modified: Thu, 22 Oct 2020 09:32:54 GMT  
		Size: 198.4 KB (198362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aaf1b15d6e46104f6566df081782ed2ac537c416d74e2d8820c3375d4de796`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64314cf23e502ff1d541e21714ebf47fd1719c58368cfd56ee7fc9c2b75c1397`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:22e076d0704999df6954352a61322c7aff9e84102fb209dca8c67047f0f9ec55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12732fc9350260a757debfd45b04e105fa193198c820121c8fb104c75e4090e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:13:00 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:13:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:13:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:13:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:13:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:13:37 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:13:38 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:13:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ac12de1615c4fcf136e9caab1c56384e869fa371fb1aa91fa6a50584aede8`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49ab63c0d72d683d01704eb4d538cac06f6cccc649a32c793531090a507d758`  
		Last Modified: Thu, 22 Oct 2020 09:14:05 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7c72e8f699aad2c97e9e3116224f712f7a66a5bacec74cb4db459e9275f8d2`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 203.8 KB (203833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc60fd10df854316c0653b5c11cd733c7191a08efa7aa164d9d9e6cb76de12`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47396fd59d212f4a22fd40665e6647db1065fd9aebe2fe3394e3c973688ad64`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:69a8f9d0101fda57680f27c30ca9864f021d69a013d0d876c7f010296105365d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aeca41fe853b4af9d83ed356e1a338abb14a58e5645c3cb4a0756640886dc5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:58:32 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 05:58:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 05:58:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 05:58:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 05:58:53 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 05:58:53 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 05:58:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:58:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 05:58:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cf7cc4c20069210dbf0b03ab1fecd91e3d95b49c97e98cae7c670b28f0033`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf8eec65d1d720af4b0e901af92897e91841e174ac0414999f9174673879238`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca18ab8a4b82f11e9d159625a64a3b9923866ef0471b97f803fb09071405476`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 221.2 KB (221209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cce939bb90551e9a0f849ecdfad6c57fde68602a16c1a208154aaa6a5d2c49b`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230d405b698f37c531145e3d12d6c2db6858a39fb6b5bd2a61b1e6dec0a9f38f`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:c27d5fef225f76543118f6caa3acde60dc973cd24f4e33cb59090137381f2919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f1bbe21c527c03ef60714e2068bba645f66ce1506897d0529721db3b3db1262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 16:48:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 16:48:47 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 16:48:55 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 16:49:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 16:49:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 16:49:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 16:50:06 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 16:50:18 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 16:50:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 16:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 16:50:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942add97a5cb7e2c0420027c4ee428f7f8acc5c9ef7cf42145ae3e8d6169c280`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b04d7f19ebc8c84adc2f6cdf2f47f39edd6a40070b1a9fe013aa04bb19661`  
		Last Modified: Thu, 22 Oct 2020 16:51:11 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2284ab6cc6051b68486ca0c4ff330e9f9642af3f7edcb7b3f313e227c1dfbb81`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 219.0 KB (219035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d5eac542c6cee08a3a0540a86e200be7a8e7eacd50bfb2f6578d2dac35e894`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7c2df90d7b01b0207ff6e0e55de8177f67606a695437e5035e2c8b4e32a7ca`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:e0204033165a1ac587658e4dc23de07011115408c0d73ad47437a3e936d6bfce
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
$ docker pull spiped@sha256:e72efc9006cc88e74da18f8909e9a6d6cb80c024bc171e1de9a3bfa8082c7e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cd33bc57ff09ba0929eb9a1846e003f8ab8d35ac7f715f376161a9209fb7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:23:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 08:23:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 08:24:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 08:24:10 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 08:24:10 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 08:24:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2cfe9f1210973e807f22612ef44f79fdf4e9f1871ceb24da9c470ff4c6934a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebdc509a836b5478bba964b2f5c1712aa349a3761854c4f1193f580d18193`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2055abf7179bbbbaca992858134f6d59becb2b5cb2f516330f97082d7f4d272`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 211.4 KB (211432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a723ed90b1f6fc5a4bc245ba955d04306500cc3613e897f36a9246cb119a856`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8823b92e870bcac9a4efd674a3b7605e55d9877e47bb6d81c8d47f8e80d12a4a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:14cace5958bfa120cbf111e0c63cbaac02c7ae08cca3a8608d7f65c150a693bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6468ae1c5552249820a405840a8ca1b3217dd186e61222ca1df5425eb4b2ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:31:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:31:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:31:51 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:31:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:31:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:32:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:32:27 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:32:29 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:32:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:32:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acaaa89a9c32df4571254fbd79384a49e286b69f02ab7809109be9e080ac036`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd43fc49572c6e21badb3a526db0c4230a27c474dd5d4462f06ccfc6a96c45dd`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b785525c1135d90a9f438736d288ad7466404c9fdcc1b3dddb49668e94d281ed`  
		Last Modified: Thu, 22 Oct 2020 09:32:54 GMT  
		Size: 198.4 KB (198362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aaf1b15d6e46104f6566df081782ed2ac537c416d74e2d8820c3375d4de796`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64314cf23e502ff1d541e21714ebf47fd1719c58368cfd56ee7fc9c2b75c1397`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:22e076d0704999df6954352a61322c7aff9e84102fb209dca8c67047f0f9ec55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12732fc9350260a757debfd45b04e105fa193198c820121c8fb104c75e4090e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:13:00 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:13:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:13:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:13:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:13:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:13:37 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:13:38 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:13:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ac12de1615c4fcf136e9caab1c56384e869fa371fb1aa91fa6a50584aede8`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49ab63c0d72d683d01704eb4d538cac06f6cccc649a32c793531090a507d758`  
		Last Modified: Thu, 22 Oct 2020 09:14:05 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7c72e8f699aad2c97e9e3116224f712f7a66a5bacec74cb4db459e9275f8d2`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 203.8 KB (203833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc60fd10df854316c0653b5c11cd733c7191a08efa7aa164d9d9e6cb76de12`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47396fd59d212f4a22fd40665e6647db1065fd9aebe2fe3394e3c973688ad64`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:69a8f9d0101fda57680f27c30ca9864f021d69a013d0d876c7f010296105365d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aeca41fe853b4af9d83ed356e1a338abb14a58e5645c3cb4a0756640886dc5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:58:32 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 05:58:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 05:58:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 05:58:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 05:58:53 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 05:58:53 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 05:58:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:58:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 05:58:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cf7cc4c20069210dbf0b03ab1fecd91e3d95b49c97e98cae7c670b28f0033`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf8eec65d1d720af4b0e901af92897e91841e174ac0414999f9174673879238`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca18ab8a4b82f11e9d159625a64a3b9923866ef0471b97f803fb09071405476`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 221.2 KB (221209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cce939bb90551e9a0f849ecdfad6c57fde68602a16c1a208154aaa6a5d2c49b`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230d405b698f37c531145e3d12d6c2db6858a39fb6b5bd2a61b1e6dec0a9f38f`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:c27d5fef225f76543118f6caa3acde60dc973cd24f4e33cb59090137381f2919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f1bbe21c527c03ef60714e2068bba645f66ce1506897d0529721db3b3db1262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 16:48:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 16:48:47 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 16:48:55 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 16:49:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 16:49:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 16:49:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 16:50:06 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 16:50:18 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 16:50:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 16:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 16:50:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942add97a5cb7e2c0420027c4ee428f7f8acc5c9ef7cf42145ae3e8d6169c280`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b04d7f19ebc8c84adc2f6cdf2f47f39edd6a40070b1a9fe013aa04bb19661`  
		Last Modified: Thu, 22 Oct 2020 16:51:11 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2284ab6cc6051b68486ca0c4ff330e9f9642af3f7edcb7b3f313e227c1dfbb81`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 219.0 KB (219035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d5eac542c6cee08a3a0540a86e200be7a8e7eacd50bfb2f6578d2dac35e894`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7c2df90d7b01b0207ff6e0e55de8177f67606a695437e5035e2c8b4e32a7ca`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:e0204033165a1ac587658e4dc23de07011115408c0d73ad47437a3e936d6bfce
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
$ docker pull spiped@sha256:e72efc9006cc88e74da18f8909e9a6d6cb80c024bc171e1de9a3bfa8082c7e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cd33bc57ff09ba0929eb9a1846e003f8ab8d35ac7f715f376161a9209fb7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:23:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 08:23:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 08:24:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 08:24:10 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 08:24:10 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 08:24:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2cfe9f1210973e807f22612ef44f79fdf4e9f1871ceb24da9c470ff4c6934a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebdc509a836b5478bba964b2f5c1712aa349a3761854c4f1193f580d18193`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2055abf7179bbbbaca992858134f6d59becb2b5cb2f516330f97082d7f4d272`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 211.4 KB (211432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a723ed90b1f6fc5a4bc245ba955d04306500cc3613e897f36a9246cb119a856`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8823b92e870bcac9a4efd674a3b7605e55d9877e47bb6d81c8d47f8e80d12a4a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:14cace5958bfa120cbf111e0c63cbaac02c7ae08cca3a8608d7f65c150a693bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6468ae1c5552249820a405840a8ca1b3217dd186e61222ca1df5425eb4b2ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:31:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:31:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:31:51 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:31:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:31:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:32:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:32:27 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:32:29 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:32:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:32:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:32:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acaaa89a9c32df4571254fbd79384a49e286b69f02ab7809109be9e080ac036`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd43fc49572c6e21badb3a526db0c4230a27c474dd5d4462f06ccfc6a96c45dd`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b785525c1135d90a9f438736d288ad7466404c9fdcc1b3dddb49668e94d281ed`  
		Last Modified: Thu, 22 Oct 2020 09:32:54 GMT  
		Size: 198.4 KB (198362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aaf1b15d6e46104f6566df081782ed2ac537c416d74e2d8820c3375d4de796`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64314cf23e502ff1d541e21714ebf47fd1719c58368cfd56ee7fc9c2b75c1397`  
		Last Modified: Thu, 22 Oct 2020 09:32:53 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:22e076d0704999df6954352a61322c7aff9e84102fb209dca8c67047f0f9ec55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12732fc9350260a757debfd45b04e105fa193198c820121c8fb104c75e4090e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:13:00 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:13:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:13:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:13:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:13:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:13:37 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:13:38 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:13:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ac12de1615c4fcf136e9caab1c56384e869fa371fb1aa91fa6a50584aede8`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49ab63c0d72d683d01704eb4d538cac06f6cccc649a32c793531090a507d758`  
		Last Modified: Thu, 22 Oct 2020 09:14:05 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7c72e8f699aad2c97e9e3116224f712f7a66a5bacec74cb4db459e9275f8d2`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 203.8 KB (203833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc60fd10df854316c0653b5c11cd733c7191a08efa7aa164d9d9e6cb76de12`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47396fd59d212f4a22fd40665e6647db1065fd9aebe2fe3394e3c973688ad64`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:69a8f9d0101fda57680f27c30ca9864f021d69a013d0d876c7f010296105365d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aeca41fe853b4af9d83ed356e1a338abb14a58e5645c3cb4a0756640886dc5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:58:32 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 05:58:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 05:58:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 05:58:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 05:58:53 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 05:58:53 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 05:58:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:58:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 05:58:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cf7cc4c20069210dbf0b03ab1fecd91e3d95b49c97e98cae7c670b28f0033`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf8eec65d1d720af4b0e901af92897e91841e174ac0414999f9174673879238`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca18ab8a4b82f11e9d159625a64a3b9923866ef0471b97f803fb09071405476`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 221.2 KB (221209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cce939bb90551e9a0f849ecdfad6c57fde68602a16c1a208154aaa6a5d2c49b`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230d405b698f37c531145e3d12d6c2db6858a39fb6b5bd2a61b1e6dec0a9f38f`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:c27d5fef225f76543118f6caa3acde60dc973cd24f4e33cb59090137381f2919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f1bbe21c527c03ef60714e2068bba645f66ce1506897d0529721db3b3db1262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 16:48:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 16:48:47 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 16:48:55 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 16:49:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 16:49:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 16:49:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 16:50:06 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 16:50:18 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 16:50:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 16:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 16:50:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942add97a5cb7e2c0420027c4ee428f7f8acc5c9ef7cf42145ae3e8d6169c280`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b04d7f19ebc8c84adc2f6cdf2f47f39edd6a40070b1a9fe013aa04bb19661`  
		Last Modified: Thu, 22 Oct 2020 16:51:11 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2284ab6cc6051b68486ca0c4ff330e9f9642af3f7edcb7b3f313e227c1dfbb81`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 219.0 KB (219035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d5eac542c6cee08a3a0540a86e200be7a8e7eacd50bfb2f6578d2dac35e894`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7c2df90d7b01b0207ff6e0e55de8177f67606a695437e5035e2c8b4e32a7ca`  
		Last Modified: Thu, 22 Oct 2020 16:51:12 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:c78456708f62dbca9c7a7374b72b91c5dc039f5ae31eee00c529101049a18044
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
$ docker pull spiped@sha256:db61217a4053f03c05b983f7d2722530fd82d6735e721311d7f90b17be40b713
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33488732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b062dbf1be23d35f8fb2e20a863861f260daee06fb4b84c4e4f7a669a6ecdbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:00:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:00:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:00:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:00:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 22:01:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 22:01:22 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 22:01:22 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 22:01:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 22:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 22:01:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43806a3fd3d362292aa4489b61228dc530d6820323d12f115ae0c4736e1b8ea`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80774235907721c9cd1bfff884ac7b597fe103ccb597a2563894bbc9a60bbb7`  
		Last Modified: Tue, 17 Nov 2020 22:02:11 GMT  
		Size: 1.8 MB (1821805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af91886a196e09e46584c37d8e2a8b40ab99d06f7096b4bed331ab4a63609ee`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 5.9 MB (5943582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d47aa91c0fe928301af1785740dd8890de723dff4c762a9c290e2b85178a1b`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a66f51280aa12fc65c7a03ae1bc737a260e3eb12d0c742a80d2757c48ba6cc`  
		Last Modified: Tue, 17 Nov 2020 22:02:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
