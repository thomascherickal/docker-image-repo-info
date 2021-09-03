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
$ docker pull spiped@sha256:6211c62aba90f5a091c3e8bf9fd958676ac9d75e01ba5b38d95df35bac823f5c
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
$ docker pull spiped@sha256:d779db31393bf73bb7a45ab8a3e8f547216d6a0abbaa630fe44332adefc6f054
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37324937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306415ec98a85eb9753b91a8c6c8d4f25c43dd898da213370452cde68fd6125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:40 GMT
ADD file:5e8343ab9a73edc27c2889634896e792ab289b85c206de0fc31183fdc0a32ac7 in / 
# Tue, 17 Aug 2021 01:23:41 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:05:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 15:05:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:05:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 15:06:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 15:06:25 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 15:06:25 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 15:06:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 15:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 15:06:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99046ad9247f8a1cbd1048d9099d026191ad9cda63c08aadeb704b7000a51717`  
		Last Modified: Tue, 17 Aug 2021 01:29:35 GMT  
		Size: 31.4 MB (31361314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc464d0b8e823e26756d296bc514c2d5b282b5ab89630b586934ee6cb2a037ff`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d965e596cfe4edd8ac0758b349deab04685e0808f972fed94586afdb1adb57`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfffba101beb13e886e681ef1388d2f2df4a89c8ac5c6b7f35ec01506bd2f1c`  
		Last Modified: Tue, 17 Aug 2021 15:06:54 GMT  
		Size: 6.0 MB (5960364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903fa4411c463574fad05212e81bea73cf8f1310ced1b8b733d706a371e89e74`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13bd7a2594aff90e0447dbe191de68e7a9f0074848194a7833d0819a330dd4f`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d2b531d8f0a42f8007d557790380594037ed5a3187dcda60468ba6f7b205a3f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33932544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25830ba5d141ad6cd8b98286a5cd9a1815be8f4783bec5b75a895cd325b7756`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:48 GMT
ADD file:9ab41fbe9b84c147eb71d451b4d31f27a0eb362bb6d14ee3ba6279d67ae25531 in / 
# Tue, 17 Aug 2021 01:55:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 17:44:38 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 17:44:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 17:44:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 17:45:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 17:45:50 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 17:45:50 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 17:45:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 17:45:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 17:45:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91b48139ec3e0280b0a9be84b502b3d6394149000106be38ac11a1c31b59d956`  
		Last Modified: Tue, 17 Aug 2021 02:11:08 GMT  
		Size: 28.9 MB (28904169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529af9182deb82a91ca1183e2f07ecae36ac80f65deb9aff5fc00aefe37b6cc9`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ff236190840487b8990652b37a3a02c6e5d5b21abc3955ab978f2431daea0b`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736ab94697c6fe32a81e259b0b22e03fa3ac4a224f1cf6be8647408d9c5dc2c4`  
		Last Modified: Tue, 17 Aug 2021 17:46:32 GMT  
		Size: 5.0 MB (5025125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521e8718ebe2c738541e1e87062916db439105c9e6bb71a5620be53f30384b46`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da9926511e4c596a58c07504e57c175041264b8361b4a900adb663d63fbbc8`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:82c3c2ebe3bd31cb51b8698b02fed6c6c8ddababab59c49902dbfb838fde261a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31314263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a771171769e644813614e8ec5270e93b93c509715bd5b1d357f8536dbe89c16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:16 GMT
ADD file:56b22dfd365932a88a68ec72e6b9c1af8c5747606e0387a2c189dfb49998d029 in / 
# Tue, 17 Aug 2021 02:13:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 21:12:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 21:12:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 21:12:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 21:13:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 21:13:41 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 21:13:41 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 21:13:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 21:13:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 21:13:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:118503c5404bba02cc6a70fd0b808c846fefe8a3435d831a37127a6fdc8f96a2`  
		Last Modified: Tue, 17 Aug 2021 02:29:31 GMT  
		Size: 26.6 MB (26565574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c45a3e608c37966ffad43edbc665486402dd651491b7a21297039852eafb658`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c41d652aa1399132c065b29940395b49fe97738bf2020b48ecb6861757d884`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0c590b6187a7f7de3a81cb5f71d2bece146d195f838c9c5e7134c614f60675`  
		Last Modified: Tue, 17 Aug 2021 21:14:58 GMT  
		Size: 4.7 MB (4745433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a95b0f4e791c265d50fe017d3ecfa55e9266c4d89fbf2c7761a16c78ba77a`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a04c9a6b135c00d4d849bb7249448c25c40eb54fa8dea1e0237ac82791eb2d`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:a8cb1de1b7ac27edc9001452b532e01129969840f12809227cb60400cc4e39a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35316841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac4558f48bddf4104b4828089d6aa2d9e1b3b223116b94d9e70f8d17bcd91fa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:04 GMT
ADD file:0a42d4a201f0ac7889187c3212fbdfc2747f31f36e690d59c22eec50fe542614 in / 
# Tue, 17 Aug 2021 01:46:05 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:05:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 12:05:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:05:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 12:06:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 12:06:07 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 12:06:07 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 12:06:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 12:06:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 12:06:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3716b9f3c2f9e7592f5b47c2e6e13e64132071620c7551e0aa3c5c248e106139`  
		Last Modified: Tue, 17 Aug 2021 01:53:29 GMT  
		Size: 30.0 MB (30048801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d1e840bed4d3d0ccdf6507f2f244340722bfccf593ec463750eae2b86ea83d`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f75e45873615f57906ab6bd8be8065a16bfc73e217ef9b96e7ff0170ea02e43`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e964d1a9f206f9e8026c7b4c594b686d9ec49d8d9ed8e8cbda8d1437bd77ff4`  
		Last Modified: Tue, 17 Aug 2021 12:06:40 GMT  
		Size: 5.3 MB (5264787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce44b119695cd419968d21d74d37482f3bbe86cca3432a4f284309bac2d55ba`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31893ecc983ab9a027f5aae03453a9bd6611eed642bd73ac2b9d14a4b292ba90`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:51db9ecb4b19727e637474ec3edcbee6a3f8b10cf9849e1bb18e4de26e9d1cf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40262874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aea617771607db5094f062cd1b36f273130f573f444293d5b8bf8f6ca4ba586e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:28 GMT
ADD file:9afc107c0880864c9f16852bb6cc272a068f2c82a2df7c3444bbbc533f377156 in / 
# Tue, 17 Aug 2021 01:40:29 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 17:17:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 17:18:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 17:18:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 17:18:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 17:18:34 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 17:18:34 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 17:18:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 17:18:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 17:18:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6edd81381c438b83d2749dc056d46cd53320e27fb010b3e931ca1f0a752ddc07`  
		Last Modified: Tue, 17 Aug 2021 01:49:56 GMT  
		Size: 32.4 MB (32375657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f073609c1b59b4b496ff4cd4329461daeba813c650c1439397561fa937e53c`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9070386f59e19b077a8c2157fb94a95e2366a8845ed5505eb3fe31214209fae`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceead4902ad3c822b58360ac4f18d6861f2d214f601abc65685d657b693e810`  
		Last Modified: Tue, 17 Aug 2021 17:19:15 GMT  
		Size: 7.9 MB (7883966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16e38803b194f569d38caf69675f72659a74604c89befeafb476b657afe3146`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6da0e93b70ab4a38a695f1a65d884a2c6fdfe7ea92f45d91e2a962e3c89b141`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:d945e41b8d4bd950e1be63af3f3229ac00be11b318b361a3beffc50e7ef0eaac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2581ff16e0a3ffb4037d0c23b704ece31bb583ffa283a4f1bb062d42ba3def7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:01 GMT
ADD file:e842559443fb9351f1a9ac9ce03dfe0b069d8b9c3409f8d9b21abcbdc2a437c5 in / 
# Fri, 03 Sep 2021 01:10:02 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:42:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 03 Sep 2021 01:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:42:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 03 Sep 2021 01:43:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 03 Sep 2021 01:43:33 GMT
VOLUME [/spiped]
# Fri, 03 Sep 2021 01:43:33 GMT
WORKDIR /spiped
# Fri, 03 Sep 2021 01:43:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 03 Sep 2021 01:43:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 01:43:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2320664dc3760d5d905a15eef2bf52da0cbab097fb4fc626c1f96722a2e2188c`  
		Last Modified: Fri, 03 Sep 2021 01:18:25 GMT  
		Size: 29.6 MB (29627416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18f077ba2ec335663d52307f6bfd922f985212d8fa94ecb63cb11050a8f3314`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d948a422c2276c40a4832dee38f347f364a0a1c2b3f5d0c1df29141d7fb1492`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46b33b2146e543c4306686645f91f5627385bf944b5ea340c691c7aa580f37c`  
		Last Modified: Fri, 03 Sep 2021 01:44:00 GMT  
		Size: 5.7 MB (5706047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808267f420422a78f98748362d203d41a9e7033571d62e15511faac06294aebc`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcfb83ee5525340e79d5b08f1809304f00d86ed6570a024a41fa23424e3760b`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:eb4b77221b29aca3170128d240159baca14887a971ae076251bba0b9cc49f493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41268765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df33ed783b716cb0f12e35a85b119a6dfb68665722c2cb9b7fbcf3c98404f6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:09 GMT
ADD file:b7348f0e1a41ce54354496488a0ee8bb949743444973dc6ab51ea80926f596f2 in / 
# Tue, 17 Aug 2021 01:33:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 16:29:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 16:29:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 16:29:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 16:32:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 16:32:20 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 16:32:26 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 16:32:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 16:32:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 16:32:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:80e30391b3a42f13bd8cb2b497506fa7a23b074d43f7446d94b06514e408020b`  
		Last Modified: Tue, 17 Aug 2021 01:46:01 GMT  
		Size: 35.3 MB (35264011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60929bf2df877410036f8525da51c93fc047d640fe7d71540bce092c2dbc3c3f`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a700ec7060ef93bf348dbb18aebd9b1065b822685cbf1f5d70efe88648fb7d4a`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d945be8f4c7314b6ac7aee0b27681d8890d66197b5376c96b23aa2534911589a`  
		Last Modified: Tue, 17 Aug 2021 16:33:20 GMT  
		Size: 6.0 MB (6001477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7914ec06b96350b2868d9788e0d8df35e4fdbed1ec14e573025bfeaaa37ec4d`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ceb8036a7f8603020bdab26c0cc2d6f074327d9295ecb58d17441ab98f960b`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:ef96b17d2a788c7bfb1d3838d6545d7f2c5b43cc8141107856c7cbd37eea1853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34834136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a087283bae8568adc0cf7b07e5eb5f24718cbafcdd6545ac0fb12315ccdd99e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:02 GMT
ADD file:9a849f976712983c3bf95c9d110ab1c38643273c19644a436242e8b8bd5eb225 in / 
# Tue, 17 Aug 2021 01:49:07 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:53:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 09:53:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:53:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 09:54:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 09:54:27 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 09:54:27 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 09:54:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 09:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:54:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:16c136b299a1426955abff4eb0ed556e3c2e8e67509fba84e416f1d5cc77189a`  
		Last Modified: Tue, 17 Aug 2021 01:57:33 GMT  
		Size: 29.6 MB (29647028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101ad9278b6e0a43e087711eaabf1f30721c9e7522020a583d5a3da6e16f3b4b`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3812b210386b50d3cb22925b3646ab61d16da033fd61ecbe3768c4e3e716d0`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436874c5caaa558dc75edb5e309ac884c077ca1b6c376902ad4e2d6b7b2157f9`  
		Last Modified: Tue, 17 Aug 2021 09:55:16 GMT  
		Size: 5.2 MB (5183847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea485d629322bebbea0f2d218fd81ce6928baba229a9097169b5cf111713ae36`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50377e04053d99e09a6cb5a363b98fc242cf892438537e805afda7c2fe7bfad`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:89f362dd004a510b0e2dfdfdf849444c25d6fb0c60e3b7df331ece34ce763a31
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
$ docker pull spiped@sha256:44015ddc42ceef8878c9b2bad7a6bcbf2b5d2ca42ab52cca20f9f66b2c15ffd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65d8337530e6b8e116202287d477945c4375886702df4698f8740106658a777`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:56:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:56:13 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:56:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:56:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:56:31 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:56:31 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:56:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:56:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:56:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72fe484884c949a7fba8b7d917cbe40b9fa50036f4c10e4b82e3075576fe3fc`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06083e8d35a44724cf84de43d971fb5b141e8ce6468a5c267c43c96f79869f23`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037fda176acae1eef93fa1dde784253576faf4d880c75c8d7df76fdf212dda`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 212.5 KB (212547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb3cd7f024c8cfa70e1c8e8f282e44395bbaa20cd69851af0552d8041deaea2`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fccea2af66d4ffdbdd93edf485c1e6e17f14ac10329842af6fea7741bd3504`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:7e548b9910cf9bcbce660ff537e09660dbd9d84cbc06621e45fb2282f2f52270
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2838978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8539d235dbd2d180f98df622ec1586ed595c7026c53f57b67876cbe0b641be9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:39:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:39:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:39:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:39:57 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:39:58 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:39:58 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:39:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:39:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:40:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ec865614b924d3ebd8faaf1468ff031de3ccb2f178656d907e4a89f8673776`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07908dc20812a0124cb96563b08ff2d4ebd32f0ca0cef02511faa0c127496e96`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 7.3 KB (7290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2ce7f8303145adfe2a17235c758d30fa18338c417eb73738b591c1dd3d1315`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 202.5 KB (202499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07f8ab6ed47190923d1d152d960c5fd80b7d9f27f84a289e8236a1e4f22843c`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17d0a64e682741c70413fc90f0d8a4dac61425dcc5c98ce054909120977e587`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:24d05f05df7127b2aa61654a9d29c77a0c2a00f8ba29dbfc127a672700d5f652
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2635217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c197156cacbfdbdb870ce3391ad1bdf7d6c922d18648489e7549033356f432b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 03:04:23 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 03:04:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 03:04:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 03:04:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 03:04:59 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 03:05:00 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 03:05:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 03:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 03:05:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c187e6961a8f3ae8bf645e1fbec375c4f7c3d8146ab5ee5a09f57cd5615f33cb`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56c389f9017243d26a8fd61b3cc3385e2b4dcf930d608cc682a5ff3b437137`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0da469457d5465481ffd06dc86cd457daaf02e8b501cbee7b9cb52b675525`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 195.8 KB (195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea4333c9f229866ca36ab2d7e036e1d23031e78c62c3ad0bcbbeacaaf8f8e65`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4907440a689992d3e1fbcc2fcef650c5ef7b7abe5b8b3aa9c97d6d697d5050fd`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:026d11edbbedc8b8a63207a745859b0ada912c11cbd6bf77d2eb162cfb1a6577
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7dbad85a08f79ca7ef7c449feb1dfbd6973498a21db9a0721af19e181fc39f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:45:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 01:45:36 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 01:45:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 01:45:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 01:45:53 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 01:45:53 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 01:45:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:45:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130a79b60aae9998377169e6355792370bb064e6148684353d6ed4826039492f`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43519aa40fdf82f3b05cab9731634890c7e8dc8b9731ce4c7c3fbbc35def0274`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 7.3 KB (7299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1b5762b7444935215ce9e31bc9a68cac110a8b0bf2f9ca433a2d78620fe35`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 204.6 KB (204622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156837dee9efeb5125ef7fc8d079ccf996015838cfe028bfb81695eb1230b99`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f221da4d2654d1b1432ad3c77afeed7392661b44c6a50fc1fd5e2cede5dfcb`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:da842be683e4aa6e7f0e6581d7d9bd1604d2d140a1b452e47a1ca595261af814
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3055327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7b5670b88fbd238447f1f65531173381d0aff05ec6d63ef2df4dfb7b8c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:35:24 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:35:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:35:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:35:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:35:45 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:35:45 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:35:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:35:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:35:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95070702ac27305ca355fc2880dec01d9e18d3c8a4a22842a599db59ea5467e0`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35be501885b2efd06479a1d05af31f0d06d6b0a5c4dfb3f760af81657d7919ea`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 7.3 KB (7287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f5e404d9d5a395b15445e0403dfa9a598ab9ecd02814798d33098ac6a8ba9c`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 223.4 KB (223445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b8287cb974321164bff4ca80e9a231471fecf0bbab1bbf130172709ae47ae`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c88353a13d0403b037e398aa01ea54701b91f2adf180d6ed9df1b155b62c89`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:3c83af52715b14ccfd27cc89b7b988ae73b9d05500efd053b99b027c0328f14d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59b6df7881927f19f4b2dcab5974d93c4284e7e9ba9c21098a82d888389b26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:36:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 27 Aug 2021 21:36:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 27 Aug 2021 21:37:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 27 Aug 2021 21:37:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 27 Aug 2021 21:37:41 GMT
VOLUME [/spiped]
# Fri, 27 Aug 2021 21:37:48 GMT
WORKDIR /spiped
# Fri, 27 Aug 2021 21:37:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:38:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f143c775bd94ef9de49da05aab2353301bc02ceb74a237332f8d9b23e193234b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9067169d42bea9851adf89b67776e5a280513855fb73120a8d2c5f0051a1097b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 7.3 KB (7292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe10232ba40d32a7b84a0fe16aa0a2b418d2bdf093335c9fbaf56b08e751c54e`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 221.2 KB (221238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c7d84f077aa3ad717767ac56d4b1ea509bc7a9c81e57e3f4e210fe09205ee9`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c90dd2a4fa5a2acd662ddc7f2ec01550257e4bbaae18ab7a94fdd288523cf8`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:3852ee4130c6bfe6eb29489ab1f82c2aceed2d65ba3a11477360199bd6ba4bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2817762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d772c7d45678813ce17e2e65d11aa3e23e0517de39acbfe03eaaadf3558b6f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 04:23:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 04:23:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 04:23:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 04:24:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 04:24:08 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 04:24:08 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 04:24:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 04:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 04:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a66831aa123cebdb722d7d1efb39f1ffb26129fdf9b8937935375852a206`  
		Last Modified: Sat, 28 Aug 2021 04:24:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b103bd0361f6fb48151c8780e205c3fde97140b66762b27effcf2c3b73c05c`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 7.3 KB (7283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce02139d2773db6b3c7033d9dbc6fdb427c918a69c29b8bb01669296d18c9fe`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 205.3 KB (205277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c3cb214e79007442b4d21bc48516c0ef35753d8db03a0cc129fa63d01bedde`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29859d07f0b507288c642deae1bae6cbe9d019152647a0c4e76bd86474fda106`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:6211c62aba90f5a091c3e8bf9fd958676ac9d75e01ba5b38d95df35bac823f5c
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
$ docker pull spiped@sha256:d779db31393bf73bb7a45ab8a3e8f547216d6a0abbaa630fe44332adefc6f054
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37324937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306415ec98a85eb9753b91a8c6c8d4f25c43dd898da213370452cde68fd6125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:40 GMT
ADD file:5e8343ab9a73edc27c2889634896e792ab289b85c206de0fc31183fdc0a32ac7 in / 
# Tue, 17 Aug 2021 01:23:41 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:05:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 15:05:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:05:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 15:06:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 15:06:25 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 15:06:25 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 15:06:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 15:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 15:06:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99046ad9247f8a1cbd1048d9099d026191ad9cda63c08aadeb704b7000a51717`  
		Last Modified: Tue, 17 Aug 2021 01:29:35 GMT  
		Size: 31.4 MB (31361314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc464d0b8e823e26756d296bc514c2d5b282b5ab89630b586934ee6cb2a037ff`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d965e596cfe4edd8ac0758b349deab04685e0808f972fed94586afdb1adb57`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfffba101beb13e886e681ef1388d2f2df4a89c8ac5c6b7f35ec01506bd2f1c`  
		Last Modified: Tue, 17 Aug 2021 15:06:54 GMT  
		Size: 6.0 MB (5960364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903fa4411c463574fad05212e81bea73cf8f1310ced1b8b733d706a371e89e74`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13bd7a2594aff90e0447dbe191de68e7a9f0074848194a7833d0819a330dd4f`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d2b531d8f0a42f8007d557790380594037ed5a3187dcda60468ba6f7b205a3f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33932544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25830ba5d141ad6cd8b98286a5cd9a1815be8f4783bec5b75a895cd325b7756`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:48 GMT
ADD file:9ab41fbe9b84c147eb71d451b4d31f27a0eb362bb6d14ee3ba6279d67ae25531 in / 
# Tue, 17 Aug 2021 01:55:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 17:44:38 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 17:44:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 17:44:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 17:45:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 17:45:50 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 17:45:50 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 17:45:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 17:45:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 17:45:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91b48139ec3e0280b0a9be84b502b3d6394149000106be38ac11a1c31b59d956`  
		Last Modified: Tue, 17 Aug 2021 02:11:08 GMT  
		Size: 28.9 MB (28904169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529af9182deb82a91ca1183e2f07ecae36ac80f65deb9aff5fc00aefe37b6cc9`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ff236190840487b8990652b37a3a02c6e5d5b21abc3955ab978f2431daea0b`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736ab94697c6fe32a81e259b0b22e03fa3ac4a224f1cf6be8647408d9c5dc2c4`  
		Last Modified: Tue, 17 Aug 2021 17:46:32 GMT  
		Size: 5.0 MB (5025125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521e8718ebe2c738541e1e87062916db439105c9e6bb71a5620be53f30384b46`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da9926511e4c596a58c07504e57c175041264b8361b4a900adb663d63fbbc8`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:82c3c2ebe3bd31cb51b8698b02fed6c6c8ddababab59c49902dbfb838fde261a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31314263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a771171769e644813614e8ec5270e93b93c509715bd5b1d357f8536dbe89c16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:16 GMT
ADD file:56b22dfd365932a88a68ec72e6b9c1af8c5747606e0387a2c189dfb49998d029 in / 
# Tue, 17 Aug 2021 02:13:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 21:12:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 21:12:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 21:12:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 21:13:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 21:13:41 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 21:13:41 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 21:13:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 21:13:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 21:13:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:118503c5404bba02cc6a70fd0b808c846fefe8a3435d831a37127a6fdc8f96a2`  
		Last Modified: Tue, 17 Aug 2021 02:29:31 GMT  
		Size: 26.6 MB (26565574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c45a3e608c37966ffad43edbc665486402dd651491b7a21297039852eafb658`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c41d652aa1399132c065b29940395b49fe97738bf2020b48ecb6861757d884`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0c590b6187a7f7de3a81cb5f71d2bece146d195f838c9c5e7134c614f60675`  
		Last Modified: Tue, 17 Aug 2021 21:14:58 GMT  
		Size: 4.7 MB (4745433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a95b0f4e791c265d50fe017d3ecfa55e9266c4d89fbf2c7761a16c78ba77a`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a04c9a6b135c00d4d849bb7249448c25c40eb54fa8dea1e0237ac82791eb2d`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:a8cb1de1b7ac27edc9001452b532e01129969840f12809227cb60400cc4e39a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35316841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac4558f48bddf4104b4828089d6aa2d9e1b3b223116b94d9e70f8d17bcd91fa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:04 GMT
ADD file:0a42d4a201f0ac7889187c3212fbdfc2747f31f36e690d59c22eec50fe542614 in / 
# Tue, 17 Aug 2021 01:46:05 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:05:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 12:05:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:05:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 12:06:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 12:06:07 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 12:06:07 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 12:06:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 12:06:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 12:06:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3716b9f3c2f9e7592f5b47c2e6e13e64132071620c7551e0aa3c5c248e106139`  
		Last Modified: Tue, 17 Aug 2021 01:53:29 GMT  
		Size: 30.0 MB (30048801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d1e840bed4d3d0ccdf6507f2f244340722bfccf593ec463750eae2b86ea83d`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f75e45873615f57906ab6bd8be8065a16bfc73e217ef9b96e7ff0170ea02e43`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e964d1a9f206f9e8026c7b4c594b686d9ec49d8d9ed8e8cbda8d1437bd77ff4`  
		Last Modified: Tue, 17 Aug 2021 12:06:40 GMT  
		Size: 5.3 MB (5264787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce44b119695cd419968d21d74d37482f3bbe86cca3432a4f284309bac2d55ba`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31893ecc983ab9a027f5aae03453a9bd6611eed642bd73ac2b9d14a4b292ba90`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:51db9ecb4b19727e637474ec3edcbee6a3f8b10cf9849e1bb18e4de26e9d1cf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40262874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aea617771607db5094f062cd1b36f273130f573f444293d5b8bf8f6ca4ba586e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:28 GMT
ADD file:9afc107c0880864c9f16852bb6cc272a068f2c82a2df7c3444bbbc533f377156 in / 
# Tue, 17 Aug 2021 01:40:29 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 17:17:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 17:18:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 17:18:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 17:18:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 17:18:34 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 17:18:34 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 17:18:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 17:18:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 17:18:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6edd81381c438b83d2749dc056d46cd53320e27fb010b3e931ca1f0a752ddc07`  
		Last Modified: Tue, 17 Aug 2021 01:49:56 GMT  
		Size: 32.4 MB (32375657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f073609c1b59b4b496ff4cd4329461daeba813c650c1439397561fa937e53c`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9070386f59e19b077a8c2157fb94a95e2366a8845ed5505eb3fe31214209fae`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceead4902ad3c822b58360ac4f18d6861f2d214f601abc65685d657b693e810`  
		Last Modified: Tue, 17 Aug 2021 17:19:15 GMT  
		Size: 7.9 MB (7883966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16e38803b194f569d38caf69675f72659a74604c89befeafb476b657afe3146`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6da0e93b70ab4a38a695f1a65d884a2c6fdfe7ea92f45d91e2a962e3c89b141`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:d945e41b8d4bd950e1be63af3f3229ac00be11b318b361a3beffc50e7ef0eaac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2581ff16e0a3ffb4037d0c23b704ece31bb583ffa283a4f1bb062d42ba3def7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:01 GMT
ADD file:e842559443fb9351f1a9ac9ce03dfe0b069d8b9c3409f8d9b21abcbdc2a437c5 in / 
# Fri, 03 Sep 2021 01:10:02 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:42:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 03 Sep 2021 01:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:42:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 03 Sep 2021 01:43:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 03 Sep 2021 01:43:33 GMT
VOLUME [/spiped]
# Fri, 03 Sep 2021 01:43:33 GMT
WORKDIR /spiped
# Fri, 03 Sep 2021 01:43:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 03 Sep 2021 01:43:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 01:43:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2320664dc3760d5d905a15eef2bf52da0cbab097fb4fc626c1f96722a2e2188c`  
		Last Modified: Fri, 03 Sep 2021 01:18:25 GMT  
		Size: 29.6 MB (29627416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18f077ba2ec335663d52307f6bfd922f985212d8fa94ecb63cb11050a8f3314`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d948a422c2276c40a4832dee38f347f364a0a1c2b3f5d0c1df29141d7fb1492`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46b33b2146e543c4306686645f91f5627385bf944b5ea340c691c7aa580f37c`  
		Last Modified: Fri, 03 Sep 2021 01:44:00 GMT  
		Size: 5.7 MB (5706047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808267f420422a78f98748362d203d41a9e7033571d62e15511faac06294aebc`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcfb83ee5525340e79d5b08f1809304f00d86ed6570a024a41fa23424e3760b`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:eb4b77221b29aca3170128d240159baca14887a971ae076251bba0b9cc49f493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41268765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df33ed783b716cb0f12e35a85b119a6dfb68665722c2cb9b7fbcf3c98404f6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:09 GMT
ADD file:b7348f0e1a41ce54354496488a0ee8bb949743444973dc6ab51ea80926f596f2 in / 
# Tue, 17 Aug 2021 01:33:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 16:29:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 16:29:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 16:29:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 16:32:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 16:32:20 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 16:32:26 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 16:32:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 16:32:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 16:32:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:80e30391b3a42f13bd8cb2b497506fa7a23b074d43f7446d94b06514e408020b`  
		Last Modified: Tue, 17 Aug 2021 01:46:01 GMT  
		Size: 35.3 MB (35264011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60929bf2df877410036f8525da51c93fc047d640fe7d71540bce092c2dbc3c3f`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a700ec7060ef93bf348dbb18aebd9b1065b822685cbf1f5d70efe88648fb7d4a`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d945be8f4c7314b6ac7aee0b27681d8890d66197b5376c96b23aa2534911589a`  
		Last Modified: Tue, 17 Aug 2021 16:33:20 GMT  
		Size: 6.0 MB (6001477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7914ec06b96350b2868d9788e0d8df35e4fdbed1ec14e573025bfeaaa37ec4d`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ceb8036a7f8603020bdab26c0cc2d6f074327d9295ecb58d17441ab98f960b`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:ef96b17d2a788c7bfb1d3838d6545d7f2c5b43cc8141107856c7cbd37eea1853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34834136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a087283bae8568adc0cf7b07e5eb5f24718cbafcdd6545ac0fb12315ccdd99e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:02 GMT
ADD file:9a849f976712983c3bf95c9d110ab1c38643273c19644a436242e8b8bd5eb225 in / 
# Tue, 17 Aug 2021 01:49:07 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:53:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 09:53:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:53:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 09:54:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 09:54:27 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 09:54:27 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 09:54:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 09:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:54:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:16c136b299a1426955abff4eb0ed556e3c2e8e67509fba84e416f1d5cc77189a`  
		Last Modified: Tue, 17 Aug 2021 01:57:33 GMT  
		Size: 29.6 MB (29647028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101ad9278b6e0a43e087711eaabf1f30721c9e7522020a583d5a3da6e16f3b4b`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3812b210386b50d3cb22925b3646ab61d16da033fd61ecbe3768c4e3e716d0`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436874c5caaa558dc75edb5e309ac884c077ca1b6c376902ad4e2d6b7b2157f9`  
		Last Modified: Tue, 17 Aug 2021 09:55:16 GMT  
		Size: 5.2 MB (5183847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea485d629322bebbea0f2d218fd81ce6928baba229a9097169b5cf111713ae36`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50377e04053d99e09a6cb5a363b98fc242cf892438537e805afda7c2fe7bfad`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:89f362dd004a510b0e2dfdfdf849444c25d6fb0c60e3b7df331ece34ce763a31
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
$ docker pull spiped@sha256:44015ddc42ceef8878c9b2bad7a6bcbf2b5d2ca42ab52cca20f9f66b2c15ffd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65d8337530e6b8e116202287d477945c4375886702df4698f8740106658a777`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:56:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:56:13 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:56:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:56:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:56:31 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:56:31 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:56:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:56:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:56:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72fe484884c949a7fba8b7d917cbe40b9fa50036f4c10e4b82e3075576fe3fc`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06083e8d35a44724cf84de43d971fb5b141e8ce6468a5c267c43c96f79869f23`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037fda176acae1eef93fa1dde784253576faf4d880c75c8d7df76fdf212dda`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 212.5 KB (212547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb3cd7f024c8cfa70e1c8e8f282e44395bbaa20cd69851af0552d8041deaea2`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fccea2af66d4ffdbdd93edf485c1e6e17f14ac10329842af6fea7741bd3504`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:7e548b9910cf9bcbce660ff537e09660dbd9d84cbc06621e45fb2282f2f52270
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2838978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8539d235dbd2d180f98df622ec1586ed595c7026c53f57b67876cbe0b641be9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:39:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:39:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:39:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:39:57 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:39:58 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:39:58 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:39:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:39:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:40:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ec865614b924d3ebd8faaf1468ff031de3ccb2f178656d907e4a89f8673776`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07908dc20812a0124cb96563b08ff2d4ebd32f0ca0cef02511faa0c127496e96`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 7.3 KB (7290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2ce7f8303145adfe2a17235c758d30fa18338c417eb73738b591c1dd3d1315`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 202.5 KB (202499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07f8ab6ed47190923d1d152d960c5fd80b7d9f27f84a289e8236a1e4f22843c`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17d0a64e682741c70413fc90f0d8a4dac61425dcc5c98ce054909120977e587`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:24d05f05df7127b2aa61654a9d29c77a0c2a00f8ba29dbfc127a672700d5f652
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2635217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c197156cacbfdbdb870ce3391ad1bdf7d6c922d18648489e7549033356f432b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 03:04:23 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 03:04:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 03:04:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 03:04:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 03:04:59 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 03:05:00 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 03:05:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 03:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 03:05:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c187e6961a8f3ae8bf645e1fbec375c4f7c3d8146ab5ee5a09f57cd5615f33cb`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56c389f9017243d26a8fd61b3cc3385e2b4dcf930d608cc682a5ff3b437137`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0da469457d5465481ffd06dc86cd457daaf02e8b501cbee7b9cb52b675525`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 195.8 KB (195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea4333c9f229866ca36ab2d7e036e1d23031e78c62c3ad0bcbbeacaaf8f8e65`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4907440a689992d3e1fbcc2fcef650c5ef7b7abe5b8b3aa9c97d6d697d5050fd`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:026d11edbbedc8b8a63207a745859b0ada912c11cbd6bf77d2eb162cfb1a6577
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7dbad85a08f79ca7ef7c449feb1dfbd6973498a21db9a0721af19e181fc39f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:45:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 01:45:36 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 01:45:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 01:45:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 01:45:53 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 01:45:53 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 01:45:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:45:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130a79b60aae9998377169e6355792370bb064e6148684353d6ed4826039492f`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43519aa40fdf82f3b05cab9731634890c7e8dc8b9731ce4c7c3fbbc35def0274`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 7.3 KB (7299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1b5762b7444935215ce9e31bc9a68cac110a8b0bf2f9ca433a2d78620fe35`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 204.6 KB (204622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156837dee9efeb5125ef7fc8d079ccf996015838cfe028bfb81695eb1230b99`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f221da4d2654d1b1432ad3c77afeed7392661b44c6a50fc1fd5e2cede5dfcb`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:da842be683e4aa6e7f0e6581d7d9bd1604d2d140a1b452e47a1ca595261af814
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3055327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7b5670b88fbd238447f1f65531173381d0aff05ec6d63ef2df4dfb7b8c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:35:24 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:35:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:35:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:35:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:35:45 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:35:45 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:35:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:35:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:35:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95070702ac27305ca355fc2880dec01d9e18d3c8a4a22842a599db59ea5467e0`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35be501885b2efd06479a1d05af31f0d06d6b0a5c4dfb3f760af81657d7919ea`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 7.3 KB (7287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f5e404d9d5a395b15445e0403dfa9a598ab9ecd02814798d33098ac6a8ba9c`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 223.4 KB (223445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b8287cb974321164bff4ca80e9a231471fecf0bbab1bbf130172709ae47ae`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c88353a13d0403b037e398aa01ea54701b91f2adf180d6ed9df1b155b62c89`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:3c83af52715b14ccfd27cc89b7b988ae73b9d05500efd053b99b027c0328f14d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59b6df7881927f19f4b2dcab5974d93c4284e7e9ba9c21098a82d888389b26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:36:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 27 Aug 2021 21:36:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 27 Aug 2021 21:37:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 27 Aug 2021 21:37:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 27 Aug 2021 21:37:41 GMT
VOLUME [/spiped]
# Fri, 27 Aug 2021 21:37:48 GMT
WORKDIR /spiped
# Fri, 27 Aug 2021 21:37:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:38:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f143c775bd94ef9de49da05aab2353301bc02ceb74a237332f8d9b23e193234b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9067169d42bea9851adf89b67776e5a280513855fb73120a8d2c5f0051a1097b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 7.3 KB (7292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe10232ba40d32a7b84a0fe16aa0a2b418d2bdf093335c9fbaf56b08e751c54e`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 221.2 KB (221238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c7d84f077aa3ad717767ac56d4b1ea509bc7a9c81e57e3f4e210fe09205ee9`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c90dd2a4fa5a2acd662ddc7f2ec01550257e4bbaae18ab7a94fdd288523cf8`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:3852ee4130c6bfe6eb29489ab1f82c2aceed2d65ba3a11477360199bd6ba4bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2817762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d772c7d45678813ce17e2e65d11aa3e23e0517de39acbfe03eaaadf3558b6f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 04:23:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 04:23:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 04:23:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 04:24:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 04:24:08 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 04:24:08 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 04:24:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 04:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 04:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a66831aa123cebdb722d7d1efb39f1ffb26129fdf9b8937935375852a206`  
		Last Modified: Sat, 28 Aug 2021 04:24:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b103bd0361f6fb48151c8780e205c3fde97140b66762b27effcf2c3b73c05c`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 7.3 KB (7283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce02139d2773db6b3c7033d9dbc6fdb427c918a69c29b8bb01669296d18c9fe`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 205.3 KB (205277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c3cb214e79007442b4d21bc48516c0ef35753d8db03a0cc129fa63d01bedde`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29859d07f0b507288c642deae1bae6cbe9d019152647a0c4e76bd86474fda106`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:6211c62aba90f5a091c3e8bf9fd958676ac9d75e01ba5b38d95df35bac823f5c
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

### `spiped:1.6.1` - linux; amd64

```console
$ docker pull spiped@sha256:d779db31393bf73bb7a45ab8a3e8f547216d6a0abbaa630fe44332adefc6f054
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37324937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306415ec98a85eb9753b91a8c6c8d4f25c43dd898da213370452cde68fd6125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:40 GMT
ADD file:5e8343ab9a73edc27c2889634896e792ab289b85c206de0fc31183fdc0a32ac7 in / 
# Tue, 17 Aug 2021 01:23:41 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:05:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 15:05:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:05:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 15:06:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 15:06:25 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 15:06:25 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 15:06:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 15:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 15:06:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99046ad9247f8a1cbd1048d9099d026191ad9cda63c08aadeb704b7000a51717`  
		Last Modified: Tue, 17 Aug 2021 01:29:35 GMT  
		Size: 31.4 MB (31361314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc464d0b8e823e26756d296bc514c2d5b282b5ab89630b586934ee6cb2a037ff`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d965e596cfe4edd8ac0758b349deab04685e0808f972fed94586afdb1adb57`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfffba101beb13e886e681ef1388d2f2df4a89c8ac5c6b7f35ec01506bd2f1c`  
		Last Modified: Tue, 17 Aug 2021 15:06:54 GMT  
		Size: 6.0 MB (5960364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903fa4411c463574fad05212e81bea73cf8f1310ced1b8b733d706a371e89e74`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13bd7a2594aff90e0447dbe191de68e7a9f0074848194a7833d0819a330dd4f`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d2b531d8f0a42f8007d557790380594037ed5a3187dcda60468ba6f7b205a3f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33932544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25830ba5d141ad6cd8b98286a5cd9a1815be8f4783bec5b75a895cd325b7756`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:48 GMT
ADD file:9ab41fbe9b84c147eb71d451b4d31f27a0eb362bb6d14ee3ba6279d67ae25531 in / 
# Tue, 17 Aug 2021 01:55:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 17:44:38 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 17:44:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 17:44:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 17:45:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 17:45:50 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 17:45:50 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 17:45:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 17:45:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 17:45:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91b48139ec3e0280b0a9be84b502b3d6394149000106be38ac11a1c31b59d956`  
		Last Modified: Tue, 17 Aug 2021 02:11:08 GMT  
		Size: 28.9 MB (28904169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529af9182deb82a91ca1183e2f07ecae36ac80f65deb9aff5fc00aefe37b6cc9`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ff236190840487b8990652b37a3a02c6e5d5b21abc3955ab978f2431daea0b`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736ab94697c6fe32a81e259b0b22e03fa3ac4a224f1cf6be8647408d9c5dc2c4`  
		Last Modified: Tue, 17 Aug 2021 17:46:32 GMT  
		Size: 5.0 MB (5025125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521e8718ebe2c738541e1e87062916db439105c9e6bb71a5620be53f30384b46`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da9926511e4c596a58c07504e57c175041264b8361b4a900adb663d63fbbc8`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:82c3c2ebe3bd31cb51b8698b02fed6c6c8ddababab59c49902dbfb838fde261a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31314263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a771171769e644813614e8ec5270e93b93c509715bd5b1d357f8536dbe89c16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:16 GMT
ADD file:56b22dfd365932a88a68ec72e6b9c1af8c5747606e0387a2c189dfb49998d029 in / 
# Tue, 17 Aug 2021 02:13:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 21:12:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 21:12:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 21:12:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 21:13:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 21:13:41 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 21:13:41 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 21:13:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 21:13:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 21:13:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:118503c5404bba02cc6a70fd0b808c846fefe8a3435d831a37127a6fdc8f96a2`  
		Last Modified: Tue, 17 Aug 2021 02:29:31 GMT  
		Size: 26.6 MB (26565574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c45a3e608c37966ffad43edbc665486402dd651491b7a21297039852eafb658`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c41d652aa1399132c065b29940395b49fe97738bf2020b48ecb6861757d884`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0c590b6187a7f7de3a81cb5f71d2bece146d195f838c9c5e7134c614f60675`  
		Last Modified: Tue, 17 Aug 2021 21:14:58 GMT  
		Size: 4.7 MB (4745433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a95b0f4e791c265d50fe017d3ecfa55e9266c4d89fbf2c7761a16c78ba77a`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a04c9a6b135c00d4d849bb7249448c25c40eb54fa8dea1e0237ac82791eb2d`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:a8cb1de1b7ac27edc9001452b532e01129969840f12809227cb60400cc4e39a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35316841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac4558f48bddf4104b4828089d6aa2d9e1b3b223116b94d9e70f8d17bcd91fa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:04 GMT
ADD file:0a42d4a201f0ac7889187c3212fbdfc2747f31f36e690d59c22eec50fe542614 in / 
# Tue, 17 Aug 2021 01:46:05 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:05:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 12:05:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:05:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 12:06:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 12:06:07 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 12:06:07 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 12:06:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 12:06:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 12:06:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3716b9f3c2f9e7592f5b47c2e6e13e64132071620c7551e0aa3c5c248e106139`  
		Last Modified: Tue, 17 Aug 2021 01:53:29 GMT  
		Size: 30.0 MB (30048801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d1e840bed4d3d0ccdf6507f2f244340722bfccf593ec463750eae2b86ea83d`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f75e45873615f57906ab6bd8be8065a16bfc73e217ef9b96e7ff0170ea02e43`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e964d1a9f206f9e8026c7b4c594b686d9ec49d8d9ed8e8cbda8d1437bd77ff4`  
		Last Modified: Tue, 17 Aug 2021 12:06:40 GMT  
		Size: 5.3 MB (5264787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce44b119695cd419968d21d74d37482f3bbe86cca3432a4f284309bac2d55ba`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31893ecc983ab9a027f5aae03453a9bd6611eed642bd73ac2b9d14a4b292ba90`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:51db9ecb4b19727e637474ec3edcbee6a3f8b10cf9849e1bb18e4de26e9d1cf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40262874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aea617771607db5094f062cd1b36f273130f573f444293d5b8bf8f6ca4ba586e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:28 GMT
ADD file:9afc107c0880864c9f16852bb6cc272a068f2c82a2df7c3444bbbc533f377156 in / 
# Tue, 17 Aug 2021 01:40:29 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 17:17:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 17:18:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 17:18:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 17:18:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 17:18:34 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 17:18:34 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 17:18:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 17:18:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 17:18:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6edd81381c438b83d2749dc056d46cd53320e27fb010b3e931ca1f0a752ddc07`  
		Last Modified: Tue, 17 Aug 2021 01:49:56 GMT  
		Size: 32.4 MB (32375657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f073609c1b59b4b496ff4cd4329461daeba813c650c1439397561fa937e53c`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9070386f59e19b077a8c2157fb94a95e2366a8845ed5505eb3fe31214209fae`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceead4902ad3c822b58360ac4f18d6861f2d214f601abc65685d657b693e810`  
		Last Modified: Tue, 17 Aug 2021 17:19:15 GMT  
		Size: 7.9 MB (7883966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16e38803b194f569d38caf69675f72659a74604c89befeafb476b657afe3146`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6da0e93b70ab4a38a695f1a65d884a2c6fdfe7ea92f45d91e2a962e3c89b141`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:d945e41b8d4bd950e1be63af3f3229ac00be11b318b361a3beffc50e7ef0eaac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2581ff16e0a3ffb4037d0c23b704ece31bb583ffa283a4f1bb062d42ba3def7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:01 GMT
ADD file:e842559443fb9351f1a9ac9ce03dfe0b069d8b9c3409f8d9b21abcbdc2a437c5 in / 
# Fri, 03 Sep 2021 01:10:02 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:42:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 03 Sep 2021 01:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:42:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 03 Sep 2021 01:43:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 03 Sep 2021 01:43:33 GMT
VOLUME [/spiped]
# Fri, 03 Sep 2021 01:43:33 GMT
WORKDIR /spiped
# Fri, 03 Sep 2021 01:43:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 03 Sep 2021 01:43:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 01:43:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2320664dc3760d5d905a15eef2bf52da0cbab097fb4fc626c1f96722a2e2188c`  
		Last Modified: Fri, 03 Sep 2021 01:18:25 GMT  
		Size: 29.6 MB (29627416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18f077ba2ec335663d52307f6bfd922f985212d8fa94ecb63cb11050a8f3314`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d948a422c2276c40a4832dee38f347f364a0a1c2b3f5d0c1df29141d7fb1492`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46b33b2146e543c4306686645f91f5627385bf944b5ea340c691c7aa580f37c`  
		Last Modified: Fri, 03 Sep 2021 01:44:00 GMT  
		Size: 5.7 MB (5706047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808267f420422a78f98748362d203d41a9e7033571d62e15511faac06294aebc`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcfb83ee5525340e79d5b08f1809304f00d86ed6570a024a41fa23424e3760b`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:eb4b77221b29aca3170128d240159baca14887a971ae076251bba0b9cc49f493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41268765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df33ed783b716cb0f12e35a85b119a6dfb68665722c2cb9b7fbcf3c98404f6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:09 GMT
ADD file:b7348f0e1a41ce54354496488a0ee8bb949743444973dc6ab51ea80926f596f2 in / 
# Tue, 17 Aug 2021 01:33:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 16:29:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 16:29:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 16:29:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 16:32:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 16:32:20 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 16:32:26 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 16:32:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 16:32:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 16:32:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:80e30391b3a42f13bd8cb2b497506fa7a23b074d43f7446d94b06514e408020b`  
		Last Modified: Tue, 17 Aug 2021 01:46:01 GMT  
		Size: 35.3 MB (35264011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60929bf2df877410036f8525da51c93fc047d640fe7d71540bce092c2dbc3c3f`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a700ec7060ef93bf348dbb18aebd9b1065b822685cbf1f5d70efe88648fb7d4a`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d945be8f4c7314b6ac7aee0b27681d8890d66197b5376c96b23aa2534911589a`  
		Last Modified: Tue, 17 Aug 2021 16:33:20 GMT  
		Size: 6.0 MB (6001477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7914ec06b96350b2868d9788e0d8df35e4fdbed1ec14e573025bfeaaa37ec4d`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ceb8036a7f8603020bdab26c0cc2d6f074327d9295ecb58d17441ab98f960b`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:ef96b17d2a788c7bfb1d3838d6545d7f2c5b43cc8141107856c7cbd37eea1853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34834136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a087283bae8568adc0cf7b07e5eb5f24718cbafcdd6545ac0fb12315ccdd99e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:02 GMT
ADD file:9a849f976712983c3bf95c9d110ab1c38643273c19644a436242e8b8bd5eb225 in / 
# Tue, 17 Aug 2021 01:49:07 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:53:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 09:53:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:53:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 09:54:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 09:54:27 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 09:54:27 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 09:54:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 09:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:54:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:16c136b299a1426955abff4eb0ed556e3c2e8e67509fba84e416f1d5cc77189a`  
		Last Modified: Tue, 17 Aug 2021 01:57:33 GMT  
		Size: 29.6 MB (29647028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101ad9278b6e0a43e087711eaabf1f30721c9e7522020a583d5a3da6e16f3b4b`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3812b210386b50d3cb22925b3646ab61d16da033fd61ecbe3768c4e3e716d0`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436874c5caaa558dc75edb5e309ac884c077ca1b6c376902ad4e2d6b7b2157f9`  
		Last Modified: Tue, 17 Aug 2021 09:55:16 GMT  
		Size: 5.2 MB (5183847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea485d629322bebbea0f2d218fd81ce6928baba229a9097169b5cf111713ae36`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50377e04053d99e09a6cb5a363b98fc242cf892438537e805afda7c2fe7bfad`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:89f362dd004a510b0e2dfdfdf849444c25d6fb0c60e3b7df331ece34ce763a31
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

### `spiped:1.6.1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:44015ddc42ceef8878c9b2bad7a6bcbf2b5d2ca42ab52cca20f9f66b2c15ffd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65d8337530e6b8e116202287d477945c4375886702df4698f8740106658a777`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:56:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:56:13 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:56:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:56:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:56:31 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:56:31 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:56:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:56:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:56:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72fe484884c949a7fba8b7d917cbe40b9fa50036f4c10e4b82e3075576fe3fc`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06083e8d35a44724cf84de43d971fb5b141e8ce6468a5c267c43c96f79869f23`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037fda176acae1eef93fa1dde784253576faf4d880c75c8d7df76fdf212dda`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 212.5 KB (212547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb3cd7f024c8cfa70e1c8e8f282e44395bbaa20cd69851af0552d8041deaea2`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fccea2af66d4ffdbdd93edf485c1e6e17f14ac10329842af6fea7741bd3504`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:7e548b9910cf9bcbce660ff537e09660dbd9d84cbc06621e45fb2282f2f52270
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2838978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8539d235dbd2d180f98df622ec1586ed595c7026c53f57b67876cbe0b641be9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:39:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:39:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:39:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:39:57 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:39:58 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:39:58 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:39:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:39:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:40:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ec865614b924d3ebd8faaf1468ff031de3ccb2f178656d907e4a89f8673776`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07908dc20812a0124cb96563b08ff2d4ebd32f0ca0cef02511faa0c127496e96`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 7.3 KB (7290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2ce7f8303145adfe2a17235c758d30fa18338c417eb73738b591c1dd3d1315`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 202.5 KB (202499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07f8ab6ed47190923d1d152d960c5fd80b7d9f27f84a289e8236a1e4f22843c`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17d0a64e682741c70413fc90f0d8a4dac61425dcc5c98ce054909120977e587`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:24d05f05df7127b2aa61654a9d29c77a0c2a00f8ba29dbfc127a672700d5f652
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2635217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c197156cacbfdbdb870ce3391ad1bdf7d6c922d18648489e7549033356f432b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 03:04:23 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 03:04:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 03:04:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 03:04:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 03:04:59 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 03:05:00 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 03:05:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 03:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 03:05:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c187e6961a8f3ae8bf645e1fbec375c4f7c3d8146ab5ee5a09f57cd5615f33cb`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56c389f9017243d26a8fd61b3cc3385e2b4dcf930d608cc682a5ff3b437137`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0da469457d5465481ffd06dc86cd457daaf02e8b501cbee7b9cb52b675525`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 195.8 KB (195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea4333c9f229866ca36ab2d7e036e1d23031e78c62c3ad0bcbbeacaaf8f8e65`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4907440a689992d3e1fbcc2fcef650c5ef7b7abe5b8b3aa9c97d6d697d5050fd`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:026d11edbbedc8b8a63207a745859b0ada912c11cbd6bf77d2eb162cfb1a6577
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7dbad85a08f79ca7ef7c449feb1dfbd6973498a21db9a0721af19e181fc39f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:45:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 01:45:36 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 01:45:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 01:45:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 01:45:53 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 01:45:53 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 01:45:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:45:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130a79b60aae9998377169e6355792370bb064e6148684353d6ed4826039492f`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43519aa40fdf82f3b05cab9731634890c7e8dc8b9731ce4c7c3fbbc35def0274`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 7.3 KB (7299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1b5762b7444935215ce9e31bc9a68cac110a8b0bf2f9ca433a2d78620fe35`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 204.6 KB (204622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156837dee9efeb5125ef7fc8d079ccf996015838cfe028bfb81695eb1230b99`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f221da4d2654d1b1432ad3c77afeed7392661b44c6a50fc1fd5e2cede5dfcb`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:da842be683e4aa6e7f0e6581d7d9bd1604d2d140a1b452e47a1ca595261af814
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3055327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7b5670b88fbd238447f1f65531173381d0aff05ec6d63ef2df4dfb7b8c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:35:24 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:35:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:35:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:35:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:35:45 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:35:45 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:35:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:35:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:35:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95070702ac27305ca355fc2880dec01d9e18d3c8a4a22842a599db59ea5467e0`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35be501885b2efd06479a1d05af31f0d06d6b0a5c4dfb3f760af81657d7919ea`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 7.3 KB (7287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f5e404d9d5a395b15445e0403dfa9a598ab9ecd02814798d33098ac6a8ba9c`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 223.4 KB (223445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b8287cb974321164bff4ca80e9a231471fecf0bbab1bbf130172709ae47ae`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c88353a13d0403b037e398aa01ea54701b91f2adf180d6ed9df1b155b62c89`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:3c83af52715b14ccfd27cc89b7b988ae73b9d05500efd053b99b027c0328f14d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59b6df7881927f19f4b2dcab5974d93c4284e7e9ba9c21098a82d888389b26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:36:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 27 Aug 2021 21:36:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 27 Aug 2021 21:37:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 27 Aug 2021 21:37:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 27 Aug 2021 21:37:41 GMT
VOLUME [/spiped]
# Fri, 27 Aug 2021 21:37:48 GMT
WORKDIR /spiped
# Fri, 27 Aug 2021 21:37:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:38:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f143c775bd94ef9de49da05aab2353301bc02ceb74a237332f8d9b23e193234b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9067169d42bea9851adf89b67776e5a280513855fb73120a8d2c5f0051a1097b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 7.3 KB (7292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe10232ba40d32a7b84a0fe16aa0a2b418d2bdf093335c9fbaf56b08e751c54e`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 221.2 KB (221238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c7d84f077aa3ad717767ac56d4b1ea509bc7a9c81e57e3f4e210fe09205ee9`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c90dd2a4fa5a2acd662ddc7f2ec01550257e4bbaae18ab7a94fdd288523cf8`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:3852ee4130c6bfe6eb29489ab1f82c2aceed2d65ba3a11477360199bd6ba4bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2817762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d772c7d45678813ce17e2e65d11aa3e23e0517de39acbfe03eaaadf3558b6f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 04:23:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 04:23:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 04:23:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 04:24:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 04:24:08 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 04:24:08 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 04:24:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 04:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 04:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a66831aa123cebdb722d7d1efb39f1ffb26129fdf9b8937935375852a206`  
		Last Modified: Sat, 28 Aug 2021 04:24:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b103bd0361f6fb48151c8780e205c3fde97140b66762b27effcf2c3b73c05c`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 7.3 KB (7283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce02139d2773db6b3c7033d9dbc6fdb427c918a69c29b8bb01669296d18c9fe`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 205.3 KB (205277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c3cb214e79007442b4d21bc48516c0ef35753d8db03a0cc129fa63d01bedde`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29859d07f0b507288c642deae1bae6cbe9d019152647a0c4e76bd86474fda106`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:89f362dd004a510b0e2dfdfdf849444c25d6fb0c60e3b7df331ece34ce763a31
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
$ docker pull spiped@sha256:44015ddc42ceef8878c9b2bad7a6bcbf2b5d2ca42ab52cca20f9f66b2c15ffd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65d8337530e6b8e116202287d477945c4375886702df4698f8740106658a777`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:56:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:56:13 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:56:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:56:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:56:31 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:56:31 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:56:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:56:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:56:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72fe484884c949a7fba8b7d917cbe40b9fa50036f4c10e4b82e3075576fe3fc`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06083e8d35a44724cf84de43d971fb5b141e8ce6468a5c267c43c96f79869f23`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037fda176acae1eef93fa1dde784253576faf4d880c75c8d7df76fdf212dda`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 212.5 KB (212547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb3cd7f024c8cfa70e1c8e8f282e44395bbaa20cd69851af0552d8041deaea2`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fccea2af66d4ffdbdd93edf485c1e6e17f14ac10329842af6fea7741bd3504`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:7e548b9910cf9bcbce660ff537e09660dbd9d84cbc06621e45fb2282f2f52270
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2838978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8539d235dbd2d180f98df622ec1586ed595c7026c53f57b67876cbe0b641be9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:39:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:39:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:39:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:39:57 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:39:58 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:39:58 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:39:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:39:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:40:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ec865614b924d3ebd8faaf1468ff031de3ccb2f178656d907e4a89f8673776`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07908dc20812a0124cb96563b08ff2d4ebd32f0ca0cef02511faa0c127496e96`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 7.3 KB (7290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2ce7f8303145adfe2a17235c758d30fa18338c417eb73738b591c1dd3d1315`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 202.5 KB (202499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07f8ab6ed47190923d1d152d960c5fd80b7d9f27f84a289e8236a1e4f22843c`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17d0a64e682741c70413fc90f0d8a4dac61425dcc5c98ce054909120977e587`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:24d05f05df7127b2aa61654a9d29c77a0c2a00f8ba29dbfc127a672700d5f652
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2635217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c197156cacbfdbdb870ce3391ad1bdf7d6c922d18648489e7549033356f432b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 03:04:23 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 03:04:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 03:04:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 03:04:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 03:04:59 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 03:05:00 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 03:05:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 03:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 03:05:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c187e6961a8f3ae8bf645e1fbec375c4f7c3d8146ab5ee5a09f57cd5615f33cb`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56c389f9017243d26a8fd61b3cc3385e2b4dcf930d608cc682a5ff3b437137`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0da469457d5465481ffd06dc86cd457daaf02e8b501cbee7b9cb52b675525`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 195.8 KB (195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea4333c9f229866ca36ab2d7e036e1d23031e78c62c3ad0bcbbeacaaf8f8e65`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4907440a689992d3e1fbcc2fcef650c5ef7b7abe5b8b3aa9c97d6d697d5050fd`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:026d11edbbedc8b8a63207a745859b0ada912c11cbd6bf77d2eb162cfb1a6577
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7dbad85a08f79ca7ef7c449feb1dfbd6973498a21db9a0721af19e181fc39f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:45:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 01:45:36 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 01:45:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 01:45:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 01:45:53 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 01:45:53 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 01:45:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:45:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130a79b60aae9998377169e6355792370bb064e6148684353d6ed4826039492f`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43519aa40fdf82f3b05cab9731634890c7e8dc8b9731ce4c7c3fbbc35def0274`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 7.3 KB (7299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1b5762b7444935215ce9e31bc9a68cac110a8b0bf2f9ca433a2d78620fe35`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 204.6 KB (204622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156837dee9efeb5125ef7fc8d079ccf996015838cfe028bfb81695eb1230b99`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f221da4d2654d1b1432ad3c77afeed7392661b44c6a50fc1fd5e2cede5dfcb`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:da842be683e4aa6e7f0e6581d7d9bd1604d2d140a1b452e47a1ca595261af814
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3055327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7b5670b88fbd238447f1f65531173381d0aff05ec6d63ef2df4dfb7b8c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:35:24 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:35:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:35:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:35:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:35:45 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:35:45 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:35:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:35:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:35:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95070702ac27305ca355fc2880dec01d9e18d3c8a4a22842a599db59ea5467e0`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35be501885b2efd06479a1d05af31f0d06d6b0a5c4dfb3f760af81657d7919ea`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 7.3 KB (7287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f5e404d9d5a395b15445e0403dfa9a598ab9ecd02814798d33098ac6a8ba9c`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 223.4 KB (223445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b8287cb974321164bff4ca80e9a231471fecf0bbab1bbf130172709ae47ae`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c88353a13d0403b037e398aa01ea54701b91f2adf180d6ed9df1b155b62c89`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:3c83af52715b14ccfd27cc89b7b988ae73b9d05500efd053b99b027c0328f14d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59b6df7881927f19f4b2dcab5974d93c4284e7e9ba9c21098a82d888389b26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:36:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 27 Aug 2021 21:36:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 27 Aug 2021 21:37:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 27 Aug 2021 21:37:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 27 Aug 2021 21:37:41 GMT
VOLUME [/spiped]
# Fri, 27 Aug 2021 21:37:48 GMT
WORKDIR /spiped
# Fri, 27 Aug 2021 21:37:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:38:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f143c775bd94ef9de49da05aab2353301bc02ceb74a237332f8d9b23e193234b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9067169d42bea9851adf89b67776e5a280513855fb73120a8d2c5f0051a1097b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 7.3 KB (7292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe10232ba40d32a7b84a0fe16aa0a2b418d2bdf093335c9fbaf56b08e751c54e`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 221.2 KB (221238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c7d84f077aa3ad717767ac56d4b1ea509bc7a9c81e57e3f4e210fe09205ee9`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c90dd2a4fa5a2acd662ddc7f2ec01550257e4bbaae18ab7a94fdd288523cf8`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:3852ee4130c6bfe6eb29489ab1f82c2aceed2d65ba3a11477360199bd6ba4bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2817762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d772c7d45678813ce17e2e65d11aa3e23e0517de39acbfe03eaaadf3558b6f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 04:23:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 04:23:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 04:23:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 04:24:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 04:24:08 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 04:24:08 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 04:24:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 04:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 04:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a66831aa123cebdb722d7d1efb39f1ffb26129fdf9b8937935375852a206`  
		Last Modified: Sat, 28 Aug 2021 04:24:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b103bd0361f6fb48151c8780e205c3fde97140b66762b27effcf2c3b73c05c`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 7.3 KB (7283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce02139d2773db6b3c7033d9dbc6fdb427c918a69c29b8bb01669296d18c9fe`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 205.3 KB (205277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c3cb214e79007442b4d21bc48516c0ef35753d8db03a0cc129fa63d01bedde`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29859d07f0b507288c642deae1bae6cbe9d019152647a0c4e76bd86474fda106`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:6211c62aba90f5a091c3e8bf9fd958676ac9d75e01ba5b38d95df35bac823f5c
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
$ docker pull spiped@sha256:d779db31393bf73bb7a45ab8a3e8f547216d6a0abbaa630fe44332adefc6f054
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37324937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306415ec98a85eb9753b91a8c6c8d4f25c43dd898da213370452cde68fd6125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:40 GMT
ADD file:5e8343ab9a73edc27c2889634896e792ab289b85c206de0fc31183fdc0a32ac7 in / 
# Tue, 17 Aug 2021 01:23:41 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:05:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 15:05:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:05:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 15:06:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 15:06:25 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 15:06:25 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 15:06:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 15:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 15:06:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:99046ad9247f8a1cbd1048d9099d026191ad9cda63c08aadeb704b7000a51717`  
		Last Modified: Tue, 17 Aug 2021 01:29:35 GMT  
		Size: 31.4 MB (31361314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc464d0b8e823e26756d296bc514c2d5b282b5ab89630b586934ee6cb2a037ff`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d965e596cfe4edd8ac0758b349deab04685e0808f972fed94586afdb1adb57`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfffba101beb13e886e681ef1388d2f2df4a89c8ac5c6b7f35ec01506bd2f1c`  
		Last Modified: Tue, 17 Aug 2021 15:06:54 GMT  
		Size: 6.0 MB (5960364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903fa4411c463574fad05212e81bea73cf8f1310ced1b8b733d706a371e89e74`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13bd7a2594aff90e0447dbe191de68e7a9f0074848194a7833d0819a330dd4f`  
		Last Modified: Tue, 17 Aug 2021 15:06:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d2b531d8f0a42f8007d557790380594037ed5a3187dcda60468ba6f7b205a3f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33932544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25830ba5d141ad6cd8b98286a5cd9a1815be8f4783bec5b75a895cd325b7756`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:48 GMT
ADD file:9ab41fbe9b84c147eb71d451b4d31f27a0eb362bb6d14ee3ba6279d67ae25531 in / 
# Tue, 17 Aug 2021 01:55:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 17:44:38 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 17:44:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 17:44:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 17:45:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 17:45:50 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 17:45:50 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 17:45:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 17:45:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 17:45:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91b48139ec3e0280b0a9be84b502b3d6394149000106be38ac11a1c31b59d956`  
		Last Modified: Tue, 17 Aug 2021 02:11:08 GMT  
		Size: 28.9 MB (28904169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529af9182deb82a91ca1183e2f07ecae36ac80f65deb9aff5fc00aefe37b6cc9`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ff236190840487b8990652b37a3a02c6e5d5b21abc3955ab978f2431daea0b`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736ab94697c6fe32a81e259b0b22e03fa3ac4a224f1cf6be8647408d9c5dc2c4`  
		Last Modified: Tue, 17 Aug 2021 17:46:32 GMT  
		Size: 5.0 MB (5025125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521e8718ebe2c738541e1e87062916db439105c9e6bb71a5620be53f30384b46`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da9926511e4c596a58c07504e57c175041264b8361b4a900adb663d63fbbc8`  
		Last Modified: Tue, 17 Aug 2021 17:46:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:82c3c2ebe3bd31cb51b8698b02fed6c6c8ddababab59c49902dbfb838fde261a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31314263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a771171769e644813614e8ec5270e93b93c509715bd5b1d357f8536dbe89c16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:16 GMT
ADD file:56b22dfd365932a88a68ec72e6b9c1af8c5747606e0387a2c189dfb49998d029 in / 
# Tue, 17 Aug 2021 02:13:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 21:12:26 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 21:12:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 21:12:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 21:13:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 21:13:41 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 21:13:41 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 21:13:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 21:13:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 21:13:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:118503c5404bba02cc6a70fd0b808c846fefe8a3435d831a37127a6fdc8f96a2`  
		Last Modified: Tue, 17 Aug 2021 02:29:31 GMT  
		Size: 26.6 MB (26565574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c45a3e608c37966ffad43edbc665486402dd651491b7a21297039852eafb658`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c41d652aa1399132c065b29940395b49fe97738bf2020b48ecb6861757d884`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0c590b6187a7f7de3a81cb5f71d2bece146d195f838c9c5e7134c614f60675`  
		Last Modified: Tue, 17 Aug 2021 21:14:58 GMT  
		Size: 4.7 MB (4745433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a95b0f4e791c265d50fe017d3ecfa55e9266c4d89fbf2c7761a16c78ba77a`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a04c9a6b135c00d4d849bb7249448c25c40eb54fa8dea1e0237ac82791eb2d`  
		Last Modified: Tue, 17 Aug 2021 21:14:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:a8cb1de1b7ac27edc9001452b532e01129969840f12809227cb60400cc4e39a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35316841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac4558f48bddf4104b4828089d6aa2d9e1b3b223116b94d9e70f8d17bcd91fa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:04 GMT
ADD file:0a42d4a201f0ac7889187c3212fbdfc2747f31f36e690d59c22eec50fe542614 in / 
# Tue, 17 Aug 2021 01:46:05 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:05:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 12:05:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:05:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 12:06:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 12:06:07 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 12:06:07 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 12:06:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 12:06:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 12:06:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3716b9f3c2f9e7592f5b47c2e6e13e64132071620c7551e0aa3c5c248e106139`  
		Last Modified: Tue, 17 Aug 2021 01:53:29 GMT  
		Size: 30.0 MB (30048801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d1e840bed4d3d0ccdf6507f2f244340722bfccf593ec463750eae2b86ea83d`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f75e45873615f57906ab6bd8be8065a16bfc73e217ef9b96e7ff0170ea02e43`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e964d1a9f206f9e8026c7b4c594b686d9ec49d8d9ed8e8cbda8d1437bd77ff4`  
		Last Modified: Tue, 17 Aug 2021 12:06:40 GMT  
		Size: 5.3 MB (5264787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce44b119695cd419968d21d74d37482f3bbe86cca3432a4f284309bac2d55ba`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31893ecc983ab9a027f5aae03453a9bd6611eed642bd73ac2b9d14a4b292ba90`  
		Last Modified: Tue, 17 Aug 2021 12:06:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:51db9ecb4b19727e637474ec3edcbee6a3f8b10cf9849e1bb18e4de26e9d1cf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40262874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aea617771607db5094f062cd1b36f273130f573f444293d5b8bf8f6ca4ba586e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:28 GMT
ADD file:9afc107c0880864c9f16852bb6cc272a068f2c82a2df7c3444bbbc533f377156 in / 
# Tue, 17 Aug 2021 01:40:29 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 17:17:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 17:18:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 17:18:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 17:18:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 17:18:34 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 17:18:34 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 17:18:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 17:18:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 17:18:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6edd81381c438b83d2749dc056d46cd53320e27fb010b3e931ca1f0a752ddc07`  
		Last Modified: Tue, 17 Aug 2021 01:49:56 GMT  
		Size: 32.4 MB (32375657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f073609c1b59b4b496ff4cd4329461daeba813c650c1439397561fa937e53c`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9070386f59e19b077a8c2157fb94a95e2366a8845ed5505eb3fe31214209fae`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceead4902ad3c822b58360ac4f18d6861f2d214f601abc65685d657b693e810`  
		Last Modified: Tue, 17 Aug 2021 17:19:15 GMT  
		Size: 7.9 MB (7883966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16e38803b194f569d38caf69675f72659a74604c89befeafb476b657afe3146`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6da0e93b70ab4a38a695f1a65d884a2c6fdfe7ea92f45d91e2a962e3c89b141`  
		Last Modified: Tue, 17 Aug 2021 17:19:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:d945e41b8d4bd950e1be63af3f3229ac00be11b318b361a3beffc50e7ef0eaac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2581ff16e0a3ffb4037d0c23b704ece31bb583ffa283a4f1bb062d42ba3def7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:01 GMT
ADD file:e842559443fb9351f1a9ac9ce03dfe0b069d8b9c3409f8d9b21abcbdc2a437c5 in / 
# Fri, 03 Sep 2021 01:10:02 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:42:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 03 Sep 2021 01:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:42:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 03 Sep 2021 01:43:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 03 Sep 2021 01:43:33 GMT
VOLUME [/spiped]
# Fri, 03 Sep 2021 01:43:33 GMT
WORKDIR /spiped
# Fri, 03 Sep 2021 01:43:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 03 Sep 2021 01:43:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 01:43:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2320664dc3760d5d905a15eef2bf52da0cbab097fb4fc626c1f96722a2e2188c`  
		Last Modified: Fri, 03 Sep 2021 01:18:25 GMT  
		Size: 29.6 MB (29627416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18f077ba2ec335663d52307f6bfd922f985212d8fa94ecb63cb11050a8f3314`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d948a422c2276c40a4832dee38f347f364a0a1c2b3f5d0c1df29141d7fb1492`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46b33b2146e543c4306686645f91f5627385bf944b5ea340c691c7aa580f37c`  
		Last Modified: Fri, 03 Sep 2021 01:44:00 GMT  
		Size: 5.7 MB (5706047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808267f420422a78f98748362d203d41a9e7033571d62e15511faac06294aebc`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcfb83ee5525340e79d5b08f1809304f00d86ed6570a024a41fa23424e3760b`  
		Last Modified: Fri, 03 Sep 2021 01:43:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:eb4b77221b29aca3170128d240159baca14887a971ae076251bba0b9cc49f493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41268765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df33ed783b716cb0f12e35a85b119a6dfb68665722c2cb9b7fbcf3c98404f6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:09 GMT
ADD file:b7348f0e1a41ce54354496488a0ee8bb949743444973dc6ab51ea80926f596f2 in / 
# Tue, 17 Aug 2021 01:33:15 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 16:29:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 16:29:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 16:29:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 16:32:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 16:32:20 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 16:32:26 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 16:32:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 16:32:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 16:32:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:80e30391b3a42f13bd8cb2b497506fa7a23b074d43f7446d94b06514e408020b`  
		Last Modified: Tue, 17 Aug 2021 01:46:01 GMT  
		Size: 35.3 MB (35264011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60929bf2df877410036f8525da51c93fc047d640fe7d71540bce092c2dbc3c3f`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a700ec7060ef93bf348dbb18aebd9b1065b822685cbf1f5d70efe88648fb7d4a`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d945be8f4c7314b6ac7aee0b27681d8890d66197b5376c96b23aa2534911589a`  
		Last Modified: Tue, 17 Aug 2021 16:33:20 GMT  
		Size: 6.0 MB (6001477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7914ec06b96350b2868d9788e0d8df35e4fdbed1ec14e573025bfeaaa37ec4d`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ceb8036a7f8603020bdab26c0cc2d6f074327d9295ecb58d17441ab98f960b`  
		Last Modified: Tue, 17 Aug 2021 16:33:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:ef96b17d2a788c7bfb1d3838d6545d7f2c5b43cc8141107856c7cbd37eea1853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34834136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a087283bae8568adc0cf7b07e5eb5f24718cbafcdd6545ac0fb12315ccdd99e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:02 GMT
ADD file:9a849f976712983c3bf95c9d110ab1c38643273c19644a436242e8b8bd5eb225 in / 
# Tue, 17 Aug 2021 01:49:07 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:53:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 09:53:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:53:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 09:54:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 09:54:27 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 09:54:27 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 09:54:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 09:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:54:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:16c136b299a1426955abff4eb0ed556e3c2e8e67509fba84e416f1d5cc77189a`  
		Last Modified: Tue, 17 Aug 2021 01:57:33 GMT  
		Size: 29.6 MB (29647028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101ad9278b6e0a43e087711eaabf1f30721c9e7522020a583d5a3da6e16f3b4b`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3812b210386b50d3cb22925b3646ab61d16da033fd61ecbe3768c4e3e716d0`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436874c5caaa558dc75edb5e309ac884c077ca1b6c376902ad4e2d6b7b2157f9`  
		Last Modified: Tue, 17 Aug 2021 09:55:16 GMT  
		Size: 5.2 MB (5183847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea485d629322bebbea0f2d218fd81ce6928baba229a9097169b5cf111713ae36`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50377e04053d99e09a6cb5a363b98fc242cf892438537e805afda7c2fe7bfad`  
		Last Modified: Tue, 17 Aug 2021 09:55:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
