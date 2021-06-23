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
$ docker pull spiped@sha256:71c26b5882a1b12cad71178d31d4d15dd3d3fe3252014611f5adc879192d2e72
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
$ docker pull spiped@sha256:deca629e565a472791c066c34d81b0536d6e3393ebbb45ede224ba9e33fac0cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36314034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cfebea6aa229524e4eb8300c3f8a158570052fa02ec5efe7973e020741adc55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:52:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 17:52:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:52:38 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 17:53:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 17:53:06 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 17:53:06 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 17:53:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 17:53:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 17:53:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9436548b6b61a5565bdee4208eb7b277f1bd36cf5416483a730e4a1ea42be97`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af92bc2edfa15c30f1fc1536102eba6dc3369e7fddc435b31c63a356e7289732`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 2.1 MB (2128557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6c58cd98ed2868a2430518c3d20baa273bd886c4b8d1578ec65631aed39497`  
		Last Modified: Wed, 23 Jun 2021 17:53:41 GMT  
		Size: 7.0 MB (7037418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30630ff604ee0f5b793f4d6dcfb3156992bb4a226f75d41213a6ea23e7057e58`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ef7cd63ea6b2f85ed3540b09e2f8f4a31a4a20ecebd88135002f0d29b2533f`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a68f5767e0f485387c46fe28df422acf740e8831955651e7b6ca916ab3f52071
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32200613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8343f39cdca8596668b92bebbdad64930181c27e383d37c1a6943182e202fb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:12:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 05:12:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:12:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 05:13:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 05:13:46 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 05:13:46 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 05:13:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:13:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:13:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7bbdd9ad10264bd31c073aa67f6e04e014d25a92fa44b8cdc85a66b49d3e`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95a6bcf02d0c380ceb6339aa314e5cc271870d64c1c131c8d1a89d5aedbf371`  
		Last Modified: Wed, 23 Jun 2021 05:14:21 GMT  
		Size: 1.8 MB (1839313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dec4e8ba1333802d705cfedbbb7d57ef3407102ba371ee5b3afeeb3b6a4906`  
		Last Modified: Wed, 23 Jun 2021 05:14:25 GMT  
		Size: 5.5 MB (5480145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e797035b745745c7aabb74f5187811477900b08d4de77418d1c4b44ae3642a9`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50aa5ce3a5b802a562d044c299aafdec277da107220ec1dd1ebdceeef4395c5a`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8f3dcc5672e08027b33653e7999eab3091a08a8cb2911f42832543451907ec22
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1835331fef38be27cb80bf4a7f5b084d008b3fbf5425bc9d9d191e76d3ec10b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 20:59:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Jun 2021 20:59:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Jun 2021 20:59:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 16 Jun 2021 21:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Jun 2021 21:00:20 GMT
VOLUME [/spiped]
# Wed, 16 Jun 2021 21:00:20 GMT
WORKDIR /spiped
# Wed, 16 Jun 2021 21:00:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Jun 2021 21:00:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 21:00:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a138a3599035cdb1344595fc1e373195d5502ba9ad2b19dded9fc9bcadf76472`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecaf1d52ed2cd4ab43df4821c429206a8d2ced2f9e20be6e12008770d746d39d`  
		Last Modified: Wed, 16 Jun 2021 21:01:10 GMT  
		Size: 1.8 MB (1759508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f53a999ed2e7f6391b4db1a00ceb30dd0b554f1258b81d7ae232af4989c0aa3`  
		Last Modified: Wed, 16 Jun 2021 21:01:10 GMT  
		Size: 5.3 MB (5285557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66830d84d7cb6aedf6f77790563281d0c2b333fbbe9e3838f92ac9e9a2faead`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de1593245c38600bbc3eded9fb1ed99e58b680e984c27b60e73689d11446712`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ac6f7688ea32f8a2f442fe68855114b8562caf896a3357d0615cc30b5d2168f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33830362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7838646f1ed01bb14846176266e7f79452000256d1ee2fc64ffa49d1cc32bc45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 04:44:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 04:44:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 04:44:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 04:44:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 04:44:48 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 04:44:48 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 04:44:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 04:44:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 04:44:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba75a48871843ec90c5653d7a68d32d4782e02661ed505a4aac4ba2e6b162b1c`  
		Last Modified: Wed, 23 Jun 2021 04:45:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78779b3a1ea7be051ec8a444920361dd44691bd2598360f19fcdea7b6cb8a5f`  
		Last Modified: Wed, 23 Jun 2021 04:45:25 GMT  
		Size: 2.0 MB (2007837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9e473ed57b4a2a7f6c6e0c3691bac286e4d62776d948af11510ba7e0be4798`  
		Last Modified: Wed, 23 Jun 2021 04:45:26 GMT  
		Size: 5.9 MB (5905325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0471736cf2872e3b8fcc5cda063cef30d8ddc0cf493dda64f0e46cc192c6fa13`  
		Last Modified: Wed, 23 Jun 2021 04:45:25 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9a2c649b4c4c03bcfaf26b19aa23ee9c4a47913c519b5d88525967c961d9c5`  
		Last Modified: Wed, 23 Jun 2021 04:45:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:c626e5813307c4a522253701a8d10044490c5089fc1028865064aba56b79a567
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41565721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d520e0fa299bb26925db9d358ba485a922493b570445e869fe9cbc2c58a7a28a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 05:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 05:25:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 05:25:44 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 05:25:44 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 05:25:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:25:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:25:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a64acf577cc0906169a6fa1d1f41dd113b4cc5d2b0c8a3abb5674bb67a0c`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fe45b208cc8a9347120d3a18375f5bf334cde361e3d200c6cc2bfcd4e434c4`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 2.1 MB (2132634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d718789ca722dbc6e8352f0995209e18d785aab7390970c8fa4ffb85f633a704`  
		Last Modified: Wed, 23 Jun 2021 05:26:30 GMT  
		Size: 11.6 MB (11633477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d07737683dbbe7090182a8b646edec35d04531fc2c86a7f16512be098c6da6b`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4226fc02e39ef6661fe88338e9310db680d285e76408908cca7423c191625554`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:f8f7c8d549f49ae5784c026f95e0f1c34050e2f2379583f963386ee6a0cb4269
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33944242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:706e105af193dd6f9cfa952b76493ca2ba0096fe4c9268215b98027fbcc56f69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:29 GMT
ADD file:ca8422268fc66c67d19fd3a33a14a9bd6280ef21404677767ffd561a8ecf6724 in / 
# Wed, 23 Jun 2021 00:09:30 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:32:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 01:32:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 01:32:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 01:33:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:33:51 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 01:33:51 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 01:33:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 01:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 01:33:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4b9d1870c33c63bfde89c401b4af9582fbbff99d4036171a7a456706bf805d6d`  
		Last Modified: Wed, 23 Jun 2021 00:15:49 GMT  
		Size: 25.8 MB (25812890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b885417e0bed54626f847700fe119413544e07f53c9499064e4abb845490d9e`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d953da28b94c0e3b1a5834ae8fe31286237bbe9e3e71baad6edaef250f76e1`  
		Last Modified: Wed, 23 Jun 2021 01:34:19 GMT  
		Size: 1.7 MB (1712456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f20808768a5d40a26c1798479f76bf9064479a905b35f2d456cda0965d0bd8`  
		Last Modified: Wed, 23 Jun 2021 01:34:23 GMT  
		Size: 6.4 MB (6416722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b761e90f141aed8e640a25f68de1ed7052106a07ddf39cccd72dfe435b327802`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834563460305f4d062830ddecdb6f066e97e325f99acc8993a775bb7d322e682`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:4b249d499e7803150d5e0bab261950fc32089f5d19ad4ac725ce45b11e671eec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39524958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:662d5d6adaafe8261a7658051c3b5d8aee9100038f6b8d1ebb0b9fb17c52dc08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:20:36 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 06:21:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:21:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 06:24:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 06:24:12 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 06:24:16 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 06:24:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 06:24:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 06:24:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191c3937be8dbf43a8cfe50ad1a13e2dfaa99ea305bc8737627f6c4287d96249`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f610226f8d0550f8b920d027e63c3d5893fb9dbd9b251c1ef4c5a74d7c7af6ec`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 2.2 MB (2225166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ccf30cf2ac919705de54736fa518e3ebb3616e369b14484a125a2ad199597d`  
		Last Modified: Wed, 23 Jun 2021 06:26:41 GMT  
		Size: 6.7 MB (6743950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242cd2a18a0f522beb5fe1b8c192dd53c4f26f1f7c3822de8844af8ca0147a80`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73fc146b40b720705bfdf9cb0e0021348650da2a65afd9422b16bae5808ff2c`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:f7dc97ece5b5e4d70543bc74530ef4deb589f4defd2da77a771256e224f5841b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33528623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25b2527cb8f7e7c6e56a036a318afecae66b8a8327a19682c3904a340ca1a91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:28 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Tue, 22 Jun 2021 23:42:29 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:07:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 07:07:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:07:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 07:07:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 07:07:41 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 07:07:41 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 07:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:07:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:07:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ce76b947c34bd5af41d4870addb2699c4d0efb8a49c56af6a652c597b57376`  
		Last Modified: Wed, 23 Jun 2021 07:08:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451210b67a054c152e290b9fb707533662c85beadc1f9b1ebea5646f8af43c61`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 1.8 MB (1822020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d555c923d315711ae231e90d1cc857f4b3b6e7262c4c5bed071c33d2838d30da`  
		Last Modified: Wed, 23 Jun 2021 07:08:13 GMT  
		Size: 5.9 MB (5943675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520d76ccbffa39f96280eb068ed865face7fd9ad86300ba6018764061c57b0d2`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadd101ff04664820ade42807681d9e370f5109c372f19eaca4aac8e6c666eaf`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:b611f87cb8a8b2e94c240963e034606320ee732a29c0de5f7ee6bdd32f1427db
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
$ docker pull spiped@sha256:91c1773cab1581d76d4d48e8b17a155fdf6fa54339e449958132b7ab0e664b7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3324815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5620d28ab14686bc056b383ca94e121a1961a59dfa98a9a4e24992d49ccaf583`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:13:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 11:13:44 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 11:13:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 16 Jun 2021 11:14:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 16 Jun 2021 11:14:01 GMT
VOLUME [/spiped]
# Wed, 16 Jun 2021 11:14:01 GMT
WORKDIR /spiped
# Wed, 16 Jun 2021 11:14:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:14:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:14:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be0802b4de23117d6b04cc1a7237f151ac257b9b6ae94c41543add13a721211`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1598d38937e859a5682a8b4222572712c05ed3cd91911fc2b0402c4d3610bd1f`  
		Last Modified: Wed, 16 Jun 2021 11:14:50 GMT  
		Size: 7.1 KB (7060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93daa195a9f9aae8df4b499ba4d793860c0aab39686330ecc6a410b8f7bf58e6`  
		Last Modified: Wed, 16 Jun 2021 11:14:50 GMT  
		Size: 604.0 KB (603997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011245e695623945bea926d3f62bed142c2caf7f2ff394931342b395e9bf2c6a`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a47c9f4da08454bed52a6c03bb7e750ec3ad498ed63773d6e46ddaccca505a5`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:71c26b5882a1b12cad71178d31d4d15dd3d3fe3252014611f5adc879192d2e72
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
$ docker pull spiped@sha256:deca629e565a472791c066c34d81b0536d6e3393ebbb45ede224ba9e33fac0cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36314034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cfebea6aa229524e4eb8300c3f8a158570052fa02ec5efe7973e020741adc55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:52:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 17:52:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:52:38 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 17:53:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 17:53:06 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 17:53:06 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 17:53:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 17:53:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 17:53:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9436548b6b61a5565bdee4208eb7b277f1bd36cf5416483a730e4a1ea42be97`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af92bc2edfa15c30f1fc1536102eba6dc3369e7fddc435b31c63a356e7289732`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 2.1 MB (2128557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6c58cd98ed2868a2430518c3d20baa273bd886c4b8d1578ec65631aed39497`  
		Last Modified: Wed, 23 Jun 2021 17:53:41 GMT  
		Size: 7.0 MB (7037418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30630ff604ee0f5b793f4d6dcfb3156992bb4a226f75d41213a6ea23e7057e58`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ef7cd63ea6b2f85ed3540b09e2f8f4a31a4a20ecebd88135002f0d29b2533f`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a68f5767e0f485387c46fe28df422acf740e8831955651e7b6ca916ab3f52071
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32200613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8343f39cdca8596668b92bebbdad64930181c27e383d37c1a6943182e202fb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:12:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 05:12:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:12:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 05:13:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 05:13:46 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 05:13:46 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 05:13:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:13:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:13:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7bbdd9ad10264bd31c073aa67f6e04e014d25a92fa44b8cdc85a66b49d3e`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95a6bcf02d0c380ceb6339aa314e5cc271870d64c1c131c8d1a89d5aedbf371`  
		Last Modified: Wed, 23 Jun 2021 05:14:21 GMT  
		Size: 1.8 MB (1839313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dec4e8ba1333802d705cfedbbb7d57ef3407102ba371ee5b3afeeb3b6a4906`  
		Last Modified: Wed, 23 Jun 2021 05:14:25 GMT  
		Size: 5.5 MB (5480145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e797035b745745c7aabb74f5187811477900b08d4de77418d1c4b44ae3642a9`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50aa5ce3a5b802a562d044c299aafdec277da107220ec1dd1ebdceeef4395c5a`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8f3dcc5672e08027b33653e7999eab3091a08a8cb2911f42832543451907ec22
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1835331fef38be27cb80bf4a7f5b084d008b3fbf5425bc9d9d191e76d3ec10b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 20:59:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Jun 2021 20:59:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Jun 2021 20:59:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 16 Jun 2021 21:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Jun 2021 21:00:20 GMT
VOLUME [/spiped]
# Wed, 16 Jun 2021 21:00:20 GMT
WORKDIR /spiped
# Wed, 16 Jun 2021 21:00:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Jun 2021 21:00:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 21:00:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a138a3599035cdb1344595fc1e373195d5502ba9ad2b19dded9fc9bcadf76472`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecaf1d52ed2cd4ab43df4821c429206a8d2ced2f9e20be6e12008770d746d39d`  
		Last Modified: Wed, 16 Jun 2021 21:01:10 GMT  
		Size: 1.8 MB (1759508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f53a999ed2e7f6391b4db1a00ceb30dd0b554f1258b81d7ae232af4989c0aa3`  
		Last Modified: Wed, 16 Jun 2021 21:01:10 GMT  
		Size: 5.3 MB (5285557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66830d84d7cb6aedf6f77790563281d0c2b333fbbe9e3838f92ac9e9a2faead`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de1593245c38600bbc3eded9fb1ed99e58b680e984c27b60e73689d11446712`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ac6f7688ea32f8a2f442fe68855114b8562caf896a3357d0615cc30b5d2168f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33830362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7838646f1ed01bb14846176266e7f79452000256d1ee2fc64ffa49d1cc32bc45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 04:44:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 04:44:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 04:44:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 04:44:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 04:44:48 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 04:44:48 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 04:44:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 04:44:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 04:44:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba75a48871843ec90c5653d7a68d32d4782e02661ed505a4aac4ba2e6b162b1c`  
		Last Modified: Wed, 23 Jun 2021 04:45:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78779b3a1ea7be051ec8a444920361dd44691bd2598360f19fcdea7b6cb8a5f`  
		Last Modified: Wed, 23 Jun 2021 04:45:25 GMT  
		Size: 2.0 MB (2007837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9e473ed57b4a2a7f6c6e0c3691bac286e4d62776d948af11510ba7e0be4798`  
		Last Modified: Wed, 23 Jun 2021 04:45:26 GMT  
		Size: 5.9 MB (5905325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0471736cf2872e3b8fcc5cda063cef30d8ddc0cf493dda64f0e46cc192c6fa13`  
		Last Modified: Wed, 23 Jun 2021 04:45:25 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9a2c649b4c4c03bcfaf26b19aa23ee9c4a47913c519b5d88525967c961d9c5`  
		Last Modified: Wed, 23 Jun 2021 04:45:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:c626e5813307c4a522253701a8d10044490c5089fc1028865064aba56b79a567
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41565721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d520e0fa299bb26925db9d358ba485a922493b570445e869fe9cbc2c58a7a28a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 05:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 05:25:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 05:25:44 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 05:25:44 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 05:25:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:25:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:25:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a64acf577cc0906169a6fa1d1f41dd113b4cc5d2b0c8a3abb5674bb67a0c`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fe45b208cc8a9347120d3a18375f5bf334cde361e3d200c6cc2bfcd4e434c4`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 2.1 MB (2132634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d718789ca722dbc6e8352f0995209e18d785aab7390970c8fa4ffb85f633a704`  
		Last Modified: Wed, 23 Jun 2021 05:26:30 GMT  
		Size: 11.6 MB (11633477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d07737683dbbe7090182a8b646edec35d04531fc2c86a7f16512be098c6da6b`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4226fc02e39ef6661fe88338e9310db680d285e76408908cca7423c191625554`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:f8f7c8d549f49ae5784c026f95e0f1c34050e2f2379583f963386ee6a0cb4269
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33944242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:706e105af193dd6f9cfa952b76493ca2ba0096fe4c9268215b98027fbcc56f69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:29 GMT
ADD file:ca8422268fc66c67d19fd3a33a14a9bd6280ef21404677767ffd561a8ecf6724 in / 
# Wed, 23 Jun 2021 00:09:30 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:32:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 01:32:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 01:32:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 01:33:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:33:51 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 01:33:51 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 01:33:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 01:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 01:33:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4b9d1870c33c63bfde89c401b4af9582fbbff99d4036171a7a456706bf805d6d`  
		Last Modified: Wed, 23 Jun 2021 00:15:49 GMT  
		Size: 25.8 MB (25812890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b885417e0bed54626f847700fe119413544e07f53c9499064e4abb845490d9e`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d953da28b94c0e3b1a5834ae8fe31286237bbe9e3e71baad6edaef250f76e1`  
		Last Modified: Wed, 23 Jun 2021 01:34:19 GMT  
		Size: 1.7 MB (1712456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f20808768a5d40a26c1798479f76bf9064479a905b35f2d456cda0965d0bd8`  
		Last Modified: Wed, 23 Jun 2021 01:34:23 GMT  
		Size: 6.4 MB (6416722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b761e90f141aed8e640a25f68de1ed7052106a07ddf39cccd72dfe435b327802`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834563460305f4d062830ddecdb6f066e97e325f99acc8993a775bb7d322e682`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:4b249d499e7803150d5e0bab261950fc32089f5d19ad4ac725ce45b11e671eec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39524958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:662d5d6adaafe8261a7658051c3b5d8aee9100038f6b8d1ebb0b9fb17c52dc08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:20:36 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 06:21:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:21:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 06:24:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 06:24:12 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 06:24:16 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 06:24:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 06:24:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 06:24:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191c3937be8dbf43a8cfe50ad1a13e2dfaa99ea305bc8737627f6c4287d96249`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f610226f8d0550f8b920d027e63c3d5893fb9dbd9b251c1ef4c5a74d7c7af6ec`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 2.2 MB (2225166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ccf30cf2ac919705de54736fa518e3ebb3616e369b14484a125a2ad199597d`  
		Last Modified: Wed, 23 Jun 2021 06:26:41 GMT  
		Size: 6.7 MB (6743950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242cd2a18a0f522beb5fe1b8c192dd53c4f26f1f7c3822de8844af8ca0147a80`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73fc146b40b720705bfdf9cb0e0021348650da2a65afd9422b16bae5808ff2c`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:f7dc97ece5b5e4d70543bc74530ef4deb589f4defd2da77a771256e224f5841b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33528623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25b2527cb8f7e7c6e56a036a318afecae66b8a8327a19682c3904a340ca1a91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:28 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Tue, 22 Jun 2021 23:42:29 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:07:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 07:07:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:07:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 07:07:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 07:07:41 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 07:07:41 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 07:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:07:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:07:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ce76b947c34bd5af41d4870addb2699c4d0efb8a49c56af6a652c597b57376`  
		Last Modified: Wed, 23 Jun 2021 07:08:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451210b67a054c152e290b9fb707533662c85beadc1f9b1ebea5646f8af43c61`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 1.8 MB (1822020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d555c923d315711ae231e90d1cc857f4b3b6e7262c4c5bed071c33d2838d30da`  
		Last Modified: Wed, 23 Jun 2021 07:08:13 GMT  
		Size: 5.9 MB (5943675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520d76ccbffa39f96280eb068ed865face7fd9ad86300ba6018764061c57b0d2`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadd101ff04664820ade42807681d9e370f5109c372f19eaca4aac8e6c666eaf`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:b611f87cb8a8b2e94c240963e034606320ee732a29c0de5f7ee6bdd32f1427db
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
$ docker pull spiped@sha256:91c1773cab1581d76d4d48e8b17a155fdf6fa54339e449958132b7ab0e664b7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3324815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5620d28ab14686bc056b383ca94e121a1961a59dfa98a9a4e24992d49ccaf583`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:13:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 11:13:44 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 11:13:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 16 Jun 2021 11:14:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 16 Jun 2021 11:14:01 GMT
VOLUME [/spiped]
# Wed, 16 Jun 2021 11:14:01 GMT
WORKDIR /spiped
# Wed, 16 Jun 2021 11:14:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:14:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:14:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be0802b4de23117d6b04cc1a7237f151ac257b9b6ae94c41543add13a721211`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1598d38937e859a5682a8b4222572712c05ed3cd91911fc2b0402c4d3610bd1f`  
		Last Modified: Wed, 16 Jun 2021 11:14:50 GMT  
		Size: 7.1 KB (7060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93daa195a9f9aae8df4b499ba4d793860c0aab39686330ecc6a410b8f7bf58e6`  
		Last Modified: Wed, 16 Jun 2021 11:14:50 GMT  
		Size: 604.0 KB (603997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011245e695623945bea926d3f62bed142c2caf7f2ff394931342b395e9bf2c6a`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a47c9f4da08454bed52a6c03bb7e750ec3ad498ed63773d6e46ddaccca505a5`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:71c26b5882a1b12cad71178d31d4d15dd3d3fe3252014611f5adc879192d2e72
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
$ docker pull spiped@sha256:deca629e565a472791c066c34d81b0536d6e3393ebbb45ede224ba9e33fac0cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36314034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cfebea6aa229524e4eb8300c3f8a158570052fa02ec5efe7973e020741adc55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:52:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 17:52:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:52:38 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 17:53:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 17:53:06 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 17:53:06 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 17:53:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 17:53:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 17:53:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9436548b6b61a5565bdee4208eb7b277f1bd36cf5416483a730e4a1ea42be97`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af92bc2edfa15c30f1fc1536102eba6dc3369e7fddc435b31c63a356e7289732`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 2.1 MB (2128557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6c58cd98ed2868a2430518c3d20baa273bd886c4b8d1578ec65631aed39497`  
		Last Modified: Wed, 23 Jun 2021 17:53:41 GMT  
		Size: 7.0 MB (7037418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30630ff604ee0f5b793f4d6dcfb3156992bb4a226f75d41213a6ea23e7057e58`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ef7cd63ea6b2f85ed3540b09e2f8f4a31a4a20ecebd88135002f0d29b2533f`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a68f5767e0f485387c46fe28df422acf740e8831955651e7b6ca916ab3f52071
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32200613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8343f39cdca8596668b92bebbdad64930181c27e383d37c1a6943182e202fb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:12:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 05:12:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:12:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 05:13:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 05:13:46 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 05:13:46 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 05:13:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:13:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:13:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7bbdd9ad10264bd31c073aa67f6e04e014d25a92fa44b8cdc85a66b49d3e`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95a6bcf02d0c380ceb6339aa314e5cc271870d64c1c131c8d1a89d5aedbf371`  
		Last Modified: Wed, 23 Jun 2021 05:14:21 GMT  
		Size: 1.8 MB (1839313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dec4e8ba1333802d705cfedbbb7d57ef3407102ba371ee5b3afeeb3b6a4906`  
		Last Modified: Wed, 23 Jun 2021 05:14:25 GMT  
		Size: 5.5 MB (5480145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e797035b745745c7aabb74f5187811477900b08d4de77418d1c4b44ae3642a9`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50aa5ce3a5b802a562d044c299aafdec277da107220ec1dd1ebdceeef4395c5a`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8f3dcc5672e08027b33653e7999eab3091a08a8cb2911f42832543451907ec22
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1835331fef38be27cb80bf4a7f5b084d008b3fbf5425bc9d9d191e76d3ec10b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 20:59:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Jun 2021 20:59:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Jun 2021 20:59:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 16 Jun 2021 21:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Jun 2021 21:00:20 GMT
VOLUME [/spiped]
# Wed, 16 Jun 2021 21:00:20 GMT
WORKDIR /spiped
# Wed, 16 Jun 2021 21:00:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Jun 2021 21:00:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 21:00:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a138a3599035cdb1344595fc1e373195d5502ba9ad2b19dded9fc9bcadf76472`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecaf1d52ed2cd4ab43df4821c429206a8d2ced2f9e20be6e12008770d746d39d`  
		Last Modified: Wed, 16 Jun 2021 21:01:10 GMT  
		Size: 1.8 MB (1759508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f53a999ed2e7f6391b4db1a00ceb30dd0b554f1258b81d7ae232af4989c0aa3`  
		Last Modified: Wed, 16 Jun 2021 21:01:10 GMT  
		Size: 5.3 MB (5285557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66830d84d7cb6aedf6f77790563281d0c2b333fbbe9e3838f92ac9e9a2faead`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de1593245c38600bbc3eded9fb1ed99e58b680e984c27b60e73689d11446712`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ac6f7688ea32f8a2f442fe68855114b8562caf896a3357d0615cc30b5d2168f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33830362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7838646f1ed01bb14846176266e7f79452000256d1ee2fc64ffa49d1cc32bc45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 04:44:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 04:44:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 04:44:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 04:44:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 04:44:48 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 04:44:48 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 04:44:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 04:44:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 04:44:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba75a48871843ec90c5653d7a68d32d4782e02661ed505a4aac4ba2e6b162b1c`  
		Last Modified: Wed, 23 Jun 2021 04:45:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78779b3a1ea7be051ec8a444920361dd44691bd2598360f19fcdea7b6cb8a5f`  
		Last Modified: Wed, 23 Jun 2021 04:45:25 GMT  
		Size: 2.0 MB (2007837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9e473ed57b4a2a7f6c6e0c3691bac286e4d62776d948af11510ba7e0be4798`  
		Last Modified: Wed, 23 Jun 2021 04:45:26 GMT  
		Size: 5.9 MB (5905325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0471736cf2872e3b8fcc5cda063cef30d8ddc0cf493dda64f0e46cc192c6fa13`  
		Last Modified: Wed, 23 Jun 2021 04:45:25 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9a2c649b4c4c03bcfaf26b19aa23ee9c4a47913c519b5d88525967c961d9c5`  
		Last Modified: Wed, 23 Jun 2021 04:45:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:c626e5813307c4a522253701a8d10044490c5089fc1028865064aba56b79a567
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41565721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d520e0fa299bb26925db9d358ba485a922493b570445e869fe9cbc2c58a7a28a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 05:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 05:25:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 05:25:44 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 05:25:44 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 05:25:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:25:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:25:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a64acf577cc0906169a6fa1d1f41dd113b4cc5d2b0c8a3abb5674bb67a0c`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fe45b208cc8a9347120d3a18375f5bf334cde361e3d200c6cc2bfcd4e434c4`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 2.1 MB (2132634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d718789ca722dbc6e8352f0995209e18d785aab7390970c8fa4ffb85f633a704`  
		Last Modified: Wed, 23 Jun 2021 05:26:30 GMT  
		Size: 11.6 MB (11633477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d07737683dbbe7090182a8b646edec35d04531fc2c86a7f16512be098c6da6b`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4226fc02e39ef6661fe88338e9310db680d285e76408908cca7423c191625554`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:f8f7c8d549f49ae5784c026f95e0f1c34050e2f2379583f963386ee6a0cb4269
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33944242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:706e105af193dd6f9cfa952b76493ca2ba0096fe4c9268215b98027fbcc56f69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:29 GMT
ADD file:ca8422268fc66c67d19fd3a33a14a9bd6280ef21404677767ffd561a8ecf6724 in / 
# Wed, 23 Jun 2021 00:09:30 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:32:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 01:32:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 01:32:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 01:33:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:33:51 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 01:33:51 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 01:33:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 01:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 01:33:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4b9d1870c33c63bfde89c401b4af9582fbbff99d4036171a7a456706bf805d6d`  
		Last Modified: Wed, 23 Jun 2021 00:15:49 GMT  
		Size: 25.8 MB (25812890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b885417e0bed54626f847700fe119413544e07f53c9499064e4abb845490d9e`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d953da28b94c0e3b1a5834ae8fe31286237bbe9e3e71baad6edaef250f76e1`  
		Last Modified: Wed, 23 Jun 2021 01:34:19 GMT  
		Size: 1.7 MB (1712456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f20808768a5d40a26c1798479f76bf9064479a905b35f2d456cda0965d0bd8`  
		Last Modified: Wed, 23 Jun 2021 01:34:23 GMT  
		Size: 6.4 MB (6416722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b761e90f141aed8e640a25f68de1ed7052106a07ddf39cccd72dfe435b327802`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834563460305f4d062830ddecdb6f066e97e325f99acc8993a775bb7d322e682`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:4b249d499e7803150d5e0bab261950fc32089f5d19ad4ac725ce45b11e671eec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39524958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:662d5d6adaafe8261a7658051c3b5d8aee9100038f6b8d1ebb0b9fb17c52dc08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:20:36 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 06:21:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:21:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 06:24:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 06:24:12 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 06:24:16 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 06:24:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 06:24:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 06:24:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191c3937be8dbf43a8cfe50ad1a13e2dfaa99ea305bc8737627f6c4287d96249`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f610226f8d0550f8b920d027e63c3d5893fb9dbd9b251c1ef4c5a74d7c7af6ec`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 2.2 MB (2225166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ccf30cf2ac919705de54736fa518e3ebb3616e369b14484a125a2ad199597d`  
		Last Modified: Wed, 23 Jun 2021 06:26:41 GMT  
		Size: 6.7 MB (6743950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242cd2a18a0f522beb5fe1b8c192dd53c4f26f1f7c3822de8844af8ca0147a80`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73fc146b40b720705bfdf9cb0e0021348650da2a65afd9422b16bae5808ff2c`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:f7dc97ece5b5e4d70543bc74530ef4deb589f4defd2da77a771256e224f5841b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33528623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25b2527cb8f7e7c6e56a036a318afecae66b8a8327a19682c3904a340ca1a91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:28 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Tue, 22 Jun 2021 23:42:29 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:07:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 07:07:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:07:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 07:07:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 07:07:41 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 07:07:41 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 07:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:07:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:07:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ce76b947c34bd5af41d4870addb2699c4d0efb8a49c56af6a652c597b57376`  
		Last Modified: Wed, 23 Jun 2021 07:08:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451210b67a054c152e290b9fb707533662c85beadc1f9b1ebea5646f8af43c61`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 1.8 MB (1822020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d555c923d315711ae231e90d1cc857f4b3b6e7262c4c5bed071c33d2838d30da`  
		Last Modified: Wed, 23 Jun 2021 07:08:13 GMT  
		Size: 5.9 MB (5943675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520d76ccbffa39f96280eb068ed865face7fd9ad86300ba6018764061c57b0d2`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadd101ff04664820ade42807681d9e370f5109c372f19eaca4aac8e6c666eaf`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:b611f87cb8a8b2e94c240963e034606320ee732a29c0de5f7ee6bdd32f1427db
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
$ docker pull spiped@sha256:91c1773cab1581d76d4d48e8b17a155fdf6fa54339e449958132b7ab0e664b7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3324815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5620d28ab14686bc056b383ca94e121a1961a59dfa98a9a4e24992d49ccaf583`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:13:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 11:13:44 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 11:13:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 16 Jun 2021 11:14:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 16 Jun 2021 11:14:01 GMT
VOLUME [/spiped]
# Wed, 16 Jun 2021 11:14:01 GMT
WORKDIR /spiped
# Wed, 16 Jun 2021 11:14:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:14:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:14:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be0802b4de23117d6b04cc1a7237f151ac257b9b6ae94c41543add13a721211`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1598d38937e859a5682a8b4222572712c05ed3cd91911fc2b0402c4d3610bd1f`  
		Last Modified: Wed, 16 Jun 2021 11:14:50 GMT  
		Size: 7.1 KB (7060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93daa195a9f9aae8df4b499ba4d793860c0aab39686330ecc6a410b8f7bf58e6`  
		Last Modified: Wed, 16 Jun 2021 11:14:50 GMT  
		Size: 604.0 KB (603997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011245e695623945bea926d3f62bed142c2caf7f2ff394931342b395e9bf2c6a`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a47c9f4da08454bed52a6c03bb7e750ec3ad498ed63773d6e46ddaccca505a5`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:b611f87cb8a8b2e94c240963e034606320ee732a29c0de5f7ee6bdd32f1427db
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
$ docker pull spiped@sha256:91c1773cab1581d76d4d48e8b17a155fdf6fa54339e449958132b7ab0e664b7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3324815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5620d28ab14686bc056b383ca94e121a1961a59dfa98a9a4e24992d49ccaf583`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:13:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 11:13:44 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 11:13:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 16 Jun 2021 11:14:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 16 Jun 2021 11:14:01 GMT
VOLUME [/spiped]
# Wed, 16 Jun 2021 11:14:01 GMT
WORKDIR /spiped
# Wed, 16 Jun 2021 11:14:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:14:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:14:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be0802b4de23117d6b04cc1a7237f151ac257b9b6ae94c41543add13a721211`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1598d38937e859a5682a8b4222572712c05ed3cd91911fc2b0402c4d3610bd1f`  
		Last Modified: Wed, 16 Jun 2021 11:14:50 GMT  
		Size: 7.1 KB (7060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93daa195a9f9aae8df4b499ba4d793860c0aab39686330ecc6a410b8f7bf58e6`  
		Last Modified: Wed, 16 Jun 2021 11:14:50 GMT  
		Size: 604.0 KB (603997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011245e695623945bea926d3f62bed142c2caf7f2ff394931342b395e9bf2c6a`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a47c9f4da08454bed52a6c03bb7e750ec3ad498ed63773d6e46ddaccca505a5`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:71c26b5882a1b12cad71178d31d4d15dd3d3fe3252014611f5adc879192d2e72
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
$ docker pull spiped@sha256:deca629e565a472791c066c34d81b0536d6e3393ebbb45ede224ba9e33fac0cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36314034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cfebea6aa229524e4eb8300c3f8a158570052fa02ec5efe7973e020741adc55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:52:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 17:52:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:52:38 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 17:53:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 17:53:06 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 17:53:06 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 17:53:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 17:53:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 17:53:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9436548b6b61a5565bdee4208eb7b277f1bd36cf5416483a730e4a1ea42be97`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af92bc2edfa15c30f1fc1536102eba6dc3369e7fddc435b31c63a356e7289732`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 2.1 MB (2128557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6c58cd98ed2868a2430518c3d20baa273bd886c4b8d1578ec65631aed39497`  
		Last Modified: Wed, 23 Jun 2021 17:53:41 GMT  
		Size: 7.0 MB (7037418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30630ff604ee0f5b793f4d6dcfb3156992bb4a226f75d41213a6ea23e7057e58`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ef7cd63ea6b2f85ed3540b09e2f8f4a31a4a20ecebd88135002f0d29b2533f`  
		Last Modified: Wed, 23 Jun 2021 17:53:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a68f5767e0f485387c46fe28df422acf740e8831955651e7b6ca916ab3f52071
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32200613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8343f39cdca8596668b92bebbdad64930181c27e383d37c1a6943182e202fb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:12:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 05:12:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:12:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 05:13:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 05:13:46 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 05:13:46 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 05:13:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:13:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:13:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7bbdd9ad10264bd31c073aa67f6e04e014d25a92fa44b8cdc85a66b49d3e`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95a6bcf02d0c380ceb6339aa314e5cc271870d64c1c131c8d1a89d5aedbf371`  
		Last Modified: Wed, 23 Jun 2021 05:14:21 GMT  
		Size: 1.8 MB (1839313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dec4e8ba1333802d705cfedbbb7d57ef3407102ba371ee5b3afeeb3b6a4906`  
		Last Modified: Wed, 23 Jun 2021 05:14:25 GMT  
		Size: 5.5 MB (5480145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e797035b745745c7aabb74f5187811477900b08d4de77418d1c4b44ae3642a9`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50aa5ce3a5b802a562d044c299aafdec277da107220ec1dd1ebdceeef4395c5a`  
		Last Modified: Wed, 23 Jun 2021 05:14:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8f3dcc5672e08027b33653e7999eab3091a08a8cb2911f42832543451907ec22
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1835331fef38be27cb80bf4a7f5b084d008b3fbf5425bc9d9d191e76d3ec10b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 20:59:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Jun 2021 20:59:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Jun 2021 20:59:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 16 Jun 2021 21:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Jun 2021 21:00:20 GMT
VOLUME [/spiped]
# Wed, 16 Jun 2021 21:00:20 GMT
WORKDIR /spiped
# Wed, 16 Jun 2021 21:00:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Jun 2021 21:00:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 21:00:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a138a3599035cdb1344595fc1e373195d5502ba9ad2b19dded9fc9bcadf76472`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecaf1d52ed2cd4ab43df4821c429206a8d2ced2f9e20be6e12008770d746d39d`  
		Last Modified: Wed, 16 Jun 2021 21:01:10 GMT  
		Size: 1.8 MB (1759508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f53a999ed2e7f6391b4db1a00ceb30dd0b554f1258b81d7ae232af4989c0aa3`  
		Last Modified: Wed, 16 Jun 2021 21:01:10 GMT  
		Size: 5.3 MB (5285557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66830d84d7cb6aedf6f77790563281d0c2b333fbbe9e3838f92ac9e9a2faead`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de1593245c38600bbc3eded9fb1ed99e58b680e984c27b60e73689d11446712`  
		Last Modified: Wed, 16 Jun 2021 21:01:09 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ac6f7688ea32f8a2f442fe68855114b8562caf896a3357d0615cc30b5d2168f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33830362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7838646f1ed01bb14846176266e7f79452000256d1ee2fc64ffa49d1cc32bc45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 04:44:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 04:44:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 04:44:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 04:44:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 04:44:48 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 04:44:48 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 04:44:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 04:44:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 04:44:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba75a48871843ec90c5653d7a68d32d4782e02661ed505a4aac4ba2e6b162b1c`  
		Last Modified: Wed, 23 Jun 2021 04:45:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78779b3a1ea7be051ec8a444920361dd44691bd2598360f19fcdea7b6cb8a5f`  
		Last Modified: Wed, 23 Jun 2021 04:45:25 GMT  
		Size: 2.0 MB (2007837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9e473ed57b4a2a7f6c6e0c3691bac286e4d62776d948af11510ba7e0be4798`  
		Last Modified: Wed, 23 Jun 2021 04:45:26 GMT  
		Size: 5.9 MB (5905325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0471736cf2872e3b8fcc5cda063cef30d8ddc0cf493dda64f0e46cc192c6fa13`  
		Last Modified: Wed, 23 Jun 2021 04:45:25 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9a2c649b4c4c03bcfaf26b19aa23ee9c4a47913c519b5d88525967c961d9c5`  
		Last Modified: Wed, 23 Jun 2021 04:45:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:c626e5813307c4a522253701a8d10044490c5089fc1028865064aba56b79a567
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41565721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d520e0fa299bb26925db9d358ba485a922493b570445e869fe9cbc2c58a7a28a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 05:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 05:25:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 05:25:44 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 05:25:44 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 05:25:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:25:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:25:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a64acf577cc0906169a6fa1d1f41dd113b4cc5d2b0c8a3abb5674bb67a0c`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fe45b208cc8a9347120d3a18375f5bf334cde361e3d200c6cc2bfcd4e434c4`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 2.1 MB (2132634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d718789ca722dbc6e8352f0995209e18d785aab7390970c8fa4ffb85f633a704`  
		Last Modified: Wed, 23 Jun 2021 05:26:30 GMT  
		Size: 11.6 MB (11633477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d07737683dbbe7090182a8b646edec35d04531fc2c86a7f16512be098c6da6b`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4226fc02e39ef6661fe88338e9310db680d285e76408908cca7423c191625554`  
		Last Modified: Wed, 23 Jun 2021 05:26:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:f8f7c8d549f49ae5784c026f95e0f1c34050e2f2379583f963386ee6a0cb4269
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33944242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:706e105af193dd6f9cfa952b76493ca2ba0096fe4c9268215b98027fbcc56f69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:29 GMT
ADD file:ca8422268fc66c67d19fd3a33a14a9bd6280ef21404677767ffd561a8ecf6724 in / 
# Wed, 23 Jun 2021 00:09:30 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 01:32:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 01:32:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 01:32:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 01:33:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 01:33:51 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 01:33:51 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 01:33:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 01:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 01:33:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4b9d1870c33c63bfde89c401b4af9582fbbff99d4036171a7a456706bf805d6d`  
		Last Modified: Wed, 23 Jun 2021 00:15:49 GMT  
		Size: 25.8 MB (25812890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b885417e0bed54626f847700fe119413544e07f53c9499064e4abb845490d9e`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d953da28b94c0e3b1a5834ae8fe31286237bbe9e3e71baad6edaef250f76e1`  
		Last Modified: Wed, 23 Jun 2021 01:34:19 GMT  
		Size: 1.7 MB (1712456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f20808768a5d40a26c1798479f76bf9064479a905b35f2d456cda0965d0bd8`  
		Last Modified: Wed, 23 Jun 2021 01:34:23 GMT  
		Size: 6.4 MB (6416722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b761e90f141aed8e640a25f68de1ed7052106a07ddf39cccd72dfe435b327802`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834563460305f4d062830ddecdb6f066e97e325f99acc8993a775bb7d322e682`  
		Last Modified: Wed, 23 Jun 2021 01:34:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:4b249d499e7803150d5e0bab261950fc32089f5d19ad4ac725ce45b11e671eec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39524958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:662d5d6adaafe8261a7658051c3b5d8aee9100038f6b8d1ebb0b9fb17c52dc08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:20:36 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 06:21:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:21:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 06:24:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 06:24:12 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 06:24:16 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 06:24:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 06:24:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 06:24:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191c3937be8dbf43a8cfe50ad1a13e2dfaa99ea305bc8737627f6c4287d96249`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f610226f8d0550f8b920d027e63c3d5893fb9dbd9b251c1ef4c5a74d7c7af6ec`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 2.2 MB (2225166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ccf30cf2ac919705de54736fa518e3ebb3616e369b14484a125a2ad199597d`  
		Last Modified: Wed, 23 Jun 2021 06:26:41 GMT  
		Size: 6.7 MB (6743950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242cd2a18a0f522beb5fe1b8c192dd53c4f26f1f7c3822de8844af8ca0147a80`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73fc146b40b720705bfdf9cb0e0021348650da2a65afd9422b16bae5808ff2c`  
		Last Modified: Wed, 23 Jun 2021 06:26:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:f7dc97ece5b5e4d70543bc74530ef4deb589f4defd2da77a771256e224f5841b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33528623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a25b2527cb8f7e7c6e56a036a318afecae66b8a8327a19682c3904a340ca1a91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:28 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Tue, 22 Jun 2021 23:42:29 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:07:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 23 Jun 2021 07:07:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:07:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 23 Jun 2021 07:07:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 23 Jun 2021 07:07:41 GMT
VOLUME [/spiped]
# Wed, 23 Jun 2021 07:07:41 GMT
WORKDIR /spiped
# Wed, 23 Jun 2021 07:07:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:07:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:07:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ce76b947c34bd5af41d4870addb2699c4d0efb8a49c56af6a652c597b57376`  
		Last Modified: Wed, 23 Jun 2021 07:08:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451210b67a054c152e290b9fb707533662c85beadc1f9b1ebea5646f8af43c61`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 1.8 MB (1822020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d555c923d315711ae231e90d1cc857f4b3b6e7262c4c5bed071c33d2838d30da`  
		Last Modified: Wed, 23 Jun 2021 07:08:13 GMT  
		Size: 5.9 MB (5943675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520d76ccbffa39f96280eb068ed865face7fd9ad86300ba6018764061c57b0d2`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadd101ff04664820ade42807681d9e370f5109c372f19eaca4aac8e6c666eaf`  
		Last Modified: Wed, 23 Jun 2021 07:08:11 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
