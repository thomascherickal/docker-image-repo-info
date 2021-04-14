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
$ docker pull spiped@sha256:bcfa5bf2019800c382c0cbf4a4065072f39596853c9b7d9778cc99380acab717
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
$ docker pull spiped@sha256:f4c8cf8326ab33cd354305073c6727b214ccf6cf9bef112e114175698f980133
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36307336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970bd62433d7ba5b68a9bb30b8743f67661c16720b39f2d79f7835749494ddf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:49:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:49:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:49:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:49:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:49:52 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:49:52 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:49:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:49:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc92f6e0387f6c4c81c2db56fc225414cd2001b6625d18d790d21dae456c7a1`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b959b67822e3f7f5b8064225f9944a56182fd013d00c6ade8afb0b38b759737`  
		Last Modified: Sat, 10 Apr 2021 17:50:17 GMT  
		Size: 2.1 MB (2128494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6395a811d45b3e5c7e9495bd87f829877641cee3b801738b305629b4d90eec35`  
		Last Modified: Sat, 10 Apr 2021 17:50:18 GMT  
		Size: 7.0 MB (7037265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af2a6a8a368f01436cdb331c2181e1d11269a377847ca2416cc230e4026046c`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1830f4c5ff2f6d2ffd051894e7a67c920d4a48b770d71df0121b5a1d7a0a83`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3fd3d9fe1ebe8666d1c6f0657f5b0a3a24c71080b95d47d62bc1d43e0bac0f3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e664e805e875edc3ba60ef0d3083f4976c237e52e46ba7ef2cd2ff5510602e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:44:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 02:44:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:44:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 02:45:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 02:45:35 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 02:45:37 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 02:45:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:45:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:45:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359ea1c1cd30128438a45a1351fdf7520a079b564420fd7f5024679aad200a53`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e0f01d18d0761741095f14750960d0d576b42baebe6013011380d3bb65d09b`  
		Last Modified: Sat, 10 Apr 2021 02:46:02 GMT  
		Size: 1.8 MB (1839353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160f3b53711a6503a1ec5a5a4813e0ca96f0837334505440e751e227d54a35fb`  
		Last Modified: Sat, 10 Apr 2021 02:46:03 GMT  
		Size: 5.5 MB (5479993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b643ff2b070f178da76cece1c6f44b280ada992902ffb22fa8d54fe781572c`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7c4ed994d4c79b38848795499cd002dc04f33e1af5e01c8ada4b5a48c66d71`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7c5a0bcce25a79c4644d397b7c4f3eeec9150f1e2551bb0acbdf6a2e28a2dc4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29787170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d9af145384c8ca2f2ae087bb8e1a5df1f699e52ff77d3ec778b12e951cedcac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:31:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:31:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:31:39 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:32:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:32:40 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:32:42 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:32:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e132f19a81693e3bea90aa7698101a380355517cf5674c8fefeae9a9b8f7397`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad66c9fc06e8f30eecb06003f9ca959dc1ed0d6bf45745e7bc7c184022ce42c`  
		Last Modified: Sat, 10 Apr 2021 17:33:21 GMT  
		Size: 1.8 MB (1759534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ce9886a1331c50e59b6865795323227794c12864a587dc8eb0985f61d6b2f8`  
		Last Modified: Sat, 10 Apr 2021 17:33:22 GMT  
		Size: 5.3 MB (5285631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623f7b9649bf9380af66dc8ccb7f9c28e41ab6cb736beaf94d7a6cdccfcf203a`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53caf6b80c2b4c1cb40842c3e50fccda582c7f2683d9d05b2e85928ec394c26`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:128d164bf24118ad5dd088f35504da3e7a06b78623fe6fa86ab78c84e6613bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33820136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2e925e557bb74d5da4d7120a6d98d40c7709b9ad5ad552f680b1ed99add6c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:01:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:01:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:01:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:03:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:03:07 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:03:08 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:03:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:03:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:03:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb133991841562847fa4d3d49051504808ca6dc6d155c988c74174cc23aa8b1c`  
		Last Modified: Sat, 10 Apr 2021 17:03:48 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4f81294ae29faf2a887908f5f0b834cbab6b5ae1cfdc8ad50f05e4d1457074`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 2.0 MB (2007922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306238b4b7fd01248f39833d7516c2a20b55fe761978bb7837e761e656bf6de2`  
		Last Modified: Sat, 10 Apr 2021 17:03:51 GMT  
		Size: 5.9 MB (5905424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f461f7ab65cbf0f96aafa4085b1bd84c6440e915f211db3328213de369d025b2`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00e526777a5016361a4ce1f4806c3a1d89fc9d7842a42ac54920784199d582c`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:d68d2d1b3c8f0ce60e342d625cf571f21aad1f2483d7db7148f1523683f3806a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f8a8936063233911434c8b1b73f2357a72cf4196b28980dcdda748efab1d532`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:16:40 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 15:16:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:16:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 15:17:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 15:17:38 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 15:17:38 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 15:17:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 15:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 15:17:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf398c419aabc68fea7850512dc92ba9a997988e025b6289e28ef3e7504ecde5`  
		Last Modified: Sat, 10 Apr 2021 15:18:16 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00a66335b36c958bff2af5d678b5fcb5c4a0116ac1f00ce3299989a9bcf96aa`  
		Last Modified: Sat, 10 Apr 2021 15:18:17 GMT  
		Size: 2.1 MB (2132686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10244eec576c73e81995793042494e8aeeaf0bc9774e606f54895db315ebcab4`  
		Last Modified: Sat, 10 Apr 2021 15:18:19 GMT  
		Size: 11.6 MB (11633276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6239beecbaf5951fb859637f32aa441c93ae2da19f535d9bd1a07364858f3b86`  
		Last Modified: Sat, 10 Apr 2021 15:18:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4d38a98dd755097789b911ed3e863da82357c9e4289805183eb96a8fbc014b`  
		Last Modified: Sat, 10 Apr 2021 15:18:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:88e595c4b27fc66524e48dc1d678f2cbba6aa124dd3c65a2f792f8317663f051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e3676406df78b6cd8501e021dc7584709e54e21d7aef150112df4116385b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:37:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 01:37:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:37:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 01:38:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 01:38:40 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 01:38:41 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 01:38:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:38:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e19b3a2a37a3ecbe5a0aef01b1271a3b63c4217adaa2cc9f1292b79afe4d54`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bdb8d46506c398b7a733af7dd918073564e2c1b5610e6077653e5a22d1a8bd`  
		Last Modified: Sat, 10 Apr 2021 01:39:05 GMT  
		Size: 1.7 MB (1712464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926e043611bbb0d92306441137302078e787a32420244e12aabb683e29d80455`  
		Last Modified: Sat, 10 Apr 2021 01:39:10 GMT  
		Size: 6.4 MB (6416465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b4bc1074f6d5e2ced135b61984cf1cf7f9bfd48fcd344e8e0aeb5bd85b125`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4518d534fd104cc99e25d1836fdb49c93d46fc837842791310d48c227d8bfda`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:a3a251b6a97959f701bf1acadc1693e943a07296b74ec6dece59b2ef5cf4aa1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39516694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977153520d8e2433a81145401c5bfaf8331fda3ed931697d5e69a5379ca096db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:08:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 03:08:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:08:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 03:10:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 03:11:00 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 03:11:05 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 03:11:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:11:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b71c6130da437d81e36b2e46715409bb7901ec1566c003390407ffc949ff6eb`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e911068150f8e65c421043fc8668c6a483fa893cbbcb63368c5f47e9dce340e5`  
		Last Modified: Sat, 10 Apr 2021 03:11:47 GMT  
		Size: 2.2 MB (2225127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7bda3e4e0b21582c4b5f98c62bbc39d07aa968bb8d0fe06b5ce3f27ead068`  
		Last Modified: Sat, 10 Apr 2021 03:11:52 GMT  
		Size: 6.7 MB (6743424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3101cf66058d718948c9600d857eb0d7e528d8476278509a227497a2f11c699`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634602e4c957f473aee73645518527fd9bdd678fb7537843b8622645d5e9ad24`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:aa1a30de2b923e99b6d6ea55762ce4a9d15c0eef4651c9a4712e9e2ecad39e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff980a5b5e94897b7af54b9c04e2610d83a31e1dc070fb483f806ee4396b8dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:23:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 02:23:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:23:46 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 02:24:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 02:24:02 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 02:24:02 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 02:24:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:24:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:24:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd6c712f3969791adfeec2f43170db16367eaef66a82536b0552e4b68a5f642`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b29032a4acd3ff5105640e38c4a45b05a57dcee751656350ca162fa404dd33`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 1.8 MB (1821986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd0c44243082c25de145fdf20d06ce41b41a86768dc7b3d2b3bb73c416e488b`  
		Last Modified: Sat, 10 Apr 2021 02:24:23 GMT  
		Size: 5.9 MB (5943443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179bb3d59a006f4ddc951a6cadea2d81f4262873eea7f2167d04a821ccb67acc`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dea98f9a5ff0fd3b0d022a829368fcc98453f3884e762bace5d032dbe7d093`  
		Last Modified: Sat, 10 Apr 2021 02:24:23 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:aefae8d25636a458e185a9bdf732f777ad466c60cedc0d9660e80d008d507bae
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
$ docker pull spiped@sha256:11ac8213b02d297409d7b7fcdd8b0a48a5be943ccb0afd600aca0acba5baf06f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c25b1de2b0d5ff0e8efabf3d3cc3abcc606adf1766270b1b437a961cc0b775`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:28:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 17:28:12 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 17:28:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 17:28:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 17:28:29 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 17:28:29 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 17:28:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 17:28:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:28:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86881cb39d8440a13e92432f2eebf9be90157813318580e5dfcfd3470cae225`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d85f5395d4deda0716a51b14ea11cabff7f6a33b0c4a4ff807e9d3e6e9b0a`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 7.0 KB (7043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f474ecd48230c6ff5ddc935a076e4f4fe4dc842cd8bc8113839f2b35227a75b5`  
		Last Modified: Thu, 01 Apr 2021 17:28:51 GMT  
		Size: 212.3 KB (212303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1525e8140e52c856b6afb278a1a36428f04cd948fd81c1361fc5575a8bcd998`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db43661c359dd89741c1ddd2a67f9902ceb333ea378289323d319e3df1b370b`  
		Last Modified: Thu, 01 Apr 2021 17:28:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a8f094524aa54d65da82ac3129b78c13a1ff5cff473d26e7953a81a96c202ab5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6d756d9322008040c5902e261b8428a4eeadbaf973e8d48fa6a7d393a33176`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:50:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 03:51:01 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 03:51:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 03:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 03:51:35 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 03:51:36 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 03:51:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08375284756efffda8b0f8680579238d367b99e6e9774c5bc2948a223609b9`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9fba38f067baa6197b369a281149dd510a1a81b8a3271a50be709bca735db`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c433c405968ee69b45b2f652261c102453e750588274755fc5de0131b9918`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 202.3 KB (202276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6fc7889befc7a0ff491331bbd30d5efd63004b5ea0da1e12bb1b849fc697b8`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1e0e8f7257294af246022ecb31dac77d4340b0787771e6d6b552b99d97616`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:076dc896656b1b4cf2ded048821367d8960a5bdb96ddb4134bbdd3187442c04b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:782d764e7be26a956af06a4286ae1b384c9c368084344c3e2900945d2f76f4d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:09:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 13:09:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 13:09:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 13:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 13:10:24 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 13:10:25 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 13:10:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 13:10:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:10:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbca5e1d36141c0703b9cfbdde21f7aceb9796887027dcd1d7a2e934b1fc721`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fc7f276e5dab20703a18829c9730a7077537acc4f6b5216feb60a48d1cb7af`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83608b5141dc6e57fd5e8a524faa93d2bdd7816d6370cdb30f2b3e66fd48312`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 195.5 KB (195543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aea0254b4506405454f45907a949681726a965e3c091150209d6b37536036`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6556f29ebddbc9769ac742e20aa5fb223a3573b7f648aa3e248a4a71f3d7f251`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:a18a91f86b35437e8de014ede30b49f8afe472d01a834ef109b1d83125b17f10
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b51f1caddfbebc660deb95c3ba908c2d59ea1915fe919d84af4688775bced6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:02:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 17:02:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 17:02:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 17:03:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 17:03:33 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 17:03:34 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 17:03:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 17:03:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:03:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdada7d83e7e80aaec853072a1598b0c0fc5272fc127acd150cc8dd6adadbdae`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88e6d0a2872d085185993ef77cc2e06a04ba200b3661ab389ce0108a0e5da41`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f834d24bb46d96feb30e4bf9137b76b2bec1a1678b72705fe99d890bd366c042`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 204.4 KB (204435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4d996ecb3b43082fd444b4ce2ff7632038162bb56e65886c1c16bf7cafd554`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3552f514ab3c2e5888b630036603538eef1cd5a75728c8e35af64dcd84115`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:654e6d7a720dfa4eb8a1d72df30b8f1e3122cba0850349dbcf246f63b93d4606
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d405b48065d7865937665d693ec98c89b327b2a5a2922eda935887d7f7d7dd0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:51:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 07:51:35 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 07:51:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 07:51:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 07:51:55 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 07:51:56 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 07:51:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:51:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d549e288a1942f308e98bd63e9a88e4b46c1fd3bf5b46f2af22e3dfde82b0bc`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aa5f33d7d1cc9f41cce3689eb319aaecec97ed85da04c9220d700f146c9e81`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e0f606528c3ab5b91505c21f3557ad732bc6d02d418edf4f63403cbe99a82`  
		Last Modified: Thu, 01 Apr 2021 07:52:32 GMT  
		Size: 223.3 KB (223283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c744159f7958c465d7ed11c8ffb2650a8a91e820729271b6c36beba8d56afae`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef80b8c05f87168506c2964fb0229d9fc6efd4fc2cc912e4b5abff7ee0a01f`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:94267d6b497d02f0f85f471c82b5b6bd0d149e12aaf359edacbbf01c941ea032
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436f12a351ea0c0ebd29c513beeb1e7e954fd1bffb8fc9aaeec88ab529a2bbca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:46:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 31 Mar 2021 19:47:04 GMT
RUN apk add --no-cache libssl1.1
# Wed, 31 Mar 2021 19:47:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:47:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 31 Mar 2021 19:47:41 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:47:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:47:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:47:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d452bef84dc63670e365215d08665984515db53171a73aac95e8fcb2e11ea8`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059bdf7279d42a1fcb055d84641ebef32bc778bca1c1d14239c4e8bd30476bd2`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96156d3c4691010d3da5a61f5368d99699eb901120314ef42751999506efe688`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 221.0 KB (220983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff346b44ef1d664ee7482a759efd0565ed8a4a05b594e069d232eee428364260`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84860a0e3e2e15db90c68d04ba424f8adfdeef75fc2e25b9719ecdd3fd36147d`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:bcfa5bf2019800c382c0cbf4a4065072f39596853c9b7d9778cc99380acab717
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
$ docker pull spiped@sha256:f4c8cf8326ab33cd354305073c6727b214ccf6cf9bef112e114175698f980133
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36307336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970bd62433d7ba5b68a9bb30b8743f67661c16720b39f2d79f7835749494ddf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:49:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:49:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:49:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:49:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:49:52 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:49:52 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:49:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:49:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc92f6e0387f6c4c81c2db56fc225414cd2001b6625d18d790d21dae456c7a1`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b959b67822e3f7f5b8064225f9944a56182fd013d00c6ade8afb0b38b759737`  
		Last Modified: Sat, 10 Apr 2021 17:50:17 GMT  
		Size: 2.1 MB (2128494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6395a811d45b3e5c7e9495bd87f829877641cee3b801738b305629b4d90eec35`  
		Last Modified: Sat, 10 Apr 2021 17:50:18 GMT  
		Size: 7.0 MB (7037265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af2a6a8a368f01436cdb331c2181e1d11269a377847ca2416cc230e4026046c`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1830f4c5ff2f6d2ffd051894e7a67c920d4a48b770d71df0121b5a1d7a0a83`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3fd3d9fe1ebe8666d1c6f0657f5b0a3a24c71080b95d47d62bc1d43e0bac0f3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e664e805e875edc3ba60ef0d3083f4976c237e52e46ba7ef2cd2ff5510602e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:44:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 02:44:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:44:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 02:45:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 02:45:35 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 02:45:37 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 02:45:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:45:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:45:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359ea1c1cd30128438a45a1351fdf7520a079b564420fd7f5024679aad200a53`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e0f01d18d0761741095f14750960d0d576b42baebe6013011380d3bb65d09b`  
		Last Modified: Sat, 10 Apr 2021 02:46:02 GMT  
		Size: 1.8 MB (1839353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160f3b53711a6503a1ec5a5a4813e0ca96f0837334505440e751e227d54a35fb`  
		Last Modified: Sat, 10 Apr 2021 02:46:03 GMT  
		Size: 5.5 MB (5479993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b643ff2b070f178da76cece1c6f44b280ada992902ffb22fa8d54fe781572c`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7c4ed994d4c79b38848795499cd002dc04f33e1af5e01c8ada4b5a48c66d71`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7c5a0bcce25a79c4644d397b7c4f3eeec9150f1e2551bb0acbdf6a2e28a2dc4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29787170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d9af145384c8ca2f2ae087bb8e1a5df1f699e52ff77d3ec778b12e951cedcac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:31:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:31:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:31:39 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:32:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:32:40 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:32:42 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:32:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e132f19a81693e3bea90aa7698101a380355517cf5674c8fefeae9a9b8f7397`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad66c9fc06e8f30eecb06003f9ca959dc1ed0d6bf45745e7bc7c184022ce42c`  
		Last Modified: Sat, 10 Apr 2021 17:33:21 GMT  
		Size: 1.8 MB (1759534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ce9886a1331c50e59b6865795323227794c12864a587dc8eb0985f61d6b2f8`  
		Last Modified: Sat, 10 Apr 2021 17:33:22 GMT  
		Size: 5.3 MB (5285631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623f7b9649bf9380af66dc8ccb7f9c28e41ab6cb736beaf94d7a6cdccfcf203a`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53caf6b80c2b4c1cb40842c3e50fccda582c7f2683d9d05b2e85928ec394c26`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:128d164bf24118ad5dd088f35504da3e7a06b78623fe6fa86ab78c84e6613bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33820136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2e925e557bb74d5da4d7120a6d98d40c7709b9ad5ad552f680b1ed99add6c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:01:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:01:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:01:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:03:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:03:07 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:03:08 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:03:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:03:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:03:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb133991841562847fa4d3d49051504808ca6dc6d155c988c74174cc23aa8b1c`  
		Last Modified: Sat, 10 Apr 2021 17:03:48 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4f81294ae29faf2a887908f5f0b834cbab6b5ae1cfdc8ad50f05e4d1457074`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 2.0 MB (2007922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306238b4b7fd01248f39833d7516c2a20b55fe761978bb7837e761e656bf6de2`  
		Last Modified: Sat, 10 Apr 2021 17:03:51 GMT  
		Size: 5.9 MB (5905424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f461f7ab65cbf0f96aafa4085b1bd84c6440e915f211db3328213de369d025b2`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00e526777a5016361a4ce1f4806c3a1d89fc9d7842a42ac54920784199d582c`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:d68d2d1b3c8f0ce60e342d625cf571f21aad1f2483d7db7148f1523683f3806a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f8a8936063233911434c8b1b73f2357a72cf4196b28980dcdda748efab1d532`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:16:40 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 15:16:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:16:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 15:17:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 15:17:38 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 15:17:38 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 15:17:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 15:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 15:17:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf398c419aabc68fea7850512dc92ba9a997988e025b6289e28ef3e7504ecde5`  
		Last Modified: Sat, 10 Apr 2021 15:18:16 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00a66335b36c958bff2af5d678b5fcb5c4a0116ac1f00ce3299989a9bcf96aa`  
		Last Modified: Sat, 10 Apr 2021 15:18:17 GMT  
		Size: 2.1 MB (2132686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10244eec576c73e81995793042494e8aeeaf0bc9774e606f54895db315ebcab4`  
		Last Modified: Sat, 10 Apr 2021 15:18:19 GMT  
		Size: 11.6 MB (11633276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6239beecbaf5951fb859637f32aa441c93ae2da19f535d9bd1a07364858f3b86`  
		Last Modified: Sat, 10 Apr 2021 15:18:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4d38a98dd755097789b911ed3e863da82357c9e4289805183eb96a8fbc014b`  
		Last Modified: Sat, 10 Apr 2021 15:18:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:88e595c4b27fc66524e48dc1d678f2cbba6aa124dd3c65a2f792f8317663f051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e3676406df78b6cd8501e021dc7584709e54e21d7aef150112df4116385b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:37:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 01:37:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:37:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 01:38:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 01:38:40 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 01:38:41 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 01:38:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:38:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e19b3a2a37a3ecbe5a0aef01b1271a3b63c4217adaa2cc9f1292b79afe4d54`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bdb8d46506c398b7a733af7dd918073564e2c1b5610e6077653e5a22d1a8bd`  
		Last Modified: Sat, 10 Apr 2021 01:39:05 GMT  
		Size: 1.7 MB (1712464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926e043611bbb0d92306441137302078e787a32420244e12aabb683e29d80455`  
		Last Modified: Sat, 10 Apr 2021 01:39:10 GMT  
		Size: 6.4 MB (6416465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b4bc1074f6d5e2ced135b61984cf1cf7f9bfd48fcd344e8e0aeb5bd85b125`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4518d534fd104cc99e25d1836fdb49c93d46fc837842791310d48c227d8bfda`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:a3a251b6a97959f701bf1acadc1693e943a07296b74ec6dece59b2ef5cf4aa1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39516694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977153520d8e2433a81145401c5bfaf8331fda3ed931697d5e69a5379ca096db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:08:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 03:08:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:08:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 03:10:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 03:11:00 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 03:11:05 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 03:11:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:11:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b71c6130da437d81e36b2e46715409bb7901ec1566c003390407ffc949ff6eb`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e911068150f8e65c421043fc8668c6a483fa893cbbcb63368c5f47e9dce340e5`  
		Last Modified: Sat, 10 Apr 2021 03:11:47 GMT  
		Size: 2.2 MB (2225127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7bda3e4e0b21582c4b5f98c62bbc39d07aa968bb8d0fe06b5ce3f27ead068`  
		Last Modified: Sat, 10 Apr 2021 03:11:52 GMT  
		Size: 6.7 MB (6743424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3101cf66058d718948c9600d857eb0d7e528d8476278509a227497a2f11c699`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634602e4c957f473aee73645518527fd9bdd678fb7537843b8622645d5e9ad24`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:aa1a30de2b923e99b6d6ea55762ce4a9d15c0eef4651c9a4712e9e2ecad39e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff980a5b5e94897b7af54b9c04e2610d83a31e1dc070fb483f806ee4396b8dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:23:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 02:23:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:23:46 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 02:24:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 02:24:02 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 02:24:02 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 02:24:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:24:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:24:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd6c712f3969791adfeec2f43170db16367eaef66a82536b0552e4b68a5f642`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b29032a4acd3ff5105640e38c4a45b05a57dcee751656350ca162fa404dd33`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 1.8 MB (1821986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd0c44243082c25de145fdf20d06ce41b41a86768dc7b3d2b3bb73c416e488b`  
		Last Modified: Sat, 10 Apr 2021 02:24:23 GMT  
		Size: 5.9 MB (5943443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179bb3d59a006f4ddc951a6cadea2d81f4262873eea7f2167d04a821ccb67acc`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dea98f9a5ff0fd3b0d022a829368fcc98453f3884e762bace5d032dbe7d093`  
		Last Modified: Sat, 10 Apr 2021 02:24:23 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:aefae8d25636a458e185a9bdf732f777ad466c60cedc0d9660e80d008d507bae
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
$ docker pull spiped@sha256:11ac8213b02d297409d7b7fcdd8b0a48a5be943ccb0afd600aca0acba5baf06f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c25b1de2b0d5ff0e8efabf3d3cc3abcc606adf1766270b1b437a961cc0b775`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:28:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 17:28:12 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 17:28:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 17:28:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 17:28:29 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 17:28:29 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 17:28:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 17:28:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:28:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86881cb39d8440a13e92432f2eebf9be90157813318580e5dfcfd3470cae225`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d85f5395d4deda0716a51b14ea11cabff7f6a33b0c4a4ff807e9d3e6e9b0a`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 7.0 KB (7043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f474ecd48230c6ff5ddc935a076e4f4fe4dc842cd8bc8113839f2b35227a75b5`  
		Last Modified: Thu, 01 Apr 2021 17:28:51 GMT  
		Size: 212.3 KB (212303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1525e8140e52c856b6afb278a1a36428f04cd948fd81c1361fc5575a8bcd998`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db43661c359dd89741c1ddd2a67f9902ceb333ea378289323d319e3df1b370b`  
		Last Modified: Thu, 01 Apr 2021 17:28:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a8f094524aa54d65da82ac3129b78c13a1ff5cff473d26e7953a81a96c202ab5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6d756d9322008040c5902e261b8428a4eeadbaf973e8d48fa6a7d393a33176`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:50:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 03:51:01 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 03:51:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 03:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 03:51:35 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 03:51:36 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 03:51:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08375284756efffda8b0f8680579238d367b99e6e9774c5bc2948a223609b9`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9fba38f067baa6197b369a281149dd510a1a81b8a3271a50be709bca735db`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c433c405968ee69b45b2f652261c102453e750588274755fc5de0131b9918`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 202.3 KB (202276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6fc7889befc7a0ff491331bbd30d5efd63004b5ea0da1e12bb1b849fc697b8`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1e0e8f7257294af246022ecb31dac77d4340b0787771e6d6b552b99d97616`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:076dc896656b1b4cf2ded048821367d8960a5bdb96ddb4134bbdd3187442c04b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:782d764e7be26a956af06a4286ae1b384c9c368084344c3e2900945d2f76f4d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:09:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 13:09:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 13:09:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 13:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 13:10:24 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 13:10:25 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 13:10:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 13:10:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:10:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbca5e1d36141c0703b9cfbdde21f7aceb9796887027dcd1d7a2e934b1fc721`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fc7f276e5dab20703a18829c9730a7077537acc4f6b5216feb60a48d1cb7af`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83608b5141dc6e57fd5e8a524faa93d2bdd7816d6370cdb30f2b3e66fd48312`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 195.5 KB (195543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aea0254b4506405454f45907a949681726a965e3c091150209d6b37536036`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6556f29ebddbc9769ac742e20aa5fb223a3573b7f648aa3e248a4a71f3d7f251`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:a18a91f86b35437e8de014ede30b49f8afe472d01a834ef109b1d83125b17f10
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b51f1caddfbebc660deb95c3ba908c2d59ea1915fe919d84af4688775bced6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:02:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 17:02:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 17:02:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 17:03:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 17:03:33 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 17:03:34 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 17:03:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 17:03:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:03:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdada7d83e7e80aaec853072a1598b0c0fc5272fc127acd150cc8dd6adadbdae`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88e6d0a2872d085185993ef77cc2e06a04ba200b3661ab389ce0108a0e5da41`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f834d24bb46d96feb30e4bf9137b76b2bec1a1678b72705fe99d890bd366c042`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 204.4 KB (204435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4d996ecb3b43082fd444b4ce2ff7632038162bb56e65886c1c16bf7cafd554`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3552f514ab3c2e5888b630036603538eef1cd5a75728c8e35af64dcd84115`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:654e6d7a720dfa4eb8a1d72df30b8f1e3122cba0850349dbcf246f63b93d4606
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d405b48065d7865937665d693ec98c89b327b2a5a2922eda935887d7f7d7dd0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:51:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 07:51:35 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 07:51:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 07:51:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 07:51:55 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 07:51:56 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 07:51:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:51:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d549e288a1942f308e98bd63e9a88e4b46c1fd3bf5b46f2af22e3dfde82b0bc`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aa5f33d7d1cc9f41cce3689eb319aaecec97ed85da04c9220d700f146c9e81`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e0f606528c3ab5b91505c21f3557ad732bc6d02d418edf4f63403cbe99a82`  
		Last Modified: Thu, 01 Apr 2021 07:52:32 GMT  
		Size: 223.3 KB (223283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c744159f7958c465d7ed11c8ffb2650a8a91e820729271b6c36beba8d56afae`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef80b8c05f87168506c2964fb0229d9fc6efd4fc2cc912e4b5abff7ee0a01f`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:94267d6b497d02f0f85f471c82b5b6bd0d149e12aaf359edacbbf01c941ea032
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436f12a351ea0c0ebd29c513beeb1e7e954fd1bffb8fc9aaeec88ab529a2bbca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:46:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 31 Mar 2021 19:47:04 GMT
RUN apk add --no-cache libssl1.1
# Wed, 31 Mar 2021 19:47:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:47:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 31 Mar 2021 19:47:41 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:47:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:47:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:47:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d452bef84dc63670e365215d08665984515db53171a73aac95e8fcb2e11ea8`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059bdf7279d42a1fcb055d84641ebef32bc778bca1c1d14239c4e8bd30476bd2`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96156d3c4691010d3da5a61f5368d99699eb901120314ef42751999506efe688`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 221.0 KB (220983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff346b44ef1d664ee7482a759efd0565ed8a4a05b594e069d232eee428364260`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84860a0e3e2e15db90c68d04ba424f8adfdeef75fc2e25b9719ecdd3fd36147d`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:bcfa5bf2019800c382c0cbf4a4065072f39596853c9b7d9778cc99380acab717
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
$ docker pull spiped@sha256:f4c8cf8326ab33cd354305073c6727b214ccf6cf9bef112e114175698f980133
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36307336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970bd62433d7ba5b68a9bb30b8743f67661c16720b39f2d79f7835749494ddf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:49:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:49:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:49:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:49:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:49:52 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:49:52 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:49:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:49:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc92f6e0387f6c4c81c2db56fc225414cd2001b6625d18d790d21dae456c7a1`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b959b67822e3f7f5b8064225f9944a56182fd013d00c6ade8afb0b38b759737`  
		Last Modified: Sat, 10 Apr 2021 17:50:17 GMT  
		Size: 2.1 MB (2128494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6395a811d45b3e5c7e9495bd87f829877641cee3b801738b305629b4d90eec35`  
		Last Modified: Sat, 10 Apr 2021 17:50:18 GMT  
		Size: 7.0 MB (7037265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af2a6a8a368f01436cdb331c2181e1d11269a377847ca2416cc230e4026046c`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1830f4c5ff2f6d2ffd051894e7a67c920d4a48b770d71df0121b5a1d7a0a83`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3fd3d9fe1ebe8666d1c6f0657f5b0a3a24c71080b95d47d62bc1d43e0bac0f3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e664e805e875edc3ba60ef0d3083f4976c237e52e46ba7ef2cd2ff5510602e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:44:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 02:44:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:44:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 02:45:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 02:45:35 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 02:45:37 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 02:45:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:45:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:45:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359ea1c1cd30128438a45a1351fdf7520a079b564420fd7f5024679aad200a53`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e0f01d18d0761741095f14750960d0d576b42baebe6013011380d3bb65d09b`  
		Last Modified: Sat, 10 Apr 2021 02:46:02 GMT  
		Size: 1.8 MB (1839353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160f3b53711a6503a1ec5a5a4813e0ca96f0837334505440e751e227d54a35fb`  
		Last Modified: Sat, 10 Apr 2021 02:46:03 GMT  
		Size: 5.5 MB (5479993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b643ff2b070f178da76cece1c6f44b280ada992902ffb22fa8d54fe781572c`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7c4ed994d4c79b38848795499cd002dc04f33e1af5e01c8ada4b5a48c66d71`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7c5a0bcce25a79c4644d397b7c4f3eeec9150f1e2551bb0acbdf6a2e28a2dc4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29787170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d9af145384c8ca2f2ae087bb8e1a5df1f699e52ff77d3ec778b12e951cedcac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:31:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:31:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:31:39 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:32:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:32:40 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:32:42 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:32:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e132f19a81693e3bea90aa7698101a380355517cf5674c8fefeae9a9b8f7397`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad66c9fc06e8f30eecb06003f9ca959dc1ed0d6bf45745e7bc7c184022ce42c`  
		Last Modified: Sat, 10 Apr 2021 17:33:21 GMT  
		Size: 1.8 MB (1759534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ce9886a1331c50e59b6865795323227794c12864a587dc8eb0985f61d6b2f8`  
		Last Modified: Sat, 10 Apr 2021 17:33:22 GMT  
		Size: 5.3 MB (5285631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623f7b9649bf9380af66dc8ccb7f9c28e41ab6cb736beaf94d7a6cdccfcf203a`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53caf6b80c2b4c1cb40842c3e50fccda582c7f2683d9d05b2e85928ec394c26`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:128d164bf24118ad5dd088f35504da3e7a06b78623fe6fa86ab78c84e6613bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33820136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2e925e557bb74d5da4d7120a6d98d40c7709b9ad5ad552f680b1ed99add6c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:01:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:01:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:01:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:03:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:03:07 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:03:08 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:03:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:03:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:03:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb133991841562847fa4d3d49051504808ca6dc6d155c988c74174cc23aa8b1c`  
		Last Modified: Sat, 10 Apr 2021 17:03:48 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4f81294ae29faf2a887908f5f0b834cbab6b5ae1cfdc8ad50f05e4d1457074`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 2.0 MB (2007922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306238b4b7fd01248f39833d7516c2a20b55fe761978bb7837e761e656bf6de2`  
		Last Modified: Sat, 10 Apr 2021 17:03:51 GMT  
		Size: 5.9 MB (5905424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f461f7ab65cbf0f96aafa4085b1bd84c6440e915f211db3328213de369d025b2`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00e526777a5016361a4ce1f4806c3a1d89fc9d7842a42ac54920784199d582c`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:d68d2d1b3c8f0ce60e342d625cf571f21aad1f2483d7db7148f1523683f3806a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f8a8936063233911434c8b1b73f2357a72cf4196b28980dcdda748efab1d532`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:16:40 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 15:16:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:16:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 15:17:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 15:17:38 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 15:17:38 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 15:17:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 15:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 15:17:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf398c419aabc68fea7850512dc92ba9a997988e025b6289e28ef3e7504ecde5`  
		Last Modified: Sat, 10 Apr 2021 15:18:16 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00a66335b36c958bff2af5d678b5fcb5c4a0116ac1f00ce3299989a9bcf96aa`  
		Last Modified: Sat, 10 Apr 2021 15:18:17 GMT  
		Size: 2.1 MB (2132686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10244eec576c73e81995793042494e8aeeaf0bc9774e606f54895db315ebcab4`  
		Last Modified: Sat, 10 Apr 2021 15:18:19 GMT  
		Size: 11.6 MB (11633276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6239beecbaf5951fb859637f32aa441c93ae2da19f535d9bd1a07364858f3b86`  
		Last Modified: Sat, 10 Apr 2021 15:18:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4d38a98dd755097789b911ed3e863da82357c9e4289805183eb96a8fbc014b`  
		Last Modified: Sat, 10 Apr 2021 15:18:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:88e595c4b27fc66524e48dc1d678f2cbba6aa124dd3c65a2f792f8317663f051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e3676406df78b6cd8501e021dc7584709e54e21d7aef150112df4116385b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:37:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 01:37:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:37:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 01:38:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 01:38:40 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 01:38:41 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 01:38:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:38:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e19b3a2a37a3ecbe5a0aef01b1271a3b63c4217adaa2cc9f1292b79afe4d54`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bdb8d46506c398b7a733af7dd918073564e2c1b5610e6077653e5a22d1a8bd`  
		Last Modified: Sat, 10 Apr 2021 01:39:05 GMT  
		Size: 1.7 MB (1712464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926e043611bbb0d92306441137302078e787a32420244e12aabb683e29d80455`  
		Last Modified: Sat, 10 Apr 2021 01:39:10 GMT  
		Size: 6.4 MB (6416465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b4bc1074f6d5e2ced135b61984cf1cf7f9bfd48fcd344e8e0aeb5bd85b125`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4518d534fd104cc99e25d1836fdb49c93d46fc837842791310d48c227d8bfda`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:a3a251b6a97959f701bf1acadc1693e943a07296b74ec6dece59b2ef5cf4aa1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39516694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977153520d8e2433a81145401c5bfaf8331fda3ed931697d5e69a5379ca096db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:08:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 03:08:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:08:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 03:10:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 03:11:00 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 03:11:05 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 03:11:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:11:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b71c6130da437d81e36b2e46715409bb7901ec1566c003390407ffc949ff6eb`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e911068150f8e65c421043fc8668c6a483fa893cbbcb63368c5f47e9dce340e5`  
		Last Modified: Sat, 10 Apr 2021 03:11:47 GMT  
		Size: 2.2 MB (2225127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7bda3e4e0b21582c4b5f98c62bbc39d07aa968bb8d0fe06b5ce3f27ead068`  
		Last Modified: Sat, 10 Apr 2021 03:11:52 GMT  
		Size: 6.7 MB (6743424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3101cf66058d718948c9600d857eb0d7e528d8476278509a227497a2f11c699`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634602e4c957f473aee73645518527fd9bdd678fb7537843b8622645d5e9ad24`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:aa1a30de2b923e99b6d6ea55762ce4a9d15c0eef4651c9a4712e9e2ecad39e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff980a5b5e94897b7af54b9c04e2610d83a31e1dc070fb483f806ee4396b8dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:23:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 02:23:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:23:46 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 02:24:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 02:24:02 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 02:24:02 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 02:24:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:24:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:24:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd6c712f3969791adfeec2f43170db16367eaef66a82536b0552e4b68a5f642`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b29032a4acd3ff5105640e38c4a45b05a57dcee751656350ca162fa404dd33`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 1.8 MB (1821986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd0c44243082c25de145fdf20d06ce41b41a86768dc7b3d2b3bb73c416e488b`  
		Last Modified: Sat, 10 Apr 2021 02:24:23 GMT  
		Size: 5.9 MB (5943443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179bb3d59a006f4ddc951a6cadea2d81f4262873eea7f2167d04a821ccb67acc`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dea98f9a5ff0fd3b0d022a829368fcc98453f3884e762bace5d032dbe7d093`  
		Last Modified: Sat, 10 Apr 2021 02:24:23 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:aefae8d25636a458e185a9bdf732f777ad466c60cedc0d9660e80d008d507bae
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
$ docker pull spiped@sha256:11ac8213b02d297409d7b7fcdd8b0a48a5be943ccb0afd600aca0acba5baf06f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c25b1de2b0d5ff0e8efabf3d3cc3abcc606adf1766270b1b437a961cc0b775`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:28:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 17:28:12 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 17:28:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 17:28:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 17:28:29 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 17:28:29 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 17:28:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 17:28:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:28:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86881cb39d8440a13e92432f2eebf9be90157813318580e5dfcfd3470cae225`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d85f5395d4deda0716a51b14ea11cabff7f6a33b0c4a4ff807e9d3e6e9b0a`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 7.0 KB (7043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f474ecd48230c6ff5ddc935a076e4f4fe4dc842cd8bc8113839f2b35227a75b5`  
		Last Modified: Thu, 01 Apr 2021 17:28:51 GMT  
		Size: 212.3 KB (212303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1525e8140e52c856b6afb278a1a36428f04cd948fd81c1361fc5575a8bcd998`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db43661c359dd89741c1ddd2a67f9902ceb333ea378289323d319e3df1b370b`  
		Last Modified: Thu, 01 Apr 2021 17:28:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a8f094524aa54d65da82ac3129b78c13a1ff5cff473d26e7953a81a96c202ab5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6d756d9322008040c5902e261b8428a4eeadbaf973e8d48fa6a7d393a33176`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:50:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 03:51:01 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 03:51:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 03:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 03:51:35 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 03:51:36 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 03:51:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08375284756efffda8b0f8680579238d367b99e6e9774c5bc2948a223609b9`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9fba38f067baa6197b369a281149dd510a1a81b8a3271a50be709bca735db`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c433c405968ee69b45b2f652261c102453e750588274755fc5de0131b9918`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 202.3 KB (202276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6fc7889befc7a0ff491331bbd30d5efd63004b5ea0da1e12bb1b849fc697b8`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1e0e8f7257294af246022ecb31dac77d4340b0787771e6d6b552b99d97616`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:076dc896656b1b4cf2ded048821367d8960a5bdb96ddb4134bbdd3187442c04b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:782d764e7be26a956af06a4286ae1b384c9c368084344c3e2900945d2f76f4d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:09:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 13:09:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 13:09:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 13:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 13:10:24 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 13:10:25 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 13:10:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 13:10:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:10:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbca5e1d36141c0703b9cfbdde21f7aceb9796887027dcd1d7a2e934b1fc721`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fc7f276e5dab20703a18829c9730a7077537acc4f6b5216feb60a48d1cb7af`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83608b5141dc6e57fd5e8a524faa93d2bdd7816d6370cdb30f2b3e66fd48312`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 195.5 KB (195543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aea0254b4506405454f45907a949681726a965e3c091150209d6b37536036`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6556f29ebddbc9769ac742e20aa5fb223a3573b7f648aa3e248a4a71f3d7f251`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:a18a91f86b35437e8de014ede30b49f8afe472d01a834ef109b1d83125b17f10
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b51f1caddfbebc660deb95c3ba908c2d59ea1915fe919d84af4688775bced6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:02:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 17:02:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 17:02:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 17:03:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 17:03:33 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 17:03:34 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 17:03:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 17:03:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:03:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdada7d83e7e80aaec853072a1598b0c0fc5272fc127acd150cc8dd6adadbdae`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88e6d0a2872d085185993ef77cc2e06a04ba200b3661ab389ce0108a0e5da41`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f834d24bb46d96feb30e4bf9137b76b2bec1a1678b72705fe99d890bd366c042`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 204.4 KB (204435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4d996ecb3b43082fd444b4ce2ff7632038162bb56e65886c1c16bf7cafd554`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3552f514ab3c2e5888b630036603538eef1cd5a75728c8e35af64dcd84115`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:654e6d7a720dfa4eb8a1d72df30b8f1e3122cba0850349dbcf246f63b93d4606
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d405b48065d7865937665d693ec98c89b327b2a5a2922eda935887d7f7d7dd0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:51:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 07:51:35 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 07:51:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 07:51:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 07:51:55 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 07:51:56 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 07:51:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:51:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d549e288a1942f308e98bd63e9a88e4b46c1fd3bf5b46f2af22e3dfde82b0bc`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aa5f33d7d1cc9f41cce3689eb319aaecec97ed85da04c9220d700f146c9e81`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e0f606528c3ab5b91505c21f3557ad732bc6d02d418edf4f63403cbe99a82`  
		Last Modified: Thu, 01 Apr 2021 07:52:32 GMT  
		Size: 223.3 KB (223283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c744159f7958c465d7ed11c8ffb2650a8a91e820729271b6c36beba8d56afae`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef80b8c05f87168506c2964fb0229d9fc6efd4fc2cc912e4b5abff7ee0a01f`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:94267d6b497d02f0f85f471c82b5b6bd0d149e12aaf359edacbbf01c941ea032
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436f12a351ea0c0ebd29c513beeb1e7e954fd1bffb8fc9aaeec88ab529a2bbca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:46:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 31 Mar 2021 19:47:04 GMT
RUN apk add --no-cache libssl1.1
# Wed, 31 Mar 2021 19:47:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:47:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 31 Mar 2021 19:47:41 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:47:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:47:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:47:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d452bef84dc63670e365215d08665984515db53171a73aac95e8fcb2e11ea8`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059bdf7279d42a1fcb055d84641ebef32bc778bca1c1d14239c4e8bd30476bd2`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96156d3c4691010d3da5a61f5368d99699eb901120314ef42751999506efe688`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 221.0 KB (220983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff346b44ef1d664ee7482a759efd0565ed8a4a05b594e069d232eee428364260`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84860a0e3e2e15db90c68d04ba424f8adfdeef75fc2e25b9719ecdd3fd36147d`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:aefae8d25636a458e185a9bdf732f777ad466c60cedc0d9660e80d008d507bae
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
$ docker pull spiped@sha256:11ac8213b02d297409d7b7fcdd8b0a48a5be943ccb0afd600aca0acba5baf06f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c25b1de2b0d5ff0e8efabf3d3cc3abcc606adf1766270b1b437a961cc0b775`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:28:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 17:28:12 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 17:28:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 17:28:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 17:28:29 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 17:28:29 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 17:28:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 17:28:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:28:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86881cb39d8440a13e92432f2eebf9be90157813318580e5dfcfd3470cae225`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d85f5395d4deda0716a51b14ea11cabff7f6a33b0c4a4ff807e9d3e6e9b0a`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 7.0 KB (7043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f474ecd48230c6ff5ddc935a076e4f4fe4dc842cd8bc8113839f2b35227a75b5`  
		Last Modified: Thu, 01 Apr 2021 17:28:51 GMT  
		Size: 212.3 KB (212303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1525e8140e52c856b6afb278a1a36428f04cd948fd81c1361fc5575a8bcd998`  
		Last Modified: Thu, 01 Apr 2021 17:28:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db43661c359dd89741c1ddd2a67f9902ceb333ea378289323d319e3df1b370b`  
		Last Modified: Thu, 01 Apr 2021 17:28:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a8f094524aa54d65da82ac3129b78c13a1ff5cff473d26e7953a81a96c202ab5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6d756d9322008040c5902e261b8428a4eeadbaf973e8d48fa6a7d393a33176`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:50:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 03:51:01 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 03:51:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 03:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 03:51:35 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 03:51:36 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 03:51:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08375284756efffda8b0f8680579238d367b99e6e9774c5bc2948a223609b9`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9fba38f067baa6197b369a281149dd510a1a81b8a3271a50be709bca735db`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c433c405968ee69b45b2f652261c102453e750588274755fc5de0131b9918`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 202.3 KB (202276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6fc7889befc7a0ff491331bbd30d5efd63004b5ea0da1e12bb1b849fc697b8`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1e0e8f7257294af246022ecb31dac77d4340b0787771e6d6b552b99d97616`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:076dc896656b1b4cf2ded048821367d8960a5bdb96ddb4134bbdd3187442c04b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:782d764e7be26a956af06a4286ae1b384c9c368084344c3e2900945d2f76f4d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:09:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 13:09:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 13:09:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 13:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 13:10:24 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 13:10:25 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 13:10:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 13:10:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:10:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbca5e1d36141c0703b9cfbdde21f7aceb9796887027dcd1d7a2e934b1fc721`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fc7f276e5dab20703a18829c9730a7077537acc4f6b5216feb60a48d1cb7af`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83608b5141dc6e57fd5e8a524faa93d2bdd7816d6370cdb30f2b3e66fd48312`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 195.5 KB (195543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aea0254b4506405454f45907a949681726a965e3c091150209d6b37536036`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6556f29ebddbc9769ac742e20aa5fb223a3573b7f648aa3e248a4a71f3d7f251`  
		Last Modified: Thu, 01 Apr 2021 13:10:46 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:a18a91f86b35437e8de014ede30b49f8afe472d01a834ef109b1d83125b17f10
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b51f1caddfbebc660deb95c3ba908c2d59ea1915fe919d84af4688775bced6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:02:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 17:02:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 17:02:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 17:03:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 17:03:33 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 17:03:34 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 17:03:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 17:03:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:03:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdada7d83e7e80aaec853072a1598b0c0fc5272fc127acd150cc8dd6adadbdae`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88e6d0a2872d085185993ef77cc2e06a04ba200b3661ab389ce0108a0e5da41`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f834d24bb46d96feb30e4bf9137b76b2bec1a1678b72705fe99d890bd366c042`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 204.4 KB (204435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4d996ecb3b43082fd444b4ce2ff7632038162bb56e65886c1c16bf7cafd554`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3552f514ab3c2e5888b630036603538eef1cd5a75728c8e35af64dcd84115`  
		Last Modified: Thu, 01 Apr 2021 17:04:05 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:654e6d7a720dfa4eb8a1d72df30b8f1e3122cba0850349dbcf246f63b93d4606
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d405b48065d7865937665d693ec98c89b327b2a5a2922eda935887d7f7d7dd0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:51:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 07:51:35 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 07:51:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 07:51:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 07:51:55 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 07:51:56 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 07:51:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:51:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d549e288a1942f308e98bd63e9a88e4b46c1fd3bf5b46f2af22e3dfde82b0bc`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aa5f33d7d1cc9f41cce3689eb319aaecec97ed85da04c9220d700f146c9e81`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e0f606528c3ab5b91505c21f3557ad732bc6d02d418edf4f63403cbe99a82`  
		Last Modified: Thu, 01 Apr 2021 07:52:32 GMT  
		Size: 223.3 KB (223283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c744159f7958c465d7ed11c8ffb2650a8a91e820729271b6c36beba8d56afae`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef80b8c05f87168506c2964fb0229d9fc6efd4fc2cc912e4b5abff7ee0a01f`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:94267d6b497d02f0f85f471c82b5b6bd0d149e12aaf359edacbbf01c941ea032
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436f12a351ea0c0ebd29c513beeb1e7e954fd1bffb8fc9aaeec88ab529a2bbca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:46:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 31 Mar 2021 19:47:04 GMT
RUN apk add --no-cache libssl1.1
# Wed, 31 Mar 2021 19:47:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:47:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 31 Mar 2021 19:47:41 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:47:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:47:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:47:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d452bef84dc63670e365215d08665984515db53171a73aac95e8fcb2e11ea8`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059bdf7279d42a1fcb055d84641ebef32bc778bca1c1d14239c4e8bd30476bd2`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96156d3c4691010d3da5a61f5368d99699eb901120314ef42751999506efe688`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 221.0 KB (220983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff346b44ef1d664ee7482a759efd0565ed8a4a05b594e069d232eee428364260`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84860a0e3e2e15db90c68d04ba424f8adfdeef75fc2e25b9719ecdd3fd36147d`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:bcfa5bf2019800c382c0cbf4a4065072f39596853c9b7d9778cc99380acab717
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
$ docker pull spiped@sha256:f4c8cf8326ab33cd354305073c6727b214ccf6cf9bef112e114175698f980133
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36307336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970bd62433d7ba5b68a9bb30b8743f67661c16720b39f2d79f7835749494ddf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:49:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:49:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:49:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:49:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:49:52 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:49:52 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:49:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:49:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc92f6e0387f6c4c81c2db56fc225414cd2001b6625d18d790d21dae456c7a1`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b959b67822e3f7f5b8064225f9944a56182fd013d00c6ade8afb0b38b759737`  
		Last Modified: Sat, 10 Apr 2021 17:50:17 GMT  
		Size: 2.1 MB (2128494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6395a811d45b3e5c7e9495bd87f829877641cee3b801738b305629b4d90eec35`  
		Last Modified: Sat, 10 Apr 2021 17:50:18 GMT  
		Size: 7.0 MB (7037265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af2a6a8a368f01436cdb331c2181e1d11269a377847ca2416cc230e4026046c`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1830f4c5ff2f6d2ffd051894e7a67c920d4a48b770d71df0121b5a1d7a0a83`  
		Last Modified: Sat, 10 Apr 2021 17:50:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:3fd3d9fe1ebe8666d1c6f0657f5b0a3a24c71080b95d47d62bc1d43e0bac0f3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e664e805e875edc3ba60ef0d3083f4976c237e52e46ba7ef2cd2ff5510602e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:44:02 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 02:44:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:44:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 02:45:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 02:45:35 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 02:45:37 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 02:45:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:45:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:45:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359ea1c1cd30128438a45a1351fdf7520a079b564420fd7f5024679aad200a53`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e0f01d18d0761741095f14750960d0d576b42baebe6013011380d3bb65d09b`  
		Last Modified: Sat, 10 Apr 2021 02:46:02 GMT  
		Size: 1.8 MB (1839353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160f3b53711a6503a1ec5a5a4813e0ca96f0837334505440e751e227d54a35fb`  
		Last Modified: Sat, 10 Apr 2021 02:46:03 GMT  
		Size: 5.5 MB (5479993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b643ff2b070f178da76cece1c6f44b280ada992902ffb22fa8d54fe781572c`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7c4ed994d4c79b38848795499cd002dc04f33e1af5e01c8ada4b5a48c66d71`  
		Last Modified: Sat, 10 Apr 2021 02:46:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7c5a0bcce25a79c4644d397b7c4f3eeec9150f1e2551bb0acbdf6a2e28a2dc4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29787170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d9af145384c8ca2f2ae087bb8e1a5df1f699e52ff77d3ec778b12e951cedcac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:31:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:31:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:31:39 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:32:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:32:40 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:32:42 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:32:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e132f19a81693e3bea90aa7698101a380355517cf5674c8fefeae9a9b8f7397`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad66c9fc06e8f30eecb06003f9ca959dc1ed0d6bf45745e7bc7c184022ce42c`  
		Last Modified: Sat, 10 Apr 2021 17:33:21 GMT  
		Size: 1.8 MB (1759534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ce9886a1331c50e59b6865795323227794c12864a587dc8eb0985f61d6b2f8`  
		Last Modified: Sat, 10 Apr 2021 17:33:22 GMT  
		Size: 5.3 MB (5285631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623f7b9649bf9380af66dc8ccb7f9c28e41ab6cb736beaf94d7a6cdccfcf203a`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53caf6b80c2b4c1cb40842c3e50fccda582c7f2683d9d05b2e85928ec394c26`  
		Last Modified: Sat, 10 Apr 2021 17:33:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:128d164bf24118ad5dd088f35504da3e7a06b78623fe6fa86ab78c84e6613bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33820136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2e925e557bb74d5da4d7120a6d98d40c7709b9ad5ad552f680b1ed99add6c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:01:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 17:01:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:01:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 17:03:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 17:03:07 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 17:03:08 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 17:03:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 17:03:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:03:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb133991841562847fa4d3d49051504808ca6dc6d155c988c74174cc23aa8b1c`  
		Last Modified: Sat, 10 Apr 2021 17:03:48 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4f81294ae29faf2a887908f5f0b834cbab6b5ae1cfdc8ad50f05e4d1457074`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 2.0 MB (2007922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306238b4b7fd01248f39833d7516c2a20b55fe761978bb7837e761e656bf6de2`  
		Last Modified: Sat, 10 Apr 2021 17:03:51 GMT  
		Size: 5.9 MB (5905424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f461f7ab65cbf0f96aafa4085b1bd84c6440e915f211db3328213de369d025b2`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00e526777a5016361a4ce1f4806c3a1d89fc9d7842a42ac54920784199d582c`  
		Last Modified: Sat, 10 Apr 2021 17:03:49 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:d68d2d1b3c8f0ce60e342d625cf571f21aad1f2483d7db7148f1523683f3806a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f8a8936063233911434c8b1b73f2357a72cf4196b28980dcdda748efab1d532`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:16:40 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 15:16:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:16:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 15:17:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 15:17:38 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 15:17:38 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 15:17:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 15:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 15:17:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf398c419aabc68fea7850512dc92ba9a997988e025b6289e28ef3e7504ecde5`  
		Last Modified: Sat, 10 Apr 2021 15:18:16 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00a66335b36c958bff2af5d678b5fcb5c4a0116ac1f00ce3299989a9bcf96aa`  
		Last Modified: Sat, 10 Apr 2021 15:18:17 GMT  
		Size: 2.1 MB (2132686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10244eec576c73e81995793042494e8aeeaf0bc9774e606f54895db315ebcab4`  
		Last Modified: Sat, 10 Apr 2021 15:18:19 GMT  
		Size: 11.6 MB (11633276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6239beecbaf5951fb859637f32aa441c93ae2da19f535d9bd1a07364858f3b86`  
		Last Modified: Sat, 10 Apr 2021 15:18:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4d38a98dd755097789b911ed3e863da82357c9e4289805183eb96a8fbc014b`  
		Last Modified: Sat, 10 Apr 2021 15:18:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:88e595c4b27fc66524e48dc1d678f2cbba6aa124dd3c65a2f792f8317663f051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e3676406df78b6cd8501e021dc7584709e54e21d7aef150112df4116385b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:37:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 01:37:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:37:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 01:38:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 01:38:40 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 01:38:41 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 01:38:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:38:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e19b3a2a37a3ecbe5a0aef01b1271a3b63c4217adaa2cc9f1292b79afe4d54`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bdb8d46506c398b7a733af7dd918073564e2c1b5610e6077653e5a22d1a8bd`  
		Last Modified: Sat, 10 Apr 2021 01:39:05 GMT  
		Size: 1.7 MB (1712464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926e043611bbb0d92306441137302078e787a32420244e12aabb683e29d80455`  
		Last Modified: Sat, 10 Apr 2021 01:39:10 GMT  
		Size: 6.4 MB (6416465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b4bc1074f6d5e2ced135b61984cf1cf7f9bfd48fcd344e8e0aeb5bd85b125`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4518d534fd104cc99e25d1836fdb49c93d46fc837842791310d48c227d8bfda`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:a3a251b6a97959f701bf1acadc1693e943a07296b74ec6dece59b2ef5cf4aa1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39516694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977153520d8e2433a81145401c5bfaf8331fda3ed931697d5e69a5379ca096db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:08:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 03:08:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:08:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 03:10:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 03:11:00 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 03:11:05 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 03:11:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:11:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b71c6130da437d81e36b2e46715409bb7901ec1566c003390407ffc949ff6eb`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e911068150f8e65c421043fc8668c6a483fa893cbbcb63368c5f47e9dce340e5`  
		Last Modified: Sat, 10 Apr 2021 03:11:47 GMT  
		Size: 2.2 MB (2225127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7bda3e4e0b21582c4b5f98c62bbc39d07aa968bb8d0fe06b5ce3f27ead068`  
		Last Modified: Sat, 10 Apr 2021 03:11:52 GMT  
		Size: 6.7 MB (6743424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3101cf66058d718948c9600d857eb0d7e528d8476278509a227497a2f11c699`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634602e4c957f473aee73645518527fd9bdd678fb7537843b8622645d5e9ad24`  
		Last Modified: Sat, 10 Apr 2021 03:11:46 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:aa1a30de2b923e99b6d6ea55762ce4a9d15c0eef4651c9a4712e9e2ecad39e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff980a5b5e94897b7af54b9c04e2610d83a31e1dc070fb483f806ee4396b8dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:23:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 02:23:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:23:46 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 02:24:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 02:24:02 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 02:24:02 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 02:24:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:24:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:24:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd6c712f3969791adfeec2f43170db16367eaef66a82536b0552e4b68a5f642`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b29032a4acd3ff5105640e38c4a45b05a57dcee751656350ca162fa404dd33`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 1.8 MB (1821986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd0c44243082c25de145fdf20d06ce41b41a86768dc7b3d2b3bb73c416e488b`  
		Last Modified: Sat, 10 Apr 2021 02:24:23 GMT  
		Size: 5.9 MB (5943443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179bb3d59a006f4ddc951a6cadea2d81f4262873eea7f2167d04a821ccb67acc`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dea98f9a5ff0fd3b0d022a829368fcc98453f3884e762bace5d032dbe7d093`  
		Last Modified: Sat, 10 Apr 2021 02:24:23 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
