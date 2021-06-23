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
