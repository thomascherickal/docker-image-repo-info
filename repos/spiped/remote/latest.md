## `spiped:latest`

```console
$ docker pull spiped@sha256:bf63c6fa540d062ba2062fb8fb3ced77d23970023129895837393889e34ca92e
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
