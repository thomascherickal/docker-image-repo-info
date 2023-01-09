<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1.6.2`](#spiped162)
-	[`spiped:1.6.2-alpine`](#spiped162-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:41cab1e6d2c73ed15bd839493a5123c7a3e2a86950c9c06b477a77a9e4506e36
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

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:85aa9ddb9cc29c6d20c055f292d7db6d1ad33a222a11df5258f1e8a0b1e59a29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37397558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f22fd9420e981a0333707ee5db302cfa3a098a848864f2ca60a62baca4f2b37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:54:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 12:54:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:54:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 12:54:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 12:54:54 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 12:54:54 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 12:54:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 12:54:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 12:54:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26577141cf487b2aa98d2458aa13f77d802a109fca8cef7ba468146855dd42b4`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa10d9cc47d642020b522e26303079e367fd8df0ac6fcc5ea75d5399368a7d1`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec94869c6e614592d5d3802a2189b4df8df5242b5a8f82156df2df36bf8c0c8`  
		Last Modified: Wed, 21 Dec 2022 12:55:13 GMT  
		Size: 6.0 MB (5997362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4594bece50255e034ef37f0889e173c77dda6d4880d51818cfd27028d92779`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4104a35ba18d4b5076c850a51535d87601f2ef3c8bf6227aea14d99479ef4a`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:797737cb5bd69499422edbd19d6f3d23defa2c13fd0c3e8b95e8136aebf0f548
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33929819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21051d375d17d94ec1a33c903f539b52d0850de47440a72590e9e11a27826e6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:49:08 GMT
ADD file:89f7788ae38bc6c172614b734ff10cba90c89ee09ca0f1acccc185c1bec630a1 in / 
# Wed, 21 Dec 2022 01:49:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 08:55:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 08:55:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 08:55:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 08:55:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 08:55:58 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 08:55:58 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 08:55:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 08:55:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 08:55:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6addfee759f2774f92392906ab5b50ba2f4a14314858c502e856f7d7de2a7e07`  
		Last Modified: Wed, 21 Dec 2022 01:54:03 GMT  
		Size: 28.9 MB (28898607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50b1fd90fa74ab502b27dc46132a9732ab610613b181393749bef0df327ee02`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c055b345bab52211392b90a1a0aff320a1e0384e19672944afbc8d06af1530a0`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d10c37400120401ef4814a61ac5d2c9c1b72833e086506ad1424c7fb2162c9`  
		Last Modified: Wed, 21 Dec 2022 08:56:17 GMT  
		Size: 5.0 MB (5028021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edc10919d2b92be136a90d05be541cdde53b3c0af84cf1aef64aa16e5ab2bd`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5769f6e8bedab011433d3aefbdbae84331a9a2445cc4741d4ac2d712860448b`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2935a5adbf6cbba0735da83eeeb853977391028b6401af92db6d4607e53c2a91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31310948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4aec4319565fe875a726a0c52970762c68fbaa3cb6cad85f349fd73f10de157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:25 GMT
ADD file:d62015d4eb206b606ae0bc76253de55403ede851d6fae0277e76bdaed196a848 in / 
# Wed, 21 Dec 2022 01:58:26 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:46:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 16:46:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:46:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 16:46:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:46:31 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 16:46:31 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 16:46:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 16:46:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8686edc9eb6f431c8c17a5eddc7bd38917d3b2d7835970d4fdb2ad0db464766`  
		Last Modified: Wed, 21 Dec 2022 02:05:08 GMT  
		Size: 26.6 MB (26559455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b14324de8263f9e18a002d36da7c9366d2b9c96b3757f5c65ef5e74d4f8d76f`  
		Last Modified: Wed, 21 Dec 2022 16:47:04 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2a0b64ddc8bb6e2d64533edacb8d09b9fc2cc16e5387ee91ddc0ebdc14c64a`  
		Last Modified: Wed, 21 Dec 2022 16:47:03 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fd3913f794254e4a2646dc43143f1ee08def7e335a42771d96d691c7ccf7ad`  
		Last Modified: Wed, 21 Dec 2022 16:47:05 GMT  
		Size: 4.7 MB (4748302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7917f26d003e09d377e722bc93613fd52ed891dc66b17343620cb3bd147b0fce`  
		Last Modified: Wed, 21 Dec 2022 16:47:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b90a2a54cef13a52a5841d0f5bc813505763391de1c34521dcecb59a0f2d5`  
		Last Modified: Wed, 21 Dec 2022 16:47:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:1bf3f1730b5aaee01a289f59e7f79b0e0a3479c6763e171a17f59e762c2da18f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35319723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9731ee95c4944b3118dab5498599a493f23011ba1bb08ee032362f7783de3155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 13:01:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 13:01:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 13:01:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 13:01:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 13:01:57 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 13:01:57 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 13:01:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 13:01:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 13:01:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5cdf62b0d2f1d74a6d834221174decc1ed41d84d8fc4959e940482d7fd1e00`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9250cba1edb63efc6479757971cd1416e33daa23490b29ff19563318f24a5943`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7304bd88756cf924a92abebc0daf7800432e751d1fbffab414dbdb6340446f8c`  
		Last Modified: Wed, 21 Dec 2022 13:02:16 GMT  
		Size: 5.3 MB (5271693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d60497a828497114eaa0a3338424a821a5fcb5af7332812ec56ced1bb22cae2`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6506c0929d8ff3c78a182e6288030da6027f27b87e5d35e1861223a213c39b`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:f92f3906350ef1e5fdec5bebb0e86a5951a47b9cee8edf66e63d2860089e58eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d712063ee68121b322cc91b7fc79a7217989af0cfbee58367991ba63e8237e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 07:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 07:10:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 07:10:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 07:10:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 07:10:56 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 07:10:57 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 07:10:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:10:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 07:11:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92616a842e988978699948189a1064084800d917ddf25e8cff4962e92db069db`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf401e3b7e18c0a67ecb197dfc8275544bc7b2b5d525f55f57c6753fe504b39`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b68fb58e59bed03e01d444721f61ceefbdac1d041a2a9be9df7857ccf3f71db`  
		Last Modified: Wed, 21 Dec 2022 07:11:28 GMT  
		Size: 7.9 MB (7889690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec61f24c1c2e5a6062318ccd0db4b6ce829d3bebfbef06a86279010ae5dbef1`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d833a289dac2b4a8b3d55f6a70e5854f01f1c90351c668e23ca28b9ce0ec4099`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:c32229c3b19cf590472dde0a8d6c70053a4810b55da01d920884b36b53d882d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54feacced6081f736e1c8de99d21837cdfacdac2fc00ef0e4b0655e21247effd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:10:32 GMT
ADD file:45a0ac3f00e914341df42a4d2a56b9081a224ee58e1167fb05ca87662d42f24c in / 
# Wed, 21 Dec 2022 01:10:37 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 23:23:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 23:23:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 23:23:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 23:25:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 23:25:29 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 23:25:31 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 23:25:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 23:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 23:25:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5410793baaff16536eff1e5ac655d98039bd44f581c42d6ceb254202d1196477`  
		Last Modified: Wed, 21 Dec 2022 01:18:42 GMT  
		Size: 29.6 MB (29619894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3fb8d064e54551314c575e324b8ec2552470c8c263b7470ec03df046460331`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 1.6 KB (1623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4888616d1b5b4132e4d3cd2f5420cc5bec1fd06285d0864bd7d56801f5b5360`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd0a4bc882e056eadcbd99493ef2278f3cab9fbcacd496e90d6c8a1d184f6b3`  
		Last Modified: Wed, 21 Dec 2022 23:26:04 GMT  
		Size: 5.7 MB (5705055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb879352f2d3c2393e5dcae50c0ec7b30cd64c3d6f167eb42c20056ccce2bff`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70b0b12bb3add98e6deb3af3872f6f5dbc039be3906abf750ffb34d1153754c`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:d68c58a419a4747edccb2d963fd7df44613a10325fa9b4b323c8f8f626b5bfae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41270795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bab744c022c6979cc8b0cdb02e9ab212343e25ea341f9bb5f75a7f0a7351379`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 14:49:00 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 14:49:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 14:49:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 14:49:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 14:49:47 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 14:49:48 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 14:49:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 14:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 14:49:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4e4f3672004cda084f3d622a6c179e4bc2e9b67824d8dcbf4908bd7bf78bef`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dd307ed8693f7f7f3282ad7a510c38f27e2414bf04e6f26cfe1a2157ca3330`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c31c5bcb8c26659926b1af7b0f277fc9734148dfea5164baf45cf8f733df2f0`  
		Last Modified: Wed, 21 Dec 2022 14:50:24 GMT  
		Size: 6.0 MB (5998788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1addfcb258ac143b8de980c0470fc8372184366c274c0762dbd3a6a37d273e`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82516a12e47c728931a2579797302a2a8ab0af04ed095de36287d7ac7d55d115`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:4c6277411e4798c460cb67e6aaaa050297047f02ca98578150d06bb7b8ab0cd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34820149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89166a98687be690072a0d2d3c54fcf3f36a6bc3e5fbdedca9cfd650b795385e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 04:44:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 04:44:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:44:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 04:45:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 04:45:07 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 04:45:08 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 04:45:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:45:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 04:45:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86a5dea122ea1383f781a97413d9ea3e808a0068037029f02bf74c67af93d3`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591956c3becaa4f0aa5492bda2c7558498f97c60ccf79b700858ee3fe3013ba9`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4fa0a653addc6672f3217593e893fd575d77c265c9527e521481005a266283`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 5.2 MB (5187128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc48ee754e31ec7edcf0f68cda3e18c45226c2d88b0ceb702c4963d5a0af6712`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a81f729da5c1c13fc42d3aebeb27638219ae5799e72543d6e7b058ca00ca516`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:4a120c25848829f0c9bc860ec77125ab86684dc349513f4866a86715fedc22ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:41cab1e6d2c73ed15bd839493a5123c7a3e2a86950c9c06b477a77a9e4506e36
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

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:85aa9ddb9cc29c6d20c055f292d7db6d1ad33a222a11df5258f1e8a0b1e59a29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37397558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f22fd9420e981a0333707ee5db302cfa3a098a848864f2ca60a62baca4f2b37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:54:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 12:54:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:54:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 12:54:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 12:54:54 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 12:54:54 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 12:54:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 12:54:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 12:54:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26577141cf487b2aa98d2458aa13f77d802a109fca8cef7ba468146855dd42b4`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa10d9cc47d642020b522e26303079e367fd8df0ac6fcc5ea75d5399368a7d1`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec94869c6e614592d5d3802a2189b4df8df5242b5a8f82156df2df36bf8c0c8`  
		Last Modified: Wed, 21 Dec 2022 12:55:13 GMT  
		Size: 6.0 MB (5997362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4594bece50255e034ef37f0889e173c77dda6d4880d51818cfd27028d92779`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4104a35ba18d4b5076c850a51535d87601f2ef3c8bf6227aea14d99479ef4a`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:797737cb5bd69499422edbd19d6f3d23defa2c13fd0c3e8b95e8136aebf0f548
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33929819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21051d375d17d94ec1a33c903f539b52d0850de47440a72590e9e11a27826e6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:49:08 GMT
ADD file:89f7788ae38bc6c172614b734ff10cba90c89ee09ca0f1acccc185c1bec630a1 in / 
# Wed, 21 Dec 2022 01:49:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 08:55:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 08:55:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 08:55:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 08:55:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 08:55:58 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 08:55:58 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 08:55:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 08:55:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 08:55:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6addfee759f2774f92392906ab5b50ba2f4a14314858c502e856f7d7de2a7e07`  
		Last Modified: Wed, 21 Dec 2022 01:54:03 GMT  
		Size: 28.9 MB (28898607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50b1fd90fa74ab502b27dc46132a9732ab610613b181393749bef0df327ee02`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c055b345bab52211392b90a1a0aff320a1e0384e19672944afbc8d06af1530a0`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d10c37400120401ef4814a61ac5d2c9c1b72833e086506ad1424c7fb2162c9`  
		Last Modified: Wed, 21 Dec 2022 08:56:17 GMT  
		Size: 5.0 MB (5028021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edc10919d2b92be136a90d05be541cdde53b3c0af84cf1aef64aa16e5ab2bd`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5769f6e8bedab011433d3aefbdbae84331a9a2445cc4741d4ac2d712860448b`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2935a5adbf6cbba0735da83eeeb853977391028b6401af92db6d4607e53c2a91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31310948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4aec4319565fe875a726a0c52970762c68fbaa3cb6cad85f349fd73f10de157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:25 GMT
ADD file:d62015d4eb206b606ae0bc76253de55403ede851d6fae0277e76bdaed196a848 in / 
# Wed, 21 Dec 2022 01:58:26 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:46:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 16:46:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:46:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 16:46:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:46:31 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 16:46:31 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 16:46:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 16:46:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8686edc9eb6f431c8c17a5eddc7bd38917d3b2d7835970d4fdb2ad0db464766`  
		Last Modified: Wed, 21 Dec 2022 02:05:08 GMT  
		Size: 26.6 MB (26559455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b14324de8263f9e18a002d36da7c9366d2b9c96b3757f5c65ef5e74d4f8d76f`  
		Last Modified: Wed, 21 Dec 2022 16:47:04 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2a0b64ddc8bb6e2d64533edacb8d09b9fc2cc16e5387ee91ddc0ebdc14c64a`  
		Last Modified: Wed, 21 Dec 2022 16:47:03 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fd3913f794254e4a2646dc43143f1ee08def7e335a42771d96d691c7ccf7ad`  
		Last Modified: Wed, 21 Dec 2022 16:47:05 GMT  
		Size: 4.7 MB (4748302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7917f26d003e09d377e722bc93613fd52ed891dc66b17343620cb3bd147b0fce`  
		Last Modified: Wed, 21 Dec 2022 16:47:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b90a2a54cef13a52a5841d0f5bc813505763391de1c34521dcecb59a0f2d5`  
		Last Modified: Wed, 21 Dec 2022 16:47:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:1bf3f1730b5aaee01a289f59e7f79b0e0a3479c6763e171a17f59e762c2da18f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35319723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9731ee95c4944b3118dab5498599a493f23011ba1bb08ee032362f7783de3155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 13:01:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 13:01:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 13:01:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 13:01:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 13:01:57 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 13:01:57 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 13:01:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 13:01:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 13:01:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5cdf62b0d2f1d74a6d834221174decc1ed41d84d8fc4959e940482d7fd1e00`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9250cba1edb63efc6479757971cd1416e33daa23490b29ff19563318f24a5943`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7304bd88756cf924a92abebc0daf7800432e751d1fbffab414dbdb6340446f8c`  
		Last Modified: Wed, 21 Dec 2022 13:02:16 GMT  
		Size: 5.3 MB (5271693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d60497a828497114eaa0a3338424a821a5fcb5af7332812ec56ced1bb22cae2`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6506c0929d8ff3c78a182e6288030da6027f27b87e5d35e1861223a213c39b`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:f92f3906350ef1e5fdec5bebb0e86a5951a47b9cee8edf66e63d2860089e58eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d712063ee68121b322cc91b7fc79a7217989af0cfbee58367991ba63e8237e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 07:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 07:10:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 07:10:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 07:10:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 07:10:56 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 07:10:57 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 07:10:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:10:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 07:11:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92616a842e988978699948189a1064084800d917ddf25e8cff4962e92db069db`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf401e3b7e18c0a67ecb197dfc8275544bc7b2b5d525f55f57c6753fe504b39`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b68fb58e59bed03e01d444721f61ceefbdac1d041a2a9be9df7857ccf3f71db`  
		Last Modified: Wed, 21 Dec 2022 07:11:28 GMT  
		Size: 7.9 MB (7889690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec61f24c1c2e5a6062318ccd0db4b6ce829d3bebfbef06a86279010ae5dbef1`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d833a289dac2b4a8b3d55f6a70e5854f01f1c90351c668e23ca28b9ce0ec4099`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:c32229c3b19cf590472dde0a8d6c70053a4810b55da01d920884b36b53d882d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54feacced6081f736e1c8de99d21837cdfacdac2fc00ef0e4b0655e21247effd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:10:32 GMT
ADD file:45a0ac3f00e914341df42a4d2a56b9081a224ee58e1167fb05ca87662d42f24c in / 
# Wed, 21 Dec 2022 01:10:37 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 23:23:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 23:23:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 23:23:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 23:25:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 23:25:29 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 23:25:31 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 23:25:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 23:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 23:25:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5410793baaff16536eff1e5ac655d98039bd44f581c42d6ceb254202d1196477`  
		Last Modified: Wed, 21 Dec 2022 01:18:42 GMT  
		Size: 29.6 MB (29619894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3fb8d064e54551314c575e324b8ec2552470c8c263b7470ec03df046460331`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 1.6 KB (1623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4888616d1b5b4132e4d3cd2f5420cc5bec1fd06285d0864bd7d56801f5b5360`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd0a4bc882e056eadcbd99493ef2278f3cab9fbcacd496e90d6c8a1d184f6b3`  
		Last Modified: Wed, 21 Dec 2022 23:26:04 GMT  
		Size: 5.7 MB (5705055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb879352f2d3c2393e5dcae50c0ec7b30cd64c3d6f167eb42c20056ccce2bff`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70b0b12bb3add98e6deb3af3872f6f5dbc039be3906abf750ffb34d1153754c`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:d68c58a419a4747edccb2d963fd7df44613a10325fa9b4b323c8f8f626b5bfae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41270795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bab744c022c6979cc8b0cdb02e9ab212343e25ea341f9bb5f75a7f0a7351379`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 14:49:00 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 14:49:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 14:49:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 14:49:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 14:49:47 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 14:49:48 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 14:49:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 14:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 14:49:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4e4f3672004cda084f3d622a6c179e4bc2e9b67824d8dcbf4908bd7bf78bef`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dd307ed8693f7f7f3282ad7a510c38f27e2414bf04e6f26cfe1a2157ca3330`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c31c5bcb8c26659926b1af7b0f277fc9734148dfea5164baf45cf8f733df2f0`  
		Last Modified: Wed, 21 Dec 2022 14:50:24 GMT  
		Size: 6.0 MB (5998788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1addfcb258ac143b8de980c0470fc8372184366c274c0762dbd3a6a37d273e`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82516a12e47c728931a2579797302a2a8ab0af04ed095de36287d7ac7d55d115`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:4c6277411e4798c460cb67e6aaaa050297047f02ca98578150d06bb7b8ab0cd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34820149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89166a98687be690072a0d2d3c54fcf3f36a6bc3e5fbdedca9cfd650b795385e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 04:44:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 04:44:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:44:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 04:45:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 04:45:07 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 04:45:08 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 04:45:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:45:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 04:45:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86a5dea122ea1383f781a97413d9ea3e808a0068037029f02bf74c67af93d3`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591956c3becaa4f0aa5492bda2c7558498f97c60ccf79b700858ee3fe3013ba9`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4fa0a653addc6672f3217593e893fd575d77c265c9527e521481005a266283`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 5.2 MB (5187128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc48ee754e31ec7edcf0f68cda3e18c45226c2d88b0ceb702c4963d5a0af6712`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a81f729da5c1c13fc42d3aebeb27638219ae5799e72543d6e7b058ca00ca516`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:4a120c25848829f0c9bc860ec77125ab86684dc349513f4866a86715fedc22ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:41cab1e6d2c73ed15bd839493a5123c7a3e2a86950c9c06b477a77a9e4506e36
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

### `spiped:1.6.2` - linux; amd64

```console
$ docker pull spiped@sha256:85aa9ddb9cc29c6d20c055f292d7db6d1ad33a222a11df5258f1e8a0b1e59a29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37397558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f22fd9420e981a0333707ee5db302cfa3a098a848864f2ca60a62baca4f2b37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:54:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 12:54:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:54:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 12:54:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 12:54:54 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 12:54:54 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 12:54:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 12:54:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 12:54:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26577141cf487b2aa98d2458aa13f77d802a109fca8cef7ba468146855dd42b4`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa10d9cc47d642020b522e26303079e367fd8df0ac6fcc5ea75d5399368a7d1`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec94869c6e614592d5d3802a2189b4df8df5242b5a8f82156df2df36bf8c0c8`  
		Last Modified: Wed, 21 Dec 2022 12:55:13 GMT  
		Size: 6.0 MB (5997362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4594bece50255e034ef37f0889e173c77dda6d4880d51818cfd27028d92779`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4104a35ba18d4b5076c850a51535d87601f2ef3c8bf6227aea14d99479ef4a`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:797737cb5bd69499422edbd19d6f3d23defa2c13fd0c3e8b95e8136aebf0f548
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33929819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21051d375d17d94ec1a33c903f539b52d0850de47440a72590e9e11a27826e6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:49:08 GMT
ADD file:89f7788ae38bc6c172614b734ff10cba90c89ee09ca0f1acccc185c1bec630a1 in / 
# Wed, 21 Dec 2022 01:49:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 08:55:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 08:55:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 08:55:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 08:55:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 08:55:58 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 08:55:58 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 08:55:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 08:55:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 08:55:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6addfee759f2774f92392906ab5b50ba2f4a14314858c502e856f7d7de2a7e07`  
		Last Modified: Wed, 21 Dec 2022 01:54:03 GMT  
		Size: 28.9 MB (28898607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50b1fd90fa74ab502b27dc46132a9732ab610613b181393749bef0df327ee02`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c055b345bab52211392b90a1a0aff320a1e0384e19672944afbc8d06af1530a0`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d10c37400120401ef4814a61ac5d2c9c1b72833e086506ad1424c7fb2162c9`  
		Last Modified: Wed, 21 Dec 2022 08:56:17 GMT  
		Size: 5.0 MB (5028021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edc10919d2b92be136a90d05be541cdde53b3c0af84cf1aef64aa16e5ab2bd`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5769f6e8bedab011433d3aefbdbae84331a9a2445cc4741d4ac2d712860448b`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2935a5adbf6cbba0735da83eeeb853977391028b6401af92db6d4607e53c2a91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31310948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4aec4319565fe875a726a0c52970762c68fbaa3cb6cad85f349fd73f10de157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:25 GMT
ADD file:d62015d4eb206b606ae0bc76253de55403ede851d6fae0277e76bdaed196a848 in / 
# Wed, 21 Dec 2022 01:58:26 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:46:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 16:46:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:46:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 16:46:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:46:31 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 16:46:31 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 16:46:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 16:46:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8686edc9eb6f431c8c17a5eddc7bd38917d3b2d7835970d4fdb2ad0db464766`  
		Last Modified: Wed, 21 Dec 2022 02:05:08 GMT  
		Size: 26.6 MB (26559455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b14324de8263f9e18a002d36da7c9366d2b9c96b3757f5c65ef5e74d4f8d76f`  
		Last Modified: Wed, 21 Dec 2022 16:47:04 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2a0b64ddc8bb6e2d64533edacb8d09b9fc2cc16e5387ee91ddc0ebdc14c64a`  
		Last Modified: Wed, 21 Dec 2022 16:47:03 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fd3913f794254e4a2646dc43143f1ee08def7e335a42771d96d691c7ccf7ad`  
		Last Modified: Wed, 21 Dec 2022 16:47:05 GMT  
		Size: 4.7 MB (4748302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7917f26d003e09d377e722bc93613fd52ed891dc66b17343620cb3bd147b0fce`  
		Last Modified: Wed, 21 Dec 2022 16:47:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b90a2a54cef13a52a5841d0f5bc813505763391de1c34521dcecb59a0f2d5`  
		Last Modified: Wed, 21 Dec 2022 16:47:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:1bf3f1730b5aaee01a289f59e7f79b0e0a3479c6763e171a17f59e762c2da18f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35319723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9731ee95c4944b3118dab5498599a493f23011ba1bb08ee032362f7783de3155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 13:01:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 13:01:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 13:01:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 13:01:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 13:01:57 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 13:01:57 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 13:01:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 13:01:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 13:01:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5cdf62b0d2f1d74a6d834221174decc1ed41d84d8fc4959e940482d7fd1e00`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9250cba1edb63efc6479757971cd1416e33daa23490b29ff19563318f24a5943`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7304bd88756cf924a92abebc0daf7800432e751d1fbffab414dbdb6340446f8c`  
		Last Modified: Wed, 21 Dec 2022 13:02:16 GMT  
		Size: 5.3 MB (5271693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d60497a828497114eaa0a3338424a821a5fcb5af7332812ec56ced1bb22cae2`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6506c0929d8ff3c78a182e6288030da6027f27b87e5d35e1861223a213c39b`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:f92f3906350ef1e5fdec5bebb0e86a5951a47b9cee8edf66e63d2860089e58eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d712063ee68121b322cc91b7fc79a7217989af0cfbee58367991ba63e8237e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 07:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 07:10:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 07:10:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 07:10:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 07:10:56 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 07:10:57 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 07:10:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:10:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 07:11:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92616a842e988978699948189a1064084800d917ddf25e8cff4962e92db069db`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf401e3b7e18c0a67ecb197dfc8275544bc7b2b5d525f55f57c6753fe504b39`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b68fb58e59bed03e01d444721f61ceefbdac1d041a2a9be9df7857ccf3f71db`  
		Last Modified: Wed, 21 Dec 2022 07:11:28 GMT  
		Size: 7.9 MB (7889690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec61f24c1c2e5a6062318ccd0db4b6ce829d3bebfbef06a86279010ae5dbef1`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d833a289dac2b4a8b3d55f6a70e5854f01f1c90351c668e23ca28b9ce0ec4099`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:c32229c3b19cf590472dde0a8d6c70053a4810b55da01d920884b36b53d882d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54feacced6081f736e1c8de99d21837cdfacdac2fc00ef0e4b0655e21247effd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:10:32 GMT
ADD file:45a0ac3f00e914341df42a4d2a56b9081a224ee58e1167fb05ca87662d42f24c in / 
# Wed, 21 Dec 2022 01:10:37 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 23:23:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 23:23:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 23:23:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 23:25:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 23:25:29 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 23:25:31 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 23:25:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 23:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 23:25:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5410793baaff16536eff1e5ac655d98039bd44f581c42d6ceb254202d1196477`  
		Last Modified: Wed, 21 Dec 2022 01:18:42 GMT  
		Size: 29.6 MB (29619894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3fb8d064e54551314c575e324b8ec2552470c8c263b7470ec03df046460331`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 1.6 KB (1623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4888616d1b5b4132e4d3cd2f5420cc5bec1fd06285d0864bd7d56801f5b5360`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd0a4bc882e056eadcbd99493ef2278f3cab9fbcacd496e90d6c8a1d184f6b3`  
		Last Modified: Wed, 21 Dec 2022 23:26:04 GMT  
		Size: 5.7 MB (5705055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb879352f2d3c2393e5dcae50c0ec7b30cd64c3d6f167eb42c20056ccce2bff`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70b0b12bb3add98e6deb3af3872f6f5dbc039be3906abf750ffb34d1153754c`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:d68c58a419a4747edccb2d963fd7df44613a10325fa9b4b323c8f8f626b5bfae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41270795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bab744c022c6979cc8b0cdb02e9ab212343e25ea341f9bb5f75a7f0a7351379`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 14:49:00 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 14:49:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 14:49:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 14:49:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 14:49:47 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 14:49:48 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 14:49:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 14:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 14:49:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4e4f3672004cda084f3d622a6c179e4bc2e9b67824d8dcbf4908bd7bf78bef`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dd307ed8693f7f7f3282ad7a510c38f27e2414bf04e6f26cfe1a2157ca3330`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c31c5bcb8c26659926b1af7b0f277fc9734148dfea5164baf45cf8f733df2f0`  
		Last Modified: Wed, 21 Dec 2022 14:50:24 GMT  
		Size: 6.0 MB (5998788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1addfcb258ac143b8de980c0470fc8372184366c274c0762dbd3a6a37d273e`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82516a12e47c728931a2579797302a2a8ab0af04ed095de36287d7ac7d55d115`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:4c6277411e4798c460cb67e6aaaa050297047f02ca98578150d06bb7b8ab0cd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34820149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89166a98687be690072a0d2d3c54fcf3f36a6bc3e5fbdedca9cfd650b795385e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 04:44:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 04:44:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:44:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 04:45:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 04:45:07 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 04:45:08 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 04:45:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:45:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 04:45:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86a5dea122ea1383f781a97413d9ea3e808a0068037029f02bf74c67af93d3`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591956c3becaa4f0aa5492bda2c7558498f97c60ccf79b700858ee3fe3013ba9`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4fa0a653addc6672f3217593e893fd575d77c265c9527e521481005a266283`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 5.2 MB (5187128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc48ee754e31ec7edcf0f68cda3e18c45226c2d88b0ceb702c4963d5a0af6712`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a81f729da5c1c13fc42d3aebeb27638219ae5799e72543d6e7b058ca00ca516`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:4a120c25848829f0c9bc860ec77125ab86684dc349513f4866a86715fedc22ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.2-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:4a120c25848829f0c9bc860ec77125ab86684dc349513f4866a86715fedc22ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:41cab1e6d2c73ed15bd839493a5123c7a3e2a86950c9c06b477a77a9e4506e36
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

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:85aa9ddb9cc29c6d20c055f292d7db6d1ad33a222a11df5258f1e8a0b1e59a29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37397558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f22fd9420e981a0333707ee5db302cfa3a098a848864f2ca60a62baca4f2b37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:54:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 12:54:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:54:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 12:54:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 12:54:54 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 12:54:54 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 12:54:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 12:54:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 12:54:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26577141cf487b2aa98d2458aa13f77d802a109fca8cef7ba468146855dd42b4`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa10d9cc47d642020b522e26303079e367fd8df0ac6fcc5ea75d5399368a7d1`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec94869c6e614592d5d3802a2189b4df8df5242b5a8f82156df2df36bf8c0c8`  
		Last Modified: Wed, 21 Dec 2022 12:55:13 GMT  
		Size: 6.0 MB (5997362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4594bece50255e034ef37f0889e173c77dda6d4880d51818cfd27028d92779`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4104a35ba18d4b5076c850a51535d87601f2ef3c8bf6227aea14d99479ef4a`  
		Last Modified: Wed, 21 Dec 2022 12:55:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:797737cb5bd69499422edbd19d6f3d23defa2c13fd0c3e8b95e8136aebf0f548
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33929819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21051d375d17d94ec1a33c903f539b52d0850de47440a72590e9e11a27826e6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:49:08 GMT
ADD file:89f7788ae38bc6c172614b734ff10cba90c89ee09ca0f1acccc185c1bec630a1 in / 
# Wed, 21 Dec 2022 01:49:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 08:55:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 08:55:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 08:55:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 08:55:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 08:55:58 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 08:55:58 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 08:55:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 08:55:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 08:55:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6addfee759f2774f92392906ab5b50ba2f4a14314858c502e856f7d7de2a7e07`  
		Last Modified: Wed, 21 Dec 2022 01:54:03 GMT  
		Size: 28.9 MB (28898607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50b1fd90fa74ab502b27dc46132a9732ab610613b181393749bef0df327ee02`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c055b345bab52211392b90a1a0aff320a1e0384e19672944afbc8d06af1530a0`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d10c37400120401ef4814a61ac5d2c9c1b72833e086506ad1424c7fb2162c9`  
		Last Modified: Wed, 21 Dec 2022 08:56:17 GMT  
		Size: 5.0 MB (5028021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edc10919d2b92be136a90d05be541cdde53b3c0af84cf1aef64aa16e5ab2bd`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5769f6e8bedab011433d3aefbdbae84331a9a2445cc4741d4ac2d712860448b`  
		Last Modified: Wed, 21 Dec 2022 08:56:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2935a5adbf6cbba0735da83eeeb853977391028b6401af92db6d4607e53c2a91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31310948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4aec4319565fe875a726a0c52970762c68fbaa3cb6cad85f349fd73f10de157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:25 GMT
ADD file:d62015d4eb206b606ae0bc76253de55403ede851d6fae0277e76bdaed196a848 in / 
# Wed, 21 Dec 2022 01:58:26 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:46:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 16:46:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:46:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 16:46:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:46:31 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 16:46:31 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 16:46:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 16:46:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8686edc9eb6f431c8c17a5eddc7bd38917d3b2d7835970d4fdb2ad0db464766`  
		Last Modified: Wed, 21 Dec 2022 02:05:08 GMT  
		Size: 26.6 MB (26559455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b14324de8263f9e18a002d36da7c9366d2b9c96b3757f5c65ef5e74d4f8d76f`  
		Last Modified: Wed, 21 Dec 2022 16:47:04 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2a0b64ddc8bb6e2d64533edacb8d09b9fc2cc16e5387ee91ddc0ebdc14c64a`  
		Last Modified: Wed, 21 Dec 2022 16:47:03 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fd3913f794254e4a2646dc43143f1ee08def7e335a42771d96d691c7ccf7ad`  
		Last Modified: Wed, 21 Dec 2022 16:47:05 GMT  
		Size: 4.7 MB (4748302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7917f26d003e09d377e722bc93613fd52ed891dc66b17343620cb3bd147b0fce`  
		Last Modified: Wed, 21 Dec 2022 16:47:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b90a2a54cef13a52a5841d0f5bc813505763391de1c34521dcecb59a0f2d5`  
		Last Modified: Wed, 21 Dec 2022 16:47:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:1bf3f1730b5aaee01a289f59e7f79b0e0a3479c6763e171a17f59e762c2da18f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35319723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9731ee95c4944b3118dab5498599a493f23011ba1bb08ee032362f7783de3155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 13:01:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 13:01:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 13:01:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 13:01:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 13:01:57 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 13:01:57 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 13:01:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 13:01:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 13:01:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5cdf62b0d2f1d74a6d834221174decc1ed41d84d8fc4959e940482d7fd1e00`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9250cba1edb63efc6479757971cd1416e33daa23490b29ff19563318f24a5943`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7304bd88756cf924a92abebc0daf7800432e751d1fbffab414dbdb6340446f8c`  
		Last Modified: Wed, 21 Dec 2022 13:02:16 GMT  
		Size: 5.3 MB (5271693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d60497a828497114eaa0a3338424a821a5fcb5af7332812ec56ced1bb22cae2`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6506c0929d8ff3c78a182e6288030da6027f27b87e5d35e1861223a213c39b`  
		Last Modified: Wed, 21 Dec 2022 13:02:15 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:f92f3906350ef1e5fdec5bebb0e86a5951a47b9cee8edf66e63d2860089e58eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d712063ee68121b322cc91b7fc79a7217989af0cfbee58367991ba63e8237e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 07:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 07:10:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 07:10:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 07:10:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 07:10:56 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 07:10:57 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 07:10:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:10:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 07:11:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92616a842e988978699948189a1064084800d917ddf25e8cff4962e92db069db`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf401e3b7e18c0a67ecb197dfc8275544bc7b2b5d525f55f57c6753fe504b39`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b68fb58e59bed03e01d444721f61ceefbdac1d041a2a9be9df7857ccf3f71db`  
		Last Modified: Wed, 21 Dec 2022 07:11:28 GMT  
		Size: 7.9 MB (7889690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec61f24c1c2e5a6062318ccd0db4b6ce829d3bebfbef06a86279010ae5dbef1`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d833a289dac2b4a8b3d55f6a70e5854f01f1c90351c668e23ca28b9ce0ec4099`  
		Last Modified: Wed, 21 Dec 2022 07:11:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:c32229c3b19cf590472dde0a8d6c70053a4810b55da01d920884b36b53d882d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54feacced6081f736e1c8de99d21837cdfacdac2fc00ef0e4b0655e21247effd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:10:32 GMT
ADD file:45a0ac3f00e914341df42a4d2a56b9081a224ee58e1167fb05ca87662d42f24c in / 
# Wed, 21 Dec 2022 01:10:37 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 23:23:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 23:23:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 23:23:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 23:25:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 23:25:29 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 23:25:31 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 23:25:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 23:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 23:25:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5410793baaff16536eff1e5ac655d98039bd44f581c42d6ceb254202d1196477`  
		Last Modified: Wed, 21 Dec 2022 01:18:42 GMT  
		Size: 29.6 MB (29619894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3fb8d064e54551314c575e324b8ec2552470c8c263b7470ec03df046460331`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 1.6 KB (1623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4888616d1b5b4132e4d3cd2f5420cc5bec1fd06285d0864bd7d56801f5b5360`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd0a4bc882e056eadcbd99493ef2278f3cab9fbcacd496e90d6c8a1d184f6b3`  
		Last Modified: Wed, 21 Dec 2022 23:26:04 GMT  
		Size: 5.7 MB (5705055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb879352f2d3c2393e5dcae50c0ec7b30cd64c3d6f167eb42c20056ccce2bff`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70b0b12bb3add98e6deb3af3872f6f5dbc039be3906abf750ffb34d1153754c`  
		Last Modified: Wed, 21 Dec 2022 23:25:59 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:d68c58a419a4747edccb2d963fd7df44613a10325fa9b4b323c8f8f626b5bfae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41270795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bab744c022c6979cc8b0cdb02e9ab212343e25ea341f9bb5f75a7f0a7351379`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 14:49:00 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 14:49:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 14:49:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 14:49:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 14:49:47 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 14:49:48 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 14:49:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 14:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 14:49:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4e4f3672004cda084f3d622a6c179e4bc2e9b67824d8dcbf4908bd7bf78bef`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dd307ed8693f7f7f3282ad7a510c38f27e2414bf04e6f26cfe1a2157ca3330`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c31c5bcb8c26659926b1af7b0f277fc9734148dfea5164baf45cf8f733df2f0`  
		Last Modified: Wed, 21 Dec 2022 14:50:24 GMT  
		Size: 6.0 MB (5998788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1addfcb258ac143b8de980c0470fc8372184366c274c0762dbd3a6a37d273e`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82516a12e47c728931a2579797302a2a8ab0af04ed095de36287d7ac7d55d115`  
		Last Modified: Wed, 21 Dec 2022 14:50:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:4c6277411e4798c460cb67e6aaaa050297047f02ca98578150d06bb7b8ab0cd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34820149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89166a98687be690072a0d2d3c54fcf3f36a6bc3e5fbdedca9cfd650b795385e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 04:44:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 21 Dec 2022 04:44:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:44:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 21 Dec 2022 04:45:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 04:45:07 GMT
VOLUME [/spiped]
# Wed, 21 Dec 2022 04:45:08 GMT
WORKDIR /spiped
# Wed, 21 Dec 2022 04:45:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:45:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 04:45:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86a5dea122ea1383f781a97413d9ea3e808a0068037029f02bf74c67af93d3`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591956c3becaa4f0aa5492bda2c7558498f97c60ccf79b700858ee3fe3013ba9`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4fa0a653addc6672f3217593e893fd575d77c265c9527e521481005a266283`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 5.2 MB (5187128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc48ee754e31ec7edcf0f68cda3e18c45226c2d88b0ceb702c4963d5a0af6712`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a81f729da5c1c13fc42d3aebeb27638219ae5799e72543d6e7b058ca00ca516`  
		Last Modified: Wed, 21 Dec 2022 04:45:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
