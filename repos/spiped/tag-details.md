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
$ docker pull spiped@sha256:e3956f14538b744b8891f7b3ca25f5bebc25191e0c09c7191a5ca5245d6bcca0
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
$ docker pull spiped@sha256:c8fcd50e24a2fac4210299a2ee03f0d8d0de3a6e51ba6f61a56c263f16a82fd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5275d81bc421af6ac42959ab8c655ffe4f05b57d6f87325b371cbe74019778`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 07:24:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 24 Jun 2021 07:24:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 07:24:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 24 Jun 2021 07:25:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 24 Jun 2021 07:25:32 GMT
VOLUME [/spiped]
# Thu, 24 Jun 2021 07:25:33 GMT
WORKDIR /spiped
# Thu, 24 Jun 2021 07:25:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 24 Jun 2021 07:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 07:25:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14b3189ef30e120910a62a83035bb35be5ad21d868baa15635cd4093e57b28`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fbbe41540f8564924d1bbf33810a5cca942d52258a07a9a0a9fa47d3e2ee4d`  
		Last Modified: Thu, 24 Jun 2021 07:26:44 GMT  
		Size: 1.8 MB (1759528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6efa0bc06b8244fc2b99086aaab3707ad97a5c1562d486c49f2643704d4c14f`  
		Last Modified: Thu, 24 Jun 2021 07:26:47 GMT  
		Size: 5.3 MB (5285807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf51d89722279aa5fe979daa99ecca041af3e85c0ecb284c9eef346e12a8525`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ce586c187940aa96e929532b8802dd2d2590ae0629d8d6ff5683defad7d791`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:54c06566e53ed883f540aac6ef04c0b592bd490887621be35c1089106b697e7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39524856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57d64ff238cc272cd4b46a7dcb066e80d77dded09ac13be158b57ebddfb9be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 20:10:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 25 Jun 2021 20:10:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 20:10:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 20:13:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 25 Jun 2021 20:13:47 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 20:13:51 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 20:13:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 20:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 20:14:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4850a05a8ee69386fd934aa7e803a6ab5114a463b2f67029a79345a3e2258215`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65420b8b6a00225fef8990d8f2bb04ac6297f210d1018a7d55ad7a16bd40f78`  
		Last Modified: Fri, 25 Jun 2021 20:15:59 GMT  
		Size: 2.2 MB (2225168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ed66b43cf8ca387a94faaeafe401ad9c331b2d56b9cf2a01dfd4a4df32246`  
		Last Modified: Fri, 25 Jun 2021 20:16:00 GMT  
		Size: 6.7 MB (6743843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a2bd0b6c1fefb2ef43012c2c366d9194597f452679f46c376dec153b5be885`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc82701a4e5b97700db148e5c577a64a955835728f7ed57cc58a7306a6e0b21`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:1054032dfae72f0807214d0751246c6675a4527de4b0af06446b9ed3281c5ff9
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
$ docker pull spiped@sha256:77bb7048879f502a0be6947d6ded556dedd56bfbd65846f202ddbae6c0220f84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecec5286e75ac64570dd86ae159bec30df6ff4bb0ecc79f42dd8a5c7126be6eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:41:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:41:21 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:41:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:03:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:03:03 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:03:03 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:03:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:03:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc49c1d100974d70cd457c65f0e781af958b9d07a56e03267424f0d11990712`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3e43d8c62d03bca76a106e58c3099bd76fb7fbad003082a81a3670c07ba69`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdfa185ef47533e780a1502b6ecf0f1486cc0955b4930432fdfdc77813e9d50`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 212.6 KB (212559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241cc499201ce5b553c5be7e1b77bfddb66137711a90180f2e25689109405751`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d6882fdc5e95f3b1481ffb5d149c0fda3dc71d8fa51eba15edc3be50dc54c`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b758b42acbf998e5a39dc12204e0be903d69a2af37753e5d2133b5df87b06523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2835923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae8ff3806515f364a387402ad57b51af1f948f849240b2e704a6de2c048ada9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 00:21:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Jun 2021 00:21:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Jun 2021 00:21:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:38:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:38:07 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:38:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:38:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9e2daf3ec825cb3613604aa1365dbe414dc4e91784135871c1b1dfc68db23d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101fbc0ffdf60230b896427f198bc223946522d7d1f77e2275181837980568d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296999154521c5c6c6c67a405f842cacada3793a86c889ce922a114bae5354a6`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 202.5 KB (202495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c40bed8d80ea82bb949a3747badad3421eb16ea2e2440962324c9d79ab00b`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd55faef8cc92525b1be13e1e39b9ee16e5caaf2df3e0db276ed2683a509da9`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:57f8db33a0eec466bfc76dd17cee895a03a3789dbd31bd89ef2e8dc7da3455e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2632718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676e5f41ec430a6e87108a46dd408d068f0e501170755f72925c7a760ed458ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 07:25:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 24 Jun 2021 07:25:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 24 Jun 2021 07:25:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:17:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:17:30 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:17:30 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:17:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:17:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c429d40f3f855015d365208d1b968cd8f34de9ccedd71360b7f05eab24ddd1`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4522338918253627f69a56835ddb741f10f29e2de17157de4ca03a12561d3e05`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f4ce029c4b37ef76a46da093755b9e24c2d0765592fd00547e013edf3479c`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 195.8 KB (195767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10cb1e83ae0b13c5adcff700076e63bf3322c49067170f59c7ec0c9d6f0698f`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e1913bac6b271f9c4b484fad7338dcbc98a4526b6e48bf1f6a8ccb3fa3b9a`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:40541478eb401d67036d56bbd4cfd5933f148ce155f8e3292a4d083fbb62ba19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2923277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02b54f6f7a1b548ed3db2fc33cafcbb8ef9b27d6ae45811deeb5ecf484a3d75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:54:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:54:08 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:54:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:54:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:54:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a6e447f49f6576247dd515ff88f610088fde09c8c378492a19009d6f6fd3b`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05549f8a714910bf1ba795919183eda4ed8c6c1dacd25e27d16f60e584efd239`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b70a09132ff271f43729154235e305beed323f6f44bb8f91d3f71be66c9f58`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 204.6 KB (204616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf3cdb40c67131120870a15e3902a71c8b1db82a03999be16d35d7d6ae59309`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17f3d198dd5104ea91d70276d05d71182af08cf309adc75a3b64bd770c1699`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:041a4401f89326839b354e7fb7aeb38b07f545fab3de4c84dc0c8f9cebefacca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f94b397232ecc82d13aa208dbbe6e5a315e7a44a1d284fc0089f766e22aea2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:55:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:55:36 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:55:37 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:55:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:55:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8a1adc7e61a91c39fcba896b070192f506dd419fc77a733ce377c563448785`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982f88ff86958b26737edc45adbf2bf850db25cdc970e348723b0d305f5f6db2`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24fe46b36c0cdba759eaf8ea030281f67337289db167fb4d8d3b7da3e191680`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 223.4 KB (223438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb79119bc0cf80b5d4a32e3035a171c2c43177ce8bd6cf5f6ad53da848ae22`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027751b1d208d42e1c73a3526f36a885067bd323348563fb1186928a536a01a`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:e3956f14538b744b8891f7b3ca25f5bebc25191e0c09c7191a5ca5245d6bcca0
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
$ docker pull spiped@sha256:c8fcd50e24a2fac4210299a2ee03f0d8d0de3a6e51ba6f61a56c263f16a82fd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5275d81bc421af6ac42959ab8c655ffe4f05b57d6f87325b371cbe74019778`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 07:24:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 24 Jun 2021 07:24:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 07:24:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 24 Jun 2021 07:25:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 24 Jun 2021 07:25:32 GMT
VOLUME [/spiped]
# Thu, 24 Jun 2021 07:25:33 GMT
WORKDIR /spiped
# Thu, 24 Jun 2021 07:25:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 24 Jun 2021 07:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 07:25:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14b3189ef30e120910a62a83035bb35be5ad21d868baa15635cd4093e57b28`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fbbe41540f8564924d1bbf33810a5cca942d52258a07a9a0a9fa47d3e2ee4d`  
		Last Modified: Thu, 24 Jun 2021 07:26:44 GMT  
		Size: 1.8 MB (1759528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6efa0bc06b8244fc2b99086aaab3707ad97a5c1562d486c49f2643704d4c14f`  
		Last Modified: Thu, 24 Jun 2021 07:26:47 GMT  
		Size: 5.3 MB (5285807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf51d89722279aa5fe979daa99ecca041af3e85c0ecb284c9eef346e12a8525`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ce586c187940aa96e929532b8802dd2d2590ae0629d8d6ff5683defad7d791`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:54c06566e53ed883f540aac6ef04c0b592bd490887621be35c1089106b697e7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39524856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57d64ff238cc272cd4b46a7dcb066e80d77dded09ac13be158b57ebddfb9be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 20:10:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 25 Jun 2021 20:10:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 20:10:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 20:13:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 25 Jun 2021 20:13:47 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 20:13:51 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 20:13:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 20:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 20:14:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4850a05a8ee69386fd934aa7e803a6ab5114a463b2f67029a79345a3e2258215`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65420b8b6a00225fef8990d8f2bb04ac6297f210d1018a7d55ad7a16bd40f78`  
		Last Modified: Fri, 25 Jun 2021 20:15:59 GMT  
		Size: 2.2 MB (2225168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ed66b43cf8ca387a94faaeafe401ad9c331b2d56b9cf2a01dfd4a4df32246`  
		Last Modified: Fri, 25 Jun 2021 20:16:00 GMT  
		Size: 6.7 MB (6743843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a2bd0b6c1fefb2ef43012c2c366d9194597f452679f46c376dec153b5be885`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc82701a4e5b97700db148e5c577a64a955835728f7ed57cc58a7306a6e0b21`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:1054032dfae72f0807214d0751246c6675a4527de4b0af06446b9ed3281c5ff9
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
$ docker pull spiped@sha256:77bb7048879f502a0be6947d6ded556dedd56bfbd65846f202ddbae6c0220f84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecec5286e75ac64570dd86ae159bec30df6ff4bb0ecc79f42dd8a5c7126be6eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:41:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:41:21 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:41:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:03:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:03:03 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:03:03 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:03:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:03:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc49c1d100974d70cd457c65f0e781af958b9d07a56e03267424f0d11990712`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3e43d8c62d03bca76a106e58c3099bd76fb7fbad003082a81a3670c07ba69`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdfa185ef47533e780a1502b6ecf0f1486cc0955b4930432fdfdc77813e9d50`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 212.6 KB (212559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241cc499201ce5b553c5be7e1b77bfddb66137711a90180f2e25689109405751`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d6882fdc5e95f3b1481ffb5d149c0fda3dc71d8fa51eba15edc3be50dc54c`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b758b42acbf998e5a39dc12204e0be903d69a2af37753e5d2133b5df87b06523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2835923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae8ff3806515f364a387402ad57b51af1f948f849240b2e704a6de2c048ada9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 00:21:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Jun 2021 00:21:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Jun 2021 00:21:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:38:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:38:07 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:38:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:38:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9e2daf3ec825cb3613604aa1365dbe414dc4e91784135871c1b1dfc68db23d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101fbc0ffdf60230b896427f198bc223946522d7d1f77e2275181837980568d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296999154521c5c6c6c67a405f842cacada3793a86c889ce922a114bae5354a6`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 202.5 KB (202495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c40bed8d80ea82bb949a3747badad3421eb16ea2e2440962324c9d79ab00b`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd55faef8cc92525b1be13e1e39b9ee16e5caaf2df3e0db276ed2683a509da9`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:57f8db33a0eec466bfc76dd17cee895a03a3789dbd31bd89ef2e8dc7da3455e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2632718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676e5f41ec430a6e87108a46dd408d068f0e501170755f72925c7a760ed458ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 07:25:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 24 Jun 2021 07:25:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 24 Jun 2021 07:25:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:17:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:17:30 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:17:30 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:17:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:17:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c429d40f3f855015d365208d1b968cd8f34de9ccedd71360b7f05eab24ddd1`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4522338918253627f69a56835ddb741f10f29e2de17157de4ca03a12561d3e05`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f4ce029c4b37ef76a46da093755b9e24c2d0765592fd00547e013edf3479c`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 195.8 KB (195767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10cb1e83ae0b13c5adcff700076e63bf3322c49067170f59c7ec0c9d6f0698f`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e1913bac6b271f9c4b484fad7338dcbc98a4526b6e48bf1f6a8ccb3fa3b9a`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:40541478eb401d67036d56bbd4cfd5933f148ce155f8e3292a4d083fbb62ba19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2923277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02b54f6f7a1b548ed3db2fc33cafcbb8ef9b27d6ae45811deeb5ecf484a3d75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:54:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:54:08 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:54:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:54:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:54:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a6e447f49f6576247dd515ff88f610088fde09c8c378492a19009d6f6fd3b`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05549f8a714910bf1ba795919183eda4ed8c6c1dacd25e27d16f60e584efd239`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b70a09132ff271f43729154235e305beed323f6f44bb8f91d3f71be66c9f58`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 204.6 KB (204616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf3cdb40c67131120870a15e3902a71c8b1db82a03999be16d35d7d6ae59309`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17f3d198dd5104ea91d70276d05d71182af08cf309adc75a3b64bd770c1699`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:041a4401f89326839b354e7fb7aeb38b07f545fab3de4c84dc0c8f9cebefacca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f94b397232ecc82d13aa208dbbe6e5a315e7a44a1d284fc0089f766e22aea2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:55:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:55:36 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:55:37 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:55:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:55:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8a1adc7e61a91c39fcba896b070192f506dd419fc77a733ce377c563448785`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982f88ff86958b26737edc45adbf2bf850db25cdc970e348723b0d305f5f6db2`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24fe46b36c0cdba759eaf8ea030281f67337289db167fb4d8d3b7da3e191680`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 223.4 KB (223438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb79119bc0cf80b5d4a32e3035a171c2c43177ce8bd6cf5f6ad53da848ae22`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027751b1d208d42e1c73a3526f36a885067bd323348563fb1186928a536a01a`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:e3956f14538b744b8891f7b3ca25f5bebc25191e0c09c7191a5ca5245d6bcca0
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
$ docker pull spiped@sha256:c8fcd50e24a2fac4210299a2ee03f0d8d0de3a6e51ba6f61a56c263f16a82fd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5275d81bc421af6ac42959ab8c655ffe4f05b57d6f87325b371cbe74019778`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 07:24:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 24 Jun 2021 07:24:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 07:24:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 24 Jun 2021 07:25:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 24 Jun 2021 07:25:32 GMT
VOLUME [/spiped]
# Thu, 24 Jun 2021 07:25:33 GMT
WORKDIR /spiped
# Thu, 24 Jun 2021 07:25:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 24 Jun 2021 07:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 07:25:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14b3189ef30e120910a62a83035bb35be5ad21d868baa15635cd4093e57b28`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fbbe41540f8564924d1bbf33810a5cca942d52258a07a9a0a9fa47d3e2ee4d`  
		Last Modified: Thu, 24 Jun 2021 07:26:44 GMT  
		Size: 1.8 MB (1759528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6efa0bc06b8244fc2b99086aaab3707ad97a5c1562d486c49f2643704d4c14f`  
		Last Modified: Thu, 24 Jun 2021 07:26:47 GMT  
		Size: 5.3 MB (5285807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf51d89722279aa5fe979daa99ecca041af3e85c0ecb284c9eef346e12a8525`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ce586c187940aa96e929532b8802dd2d2590ae0629d8d6ff5683defad7d791`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:54c06566e53ed883f540aac6ef04c0b592bd490887621be35c1089106b697e7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39524856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57d64ff238cc272cd4b46a7dcb066e80d77dded09ac13be158b57ebddfb9be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 20:10:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 25 Jun 2021 20:10:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 20:10:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 20:13:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 25 Jun 2021 20:13:47 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 20:13:51 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 20:13:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 20:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 20:14:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4850a05a8ee69386fd934aa7e803a6ab5114a463b2f67029a79345a3e2258215`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65420b8b6a00225fef8990d8f2bb04ac6297f210d1018a7d55ad7a16bd40f78`  
		Last Modified: Fri, 25 Jun 2021 20:15:59 GMT  
		Size: 2.2 MB (2225168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ed66b43cf8ca387a94faaeafe401ad9c331b2d56b9cf2a01dfd4a4df32246`  
		Last Modified: Fri, 25 Jun 2021 20:16:00 GMT  
		Size: 6.7 MB (6743843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a2bd0b6c1fefb2ef43012c2c366d9194597f452679f46c376dec153b5be885`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc82701a4e5b97700db148e5c577a64a955835728f7ed57cc58a7306a6e0b21`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:1054032dfae72f0807214d0751246c6675a4527de4b0af06446b9ed3281c5ff9
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
$ docker pull spiped@sha256:77bb7048879f502a0be6947d6ded556dedd56bfbd65846f202ddbae6c0220f84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecec5286e75ac64570dd86ae159bec30df6ff4bb0ecc79f42dd8a5c7126be6eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:41:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:41:21 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:41:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:03:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:03:03 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:03:03 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:03:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:03:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc49c1d100974d70cd457c65f0e781af958b9d07a56e03267424f0d11990712`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3e43d8c62d03bca76a106e58c3099bd76fb7fbad003082a81a3670c07ba69`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdfa185ef47533e780a1502b6ecf0f1486cc0955b4930432fdfdc77813e9d50`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 212.6 KB (212559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241cc499201ce5b553c5be7e1b77bfddb66137711a90180f2e25689109405751`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d6882fdc5e95f3b1481ffb5d149c0fda3dc71d8fa51eba15edc3be50dc54c`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b758b42acbf998e5a39dc12204e0be903d69a2af37753e5d2133b5df87b06523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2835923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae8ff3806515f364a387402ad57b51af1f948f849240b2e704a6de2c048ada9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 00:21:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Jun 2021 00:21:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Jun 2021 00:21:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:38:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:38:07 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:38:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:38:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9e2daf3ec825cb3613604aa1365dbe414dc4e91784135871c1b1dfc68db23d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101fbc0ffdf60230b896427f198bc223946522d7d1f77e2275181837980568d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296999154521c5c6c6c67a405f842cacada3793a86c889ce922a114bae5354a6`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 202.5 KB (202495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c40bed8d80ea82bb949a3747badad3421eb16ea2e2440962324c9d79ab00b`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd55faef8cc92525b1be13e1e39b9ee16e5caaf2df3e0db276ed2683a509da9`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:57f8db33a0eec466bfc76dd17cee895a03a3789dbd31bd89ef2e8dc7da3455e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2632718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676e5f41ec430a6e87108a46dd408d068f0e501170755f72925c7a760ed458ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 07:25:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 24 Jun 2021 07:25:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 24 Jun 2021 07:25:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:17:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:17:30 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:17:30 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:17:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:17:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c429d40f3f855015d365208d1b968cd8f34de9ccedd71360b7f05eab24ddd1`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4522338918253627f69a56835ddb741f10f29e2de17157de4ca03a12561d3e05`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f4ce029c4b37ef76a46da093755b9e24c2d0765592fd00547e013edf3479c`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 195.8 KB (195767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10cb1e83ae0b13c5adcff700076e63bf3322c49067170f59c7ec0c9d6f0698f`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e1913bac6b271f9c4b484fad7338dcbc98a4526b6e48bf1f6a8ccb3fa3b9a`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:40541478eb401d67036d56bbd4cfd5933f148ce155f8e3292a4d083fbb62ba19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2923277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02b54f6f7a1b548ed3db2fc33cafcbb8ef9b27d6ae45811deeb5ecf484a3d75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:54:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:54:08 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:54:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:54:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:54:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a6e447f49f6576247dd515ff88f610088fde09c8c378492a19009d6f6fd3b`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05549f8a714910bf1ba795919183eda4ed8c6c1dacd25e27d16f60e584efd239`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b70a09132ff271f43729154235e305beed323f6f44bb8f91d3f71be66c9f58`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 204.6 KB (204616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf3cdb40c67131120870a15e3902a71c8b1db82a03999be16d35d7d6ae59309`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17f3d198dd5104ea91d70276d05d71182af08cf309adc75a3b64bd770c1699`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:041a4401f89326839b354e7fb7aeb38b07f545fab3de4c84dc0c8f9cebefacca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f94b397232ecc82d13aa208dbbe6e5a315e7a44a1d284fc0089f766e22aea2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:55:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:55:36 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:55:37 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:55:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:55:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8a1adc7e61a91c39fcba896b070192f506dd419fc77a733ce377c563448785`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982f88ff86958b26737edc45adbf2bf850db25cdc970e348723b0d305f5f6db2`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24fe46b36c0cdba759eaf8ea030281f67337289db167fb4d8d3b7da3e191680`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 223.4 KB (223438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb79119bc0cf80b5d4a32e3035a171c2c43177ce8bd6cf5f6ad53da848ae22`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027751b1d208d42e1c73a3526f36a885067bd323348563fb1186928a536a01a`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:1054032dfae72f0807214d0751246c6675a4527de4b0af06446b9ed3281c5ff9
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
$ docker pull spiped@sha256:77bb7048879f502a0be6947d6ded556dedd56bfbd65846f202ddbae6c0220f84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecec5286e75ac64570dd86ae159bec30df6ff4bb0ecc79f42dd8a5c7126be6eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:41:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:41:21 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:41:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:03:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:03:03 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:03:03 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:03:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:03:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc49c1d100974d70cd457c65f0e781af958b9d07a56e03267424f0d11990712`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3e43d8c62d03bca76a106e58c3099bd76fb7fbad003082a81a3670c07ba69`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdfa185ef47533e780a1502b6ecf0f1486cc0955b4930432fdfdc77813e9d50`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 212.6 KB (212559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241cc499201ce5b553c5be7e1b77bfddb66137711a90180f2e25689109405751`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d6882fdc5e95f3b1481ffb5d149c0fda3dc71d8fa51eba15edc3be50dc54c`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b758b42acbf998e5a39dc12204e0be903d69a2af37753e5d2133b5df87b06523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2835923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae8ff3806515f364a387402ad57b51af1f948f849240b2e704a6de2c048ada9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 00:21:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Jun 2021 00:21:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Jun 2021 00:21:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:38:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:38:07 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:38:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:38:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9e2daf3ec825cb3613604aa1365dbe414dc4e91784135871c1b1dfc68db23d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101fbc0ffdf60230b896427f198bc223946522d7d1f77e2275181837980568d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296999154521c5c6c6c67a405f842cacada3793a86c889ce922a114bae5354a6`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 202.5 KB (202495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c40bed8d80ea82bb949a3747badad3421eb16ea2e2440962324c9d79ab00b`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd55faef8cc92525b1be13e1e39b9ee16e5caaf2df3e0db276ed2683a509da9`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:57f8db33a0eec466bfc76dd17cee895a03a3789dbd31bd89ef2e8dc7da3455e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2632718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676e5f41ec430a6e87108a46dd408d068f0e501170755f72925c7a760ed458ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 07:25:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 24 Jun 2021 07:25:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 24 Jun 2021 07:25:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:17:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:17:30 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:17:30 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:17:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:17:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c429d40f3f855015d365208d1b968cd8f34de9ccedd71360b7f05eab24ddd1`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4522338918253627f69a56835ddb741f10f29e2de17157de4ca03a12561d3e05`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f4ce029c4b37ef76a46da093755b9e24c2d0765592fd00547e013edf3479c`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 195.8 KB (195767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10cb1e83ae0b13c5adcff700076e63bf3322c49067170f59c7ec0c9d6f0698f`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e1913bac6b271f9c4b484fad7338dcbc98a4526b6e48bf1f6a8ccb3fa3b9a`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:40541478eb401d67036d56bbd4cfd5933f148ce155f8e3292a4d083fbb62ba19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2923277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02b54f6f7a1b548ed3db2fc33cafcbb8ef9b27d6ae45811deeb5ecf484a3d75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:54:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:54:08 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:54:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:54:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:54:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a6e447f49f6576247dd515ff88f610088fde09c8c378492a19009d6f6fd3b`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05549f8a714910bf1ba795919183eda4ed8c6c1dacd25e27d16f60e584efd239`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b70a09132ff271f43729154235e305beed323f6f44bb8f91d3f71be66c9f58`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 204.6 KB (204616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf3cdb40c67131120870a15e3902a71c8b1db82a03999be16d35d7d6ae59309`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17f3d198dd5104ea91d70276d05d71182af08cf309adc75a3b64bd770c1699`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:041a4401f89326839b354e7fb7aeb38b07f545fab3de4c84dc0c8f9cebefacca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f94b397232ecc82d13aa208dbbe6e5a315e7a44a1d284fc0089f766e22aea2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:55:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:55:36 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:55:37 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:55:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:55:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8a1adc7e61a91c39fcba896b070192f506dd419fc77a733ce377c563448785`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982f88ff86958b26737edc45adbf2bf850db25cdc970e348723b0d305f5f6db2`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24fe46b36c0cdba759eaf8ea030281f67337289db167fb4d8d3b7da3e191680`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 223.4 KB (223438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb79119bc0cf80b5d4a32e3035a171c2c43177ce8bd6cf5f6ad53da848ae22`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027751b1d208d42e1c73a3526f36a885067bd323348563fb1186928a536a01a`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:e3956f14538b744b8891f7b3ca25f5bebc25191e0c09c7191a5ca5245d6bcca0
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
$ docker pull spiped@sha256:c8fcd50e24a2fac4210299a2ee03f0d8d0de3a6e51ba6f61a56c263f16a82fd4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29793592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5275d81bc421af6ac42959ab8c655ffe4f05b57d6f87325b371cbe74019778`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 07:24:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 24 Jun 2021 07:24:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 07:24:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 24 Jun 2021 07:25:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 24 Jun 2021 07:25:32 GMT
VOLUME [/spiped]
# Thu, 24 Jun 2021 07:25:33 GMT
WORKDIR /spiped
# Thu, 24 Jun 2021 07:25:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 24 Jun 2021 07:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 07:25:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14b3189ef30e120910a62a83035bb35be5ad21d868baa15635cd4093e57b28`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fbbe41540f8564924d1bbf33810a5cca942d52258a07a9a0a9fa47d3e2ee4d`  
		Last Modified: Thu, 24 Jun 2021 07:26:44 GMT  
		Size: 1.8 MB (1759528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6efa0bc06b8244fc2b99086aaab3707ad97a5c1562d486c49f2643704d4c14f`  
		Last Modified: Thu, 24 Jun 2021 07:26:47 GMT  
		Size: 5.3 MB (5285807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf51d89722279aa5fe979daa99ecca041af3e85c0ecb284c9eef346e12a8525`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ce586c187940aa96e929532b8802dd2d2590ae0629d8d6ff5683defad7d791`  
		Last Modified: Thu, 24 Jun 2021 07:26:43 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:54c06566e53ed883f540aac6ef04c0b592bd490887621be35c1089106b697e7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39524856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57d64ff238cc272cd4b46a7dcb066e80d77dded09ac13be158b57ebddfb9be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 20:10:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 25 Jun 2021 20:10:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 20:10:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 20:13:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 25 Jun 2021 20:13:47 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 20:13:51 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 20:13:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 20:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 20:14:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4850a05a8ee69386fd934aa7e803a6ab5114a463b2f67029a79345a3e2258215`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65420b8b6a00225fef8990d8f2bb04ac6297f210d1018a7d55ad7a16bd40f78`  
		Last Modified: Fri, 25 Jun 2021 20:15:59 GMT  
		Size: 2.2 MB (2225168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ed66b43cf8ca387a94faaeafe401ad9c331b2d56b9cf2a01dfd4a4df32246`  
		Last Modified: Fri, 25 Jun 2021 20:16:00 GMT  
		Size: 6.7 MB (6743843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a2bd0b6c1fefb2ef43012c2c366d9194597f452679f46c376dec153b5be885`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc82701a4e5b97700db148e5c577a64a955835728f7ed57cc58a7306a6e0b21`  
		Last Modified: Fri, 25 Jun 2021 20:15:58 GMT  
		Size: 341.0 B  
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
