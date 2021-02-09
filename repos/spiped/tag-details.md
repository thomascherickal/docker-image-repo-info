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
$ docker pull spiped@sha256:c8fed446657ff451ffc9455f0850478c18864fdb2a3b36791e069fedd2d1f182
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
$ docker pull spiped@sha256:813fe508ddf7ef14c654e08581a59df5889155822eb779846196b8e849333938
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36263367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67f39dd2d121caaec0db3bb313564c512f9f974333b8a772963e9a9790a21a3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:21:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 11:21:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:21:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 11:21:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 11:21:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 11:22:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 11:22:13 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 11:22:14 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 11:22:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 11:22:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 11:22:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de752b69da20dffa4f368194c801b91db7f8109eb73f00e28fcf2534595c2391`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29700ba41d506288d95fe910fe16a1412fdf652d9919afe82028b5ee5b3c04ca`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 2.1 MB (2128396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412d577285af429a0e5119c64eb42081167590075ec5fb38a4d4433890b406ba`  
		Last Modified: Tue, 09 Feb 2021 11:22:40 GMT  
		Size: 7.0 MB (7037659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc602331c59adaf25976f51dc954d66801d075f027483281c6b79bd2f12c468`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3991a274f6591f9860d4f7e3d73124d6024fd27dc097414d36cda87813ef0619`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:7f6d7dcae2bcbc63a71c78634690325aa893f07b23ebdf89d495772e2b76e9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32161112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7630b8d3c6a6778b6bf060e33944e07408a5d869c0790a7912fdb44c722221d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:43:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 11:43:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:43:33 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 11:43:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 11:43:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 11:44:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 11:44:28 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 11:44:29 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 11:44:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 11:44:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 11:44:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8e683fcc73f4da7d69ce1d5f4e1d77510aa459490068f38db2d8663698b391a0`  
		Last Modified: Tue, 09 Feb 2021 02:59:07 GMT  
		Size: 24.8 MB (24839297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346f1f77623bfcedac114c95542f4a432dbfac2903c21d7af096733db6f08d7a`  
		Last Modified: Tue, 09 Feb 2021 11:44:58 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46e79f1e8ee1ac5539cad7eefe848b44ce737e874098030fc6156b53ef573a9`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 1.8 MB (1839405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c4f4a4d55f4bff867187ec0fc856d3831a4013bc7b2439663a05c05e0bceba`  
		Last Modified: Tue, 09 Feb 2021 11:45:01 GMT  
		Size: 5.5 MB (5480212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722e4239f41acf1439f868feb56543ec05a7990de0b7e19b785a656ed9cc8245`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3795fccfaef5453c447609dbd35488bfe50615dbc8aabc29d60f5c70747a28`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3ac6871810ed67f5b21e7cd83802fdae6ecb8cc0adcf6f04aaeb1bb55469b360
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29763190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:618f6b2b1cf55feedae7e3db3ca36f7b0e57e0e8df3027fa07ea587c77c1fcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:56:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 16:56:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:56:54 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 16:56:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 16:56:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 16:57:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 16:57:52 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 16:57:54 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 16:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 16:57:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 16:58:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d8c6b0eb8c3c505236b6ba8f4abeac7cb42c568eaf1638d25605157eed1665`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48182b80525569a49c82ed71c8174f895558d9cb63f669e97286a51ffc26a6`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 1.8 MB (1759589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374c08338c9f1b9019e7e9285ef3d48d0f993f4714a4cbdb5d918dbf578488c3`  
		Last Modified: Tue, 12 Jan 2021 16:58:26 GMT  
		Size: 5.3 MB (5285488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3720b24b60513881270a650b3c1d4177311c5c61ba11e7333f0231487e96596`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97338a06275c6f888b2a3c5fe0b46e06182ab49c90fb9eba4c659df33d10c06e`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:969538e0bd3f0f122782eb6c61db00162aff06e57f195fb7ace7ae809105ac13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33780003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12318f64d90b9d0808ffaa7b23d758bc88b955d911c00951492f829cdd34c72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 15:42:12 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 15:42:20 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:42:21 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 15:42:21 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 15:42:22 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 15:43:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 15:43:10 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 15:43:10 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 15:43:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 15:43:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 15:43:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0eb9193d09b9481c9b7e8fb170147ce6e276d8856a469a550dec5cc90f7a03`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2415476e63e7d74ef4ca52faea84bfe67a05fe3a41a47e686bdd2cf3b02f85e`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 2.0 MB (2007856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f5953f7f6533ef92426e5d329b897f1907b7330ff21c1e496fbb13c1b26665`  
		Last Modified: Tue, 12 Jan 2021 15:43:54 GMT  
		Size: 5.9 MB (5905445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2b2ae8ded9d7b7e98010d34f8ee794a0a263558bf21efe4b7d11635912c0d9`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadf145025c1ea60655010dbbec8968401844445366f2b5d747e43c7c5c9d4a`  
		Last Modified: Tue, 12 Jan 2021 15:43:46 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:c52d50d68d3bf72bbc961fae84e92d8cdaa061fc499248160b21f00f75c92e57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41535877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb514975d8dd949f947658497f4cd64bd2d5e5290b67e7536c61242ab41e2160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:35:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 03:35:59 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:35:59 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 03:36:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 03:36:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 03:36:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 03:36:31 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 03:36:31 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 03:36:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 03:36:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 03:36:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae7ed45a540b81c1438ebda1856d950d9f22d471261017cee150ae44932e51`  
		Last Modified: Tue, 12 Jan 2021 03:36:55 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5731e457264a48ebae724947ba8a4074df0cf2c7bb83f2a09bb2719add7a6de5`  
		Last Modified: Tue, 12 Jan 2021 03:36:56 GMT  
		Size: 2.1 MB (2132528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c7122a22a25bc5e765da780d4cb941efbcf58e2ff86d8fa040f99a07ac1e2e`  
		Last Modified: Tue, 12 Jan 2021 03:37:00 GMT  
		Size: 11.6 MB (11633191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388a70059ec0f0ead585cc8fda996f88c967af935dc16e884f488f2419810615`  
		Last Modified: Tue, 12 Jan 2021 03:36:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7120861ce4e70688817e734037c5d8ac88a9d1dd0285babe73f1950c6ece48`  
		Last Modified: Tue, 12 Jan 2021 03:36:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:2c5c7421c8ddb9e24d202b0b0f77f7354cca4312bb92fd52b19e3e3d1deb1455
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33909503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:130497a6932d05f130672da9e0c0c050ccdeed9288a72445f94bb50297b51440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:09:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 16:10:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:10:06 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 16:10:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 16:10:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 16:11:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 16:11:15 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 16:11:16 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 16:11:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 16:11:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 16:11:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa189ea5f1588e15d59aea364d7de5cf737660a7be5b43b7838447509c32fcf5`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8d546d9d0c67dd04e87cf92d1a953c59c48c19c4db573963fe4364487cc71f`  
		Last Modified: Tue, 12 Jan 2021 16:11:45 GMT  
		Size: 1.7 MB (1712346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340c9dd0d095f9bbe833a6c77c9e39053c0f4e19ce8c5d830747f9e30eac6525`  
		Last Modified: Tue, 12 Jan 2021 16:11:50 GMT  
		Size: 6.4 MB (6416289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bd43028d62609898d5fb217183fa9057c98781503e5330eadb3ad69932e4c`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad75ef390a2ace5a55e7f62becd07b6ca302b837691052bef8a2cd259b290d1`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:84ac8fc004070cc9c2effe0bb5054983c3b9ddc67d98f29310d5ccb7b6e0317a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39490582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18323e6de87099c0fdb5d1f21f7d13b343c56015aa0c28f67210e1773adf20fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:15:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 04:17:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:17:15 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 04:17:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 04:17:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 04:25:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:25:48 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 04:25:57 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 04:25:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 04:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 04:26:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46b97146405ece3ed453ad4ebc496b4b66b0fff54fdc49d2f4d3175043dffaf`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74075dd02f1d1e43b4fc1df6e050d800b9cee069d728e418758c5de00c8aab8`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 2.2 MB (2225177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea580c66676d35f6b86a60aed47a5cc5d25cb3a5d40d018953269820a453e5c`  
		Last Modified: Tue, 09 Feb 2021 04:26:41 GMT  
		Size: 6.7 MB (6743685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e9b505e0637e70b6aeacc7c2b4871dae0dc64900ccc75b80a1cb38714f859`  
		Last Modified: Tue, 09 Feb 2021 04:26:39 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37ff63f62cb2d6c72f328cc4550e6e65dc3382a23b9d6dd4e61a8d6752d0ecc`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:e1324194f0c52dc9f439b3ffcbe90f7063ed357377449c6e03ac3b1e99c9b922
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33477883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd7089a6ca9e042116c7af0c6f1e0972068d5dab27a545d24e1442f6a42b11a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:33:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 06:33:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:33:42 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 06:33:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 06:33:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 06:33:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 06:33:59 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 06:33:59 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 06:33:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 06:34:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:032413a44cf56b097e48b8221bf475ca1bec26e7a27f35fe61d699366a335b79`  
		Last Modified: Tue, 09 Feb 2021 02:45:31 GMT  
		Size: 25.7 MB (25710021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b494d8c5eab48f88712e47a52fa76da28e3b84d610e47c02ef6554cc1e57e98a`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee2f8e8efcd7e5d4ee3b434aed6008829ab2a40fc4e406d28c78b30a00a46d`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 1.8 MB (1821962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ff6c2fa7826622f66fc54c0ce06350d1802aaf2e378e77109208395d04b813`  
		Last Modified: Tue, 09 Feb 2021 06:34:20 GMT  
		Size: 5.9 MB (5943696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d941fa4c020c2b7bee864d1838e2a9a16d366a7f438cfb3ca5bf698a54491a7`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156da7b644b5b54170a00a318c3f2c9b93383aff76d10e828cbec301ad2aac2e`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:c8fed446657ff451ffc9455f0850478c18864fdb2a3b36791e069fedd2d1f182
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
$ docker pull spiped@sha256:813fe508ddf7ef14c654e08581a59df5889155822eb779846196b8e849333938
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36263367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67f39dd2d121caaec0db3bb313564c512f9f974333b8a772963e9a9790a21a3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:21:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 11:21:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:21:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 11:21:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 11:21:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 11:22:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 11:22:13 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 11:22:14 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 11:22:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 11:22:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 11:22:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de752b69da20dffa4f368194c801b91db7f8109eb73f00e28fcf2534595c2391`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29700ba41d506288d95fe910fe16a1412fdf652d9919afe82028b5ee5b3c04ca`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 2.1 MB (2128396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412d577285af429a0e5119c64eb42081167590075ec5fb38a4d4433890b406ba`  
		Last Modified: Tue, 09 Feb 2021 11:22:40 GMT  
		Size: 7.0 MB (7037659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc602331c59adaf25976f51dc954d66801d075f027483281c6b79bd2f12c468`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3991a274f6591f9860d4f7e3d73124d6024fd27dc097414d36cda87813ef0619`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:7f6d7dcae2bcbc63a71c78634690325aa893f07b23ebdf89d495772e2b76e9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32161112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7630b8d3c6a6778b6bf060e33944e07408a5d869c0790a7912fdb44c722221d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:43:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 11:43:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:43:33 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 11:43:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 11:43:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 11:44:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 11:44:28 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 11:44:29 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 11:44:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 11:44:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 11:44:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8e683fcc73f4da7d69ce1d5f4e1d77510aa459490068f38db2d8663698b391a0`  
		Last Modified: Tue, 09 Feb 2021 02:59:07 GMT  
		Size: 24.8 MB (24839297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346f1f77623bfcedac114c95542f4a432dbfac2903c21d7af096733db6f08d7a`  
		Last Modified: Tue, 09 Feb 2021 11:44:58 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46e79f1e8ee1ac5539cad7eefe848b44ce737e874098030fc6156b53ef573a9`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 1.8 MB (1839405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c4f4a4d55f4bff867187ec0fc856d3831a4013bc7b2439663a05c05e0bceba`  
		Last Modified: Tue, 09 Feb 2021 11:45:01 GMT  
		Size: 5.5 MB (5480212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722e4239f41acf1439f868feb56543ec05a7990de0b7e19b785a656ed9cc8245`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3795fccfaef5453c447609dbd35488bfe50615dbc8aabc29d60f5c70747a28`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3ac6871810ed67f5b21e7cd83802fdae6ecb8cc0adcf6f04aaeb1bb55469b360
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29763190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:618f6b2b1cf55feedae7e3db3ca36f7b0e57e0e8df3027fa07ea587c77c1fcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:56:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 16:56:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:56:54 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 16:56:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 16:56:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 16:57:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 16:57:52 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 16:57:54 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 16:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 16:57:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 16:58:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d8c6b0eb8c3c505236b6ba8f4abeac7cb42c568eaf1638d25605157eed1665`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48182b80525569a49c82ed71c8174f895558d9cb63f669e97286a51ffc26a6`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 1.8 MB (1759589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374c08338c9f1b9019e7e9285ef3d48d0f993f4714a4cbdb5d918dbf578488c3`  
		Last Modified: Tue, 12 Jan 2021 16:58:26 GMT  
		Size: 5.3 MB (5285488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3720b24b60513881270a650b3c1d4177311c5c61ba11e7333f0231487e96596`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97338a06275c6f888b2a3c5fe0b46e06182ab49c90fb9eba4c659df33d10c06e`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:969538e0bd3f0f122782eb6c61db00162aff06e57f195fb7ace7ae809105ac13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33780003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12318f64d90b9d0808ffaa7b23d758bc88b955d911c00951492f829cdd34c72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 15:42:12 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 15:42:20 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:42:21 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 15:42:21 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 15:42:22 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 15:43:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 15:43:10 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 15:43:10 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 15:43:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 15:43:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 15:43:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0eb9193d09b9481c9b7e8fb170147ce6e276d8856a469a550dec5cc90f7a03`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2415476e63e7d74ef4ca52faea84bfe67a05fe3a41a47e686bdd2cf3b02f85e`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 2.0 MB (2007856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f5953f7f6533ef92426e5d329b897f1907b7330ff21c1e496fbb13c1b26665`  
		Last Modified: Tue, 12 Jan 2021 15:43:54 GMT  
		Size: 5.9 MB (5905445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2b2ae8ded9d7b7e98010d34f8ee794a0a263558bf21efe4b7d11635912c0d9`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadf145025c1ea60655010dbbec8968401844445366f2b5d747e43c7c5c9d4a`  
		Last Modified: Tue, 12 Jan 2021 15:43:46 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:c52d50d68d3bf72bbc961fae84e92d8cdaa061fc499248160b21f00f75c92e57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41535877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb514975d8dd949f947658497f4cd64bd2d5e5290b67e7536c61242ab41e2160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:35:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 03:35:59 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:35:59 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 03:36:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 03:36:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 03:36:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 03:36:31 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 03:36:31 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 03:36:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 03:36:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 03:36:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae7ed45a540b81c1438ebda1856d950d9f22d471261017cee150ae44932e51`  
		Last Modified: Tue, 12 Jan 2021 03:36:55 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5731e457264a48ebae724947ba8a4074df0cf2c7bb83f2a09bb2719add7a6de5`  
		Last Modified: Tue, 12 Jan 2021 03:36:56 GMT  
		Size: 2.1 MB (2132528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c7122a22a25bc5e765da780d4cb941efbcf58e2ff86d8fa040f99a07ac1e2e`  
		Last Modified: Tue, 12 Jan 2021 03:37:00 GMT  
		Size: 11.6 MB (11633191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388a70059ec0f0ead585cc8fda996f88c967af935dc16e884f488f2419810615`  
		Last Modified: Tue, 12 Jan 2021 03:36:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7120861ce4e70688817e734037c5d8ac88a9d1dd0285babe73f1950c6ece48`  
		Last Modified: Tue, 12 Jan 2021 03:36:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:2c5c7421c8ddb9e24d202b0b0f77f7354cca4312bb92fd52b19e3e3d1deb1455
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33909503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:130497a6932d05f130672da9e0c0c050ccdeed9288a72445f94bb50297b51440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:09:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 16:10:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:10:06 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 16:10:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 16:10:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 16:11:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 16:11:15 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 16:11:16 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 16:11:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 16:11:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 16:11:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa189ea5f1588e15d59aea364d7de5cf737660a7be5b43b7838447509c32fcf5`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8d546d9d0c67dd04e87cf92d1a953c59c48c19c4db573963fe4364487cc71f`  
		Last Modified: Tue, 12 Jan 2021 16:11:45 GMT  
		Size: 1.7 MB (1712346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340c9dd0d095f9bbe833a6c77c9e39053c0f4e19ce8c5d830747f9e30eac6525`  
		Last Modified: Tue, 12 Jan 2021 16:11:50 GMT  
		Size: 6.4 MB (6416289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bd43028d62609898d5fb217183fa9057c98781503e5330eadb3ad69932e4c`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad75ef390a2ace5a55e7f62becd07b6ca302b837691052bef8a2cd259b290d1`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:84ac8fc004070cc9c2effe0bb5054983c3b9ddc67d98f29310d5ccb7b6e0317a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39490582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18323e6de87099c0fdb5d1f21f7d13b343c56015aa0c28f67210e1773adf20fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:15:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 04:17:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:17:15 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 04:17:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 04:17:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 04:25:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:25:48 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 04:25:57 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 04:25:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 04:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 04:26:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46b97146405ece3ed453ad4ebc496b4b66b0fff54fdc49d2f4d3175043dffaf`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74075dd02f1d1e43b4fc1df6e050d800b9cee069d728e418758c5de00c8aab8`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 2.2 MB (2225177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea580c66676d35f6b86a60aed47a5cc5d25cb3a5d40d018953269820a453e5c`  
		Last Modified: Tue, 09 Feb 2021 04:26:41 GMT  
		Size: 6.7 MB (6743685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e9b505e0637e70b6aeacc7c2b4871dae0dc64900ccc75b80a1cb38714f859`  
		Last Modified: Tue, 09 Feb 2021 04:26:39 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37ff63f62cb2d6c72f328cc4550e6e65dc3382a23b9d6dd4e61a8d6752d0ecc`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:e1324194f0c52dc9f439b3ffcbe90f7063ed357377449c6e03ac3b1e99c9b922
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33477883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd7089a6ca9e042116c7af0c6f1e0972068d5dab27a545d24e1442f6a42b11a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:33:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 06:33:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:33:42 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 06:33:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 06:33:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 06:33:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 06:33:59 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 06:33:59 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 06:33:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 06:34:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:032413a44cf56b097e48b8221bf475ca1bec26e7a27f35fe61d699366a335b79`  
		Last Modified: Tue, 09 Feb 2021 02:45:31 GMT  
		Size: 25.7 MB (25710021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b494d8c5eab48f88712e47a52fa76da28e3b84d610e47c02ef6554cc1e57e98a`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee2f8e8efcd7e5d4ee3b434aed6008829ab2a40fc4e406d28c78b30a00a46d`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 1.8 MB (1821962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ff6c2fa7826622f66fc54c0ce06350d1802aaf2e378e77109208395d04b813`  
		Last Modified: Tue, 09 Feb 2021 06:34:20 GMT  
		Size: 5.9 MB (5943696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d941fa4c020c2b7bee864d1838e2a9a16d366a7f438cfb3ca5bf698a54491a7`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156da7b644b5b54170a00a318c3f2c9b93383aff76d10e828cbec301ad2aac2e`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:c8fed446657ff451ffc9455f0850478c18864fdb2a3b36791e069fedd2d1f182
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
$ docker pull spiped@sha256:813fe508ddf7ef14c654e08581a59df5889155822eb779846196b8e849333938
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36263367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67f39dd2d121caaec0db3bb313564c512f9f974333b8a772963e9a9790a21a3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:21:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 11:21:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:21:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 11:21:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 11:21:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 11:22:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 11:22:13 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 11:22:14 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 11:22:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 11:22:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 11:22:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de752b69da20dffa4f368194c801b91db7f8109eb73f00e28fcf2534595c2391`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29700ba41d506288d95fe910fe16a1412fdf652d9919afe82028b5ee5b3c04ca`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 2.1 MB (2128396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412d577285af429a0e5119c64eb42081167590075ec5fb38a4d4433890b406ba`  
		Last Modified: Tue, 09 Feb 2021 11:22:40 GMT  
		Size: 7.0 MB (7037659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc602331c59adaf25976f51dc954d66801d075f027483281c6b79bd2f12c468`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3991a274f6591f9860d4f7e3d73124d6024fd27dc097414d36cda87813ef0619`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:7f6d7dcae2bcbc63a71c78634690325aa893f07b23ebdf89d495772e2b76e9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32161112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7630b8d3c6a6778b6bf060e33944e07408a5d869c0790a7912fdb44c722221d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:43:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 11:43:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:43:33 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 11:43:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 11:43:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 11:44:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 11:44:28 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 11:44:29 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 11:44:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 11:44:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 11:44:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8e683fcc73f4da7d69ce1d5f4e1d77510aa459490068f38db2d8663698b391a0`  
		Last Modified: Tue, 09 Feb 2021 02:59:07 GMT  
		Size: 24.8 MB (24839297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346f1f77623bfcedac114c95542f4a432dbfac2903c21d7af096733db6f08d7a`  
		Last Modified: Tue, 09 Feb 2021 11:44:58 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46e79f1e8ee1ac5539cad7eefe848b44ce737e874098030fc6156b53ef573a9`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 1.8 MB (1839405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c4f4a4d55f4bff867187ec0fc856d3831a4013bc7b2439663a05c05e0bceba`  
		Last Modified: Tue, 09 Feb 2021 11:45:01 GMT  
		Size: 5.5 MB (5480212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722e4239f41acf1439f868feb56543ec05a7990de0b7e19b785a656ed9cc8245`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3795fccfaef5453c447609dbd35488bfe50615dbc8aabc29d60f5c70747a28`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3ac6871810ed67f5b21e7cd83802fdae6ecb8cc0adcf6f04aaeb1bb55469b360
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29763190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:618f6b2b1cf55feedae7e3db3ca36f7b0e57e0e8df3027fa07ea587c77c1fcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:56:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 16:56:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:56:54 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 16:56:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 16:56:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 16:57:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 16:57:52 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 16:57:54 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 16:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 16:57:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 16:58:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d8c6b0eb8c3c505236b6ba8f4abeac7cb42c568eaf1638d25605157eed1665`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48182b80525569a49c82ed71c8174f895558d9cb63f669e97286a51ffc26a6`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 1.8 MB (1759589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374c08338c9f1b9019e7e9285ef3d48d0f993f4714a4cbdb5d918dbf578488c3`  
		Last Modified: Tue, 12 Jan 2021 16:58:26 GMT  
		Size: 5.3 MB (5285488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3720b24b60513881270a650b3c1d4177311c5c61ba11e7333f0231487e96596`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97338a06275c6f888b2a3c5fe0b46e06182ab49c90fb9eba4c659df33d10c06e`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:969538e0bd3f0f122782eb6c61db00162aff06e57f195fb7ace7ae809105ac13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33780003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12318f64d90b9d0808ffaa7b23d758bc88b955d911c00951492f829cdd34c72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 15:42:12 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 15:42:20 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:42:21 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 15:42:21 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 15:42:22 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 15:43:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 15:43:10 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 15:43:10 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 15:43:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 15:43:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 15:43:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0eb9193d09b9481c9b7e8fb170147ce6e276d8856a469a550dec5cc90f7a03`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2415476e63e7d74ef4ca52faea84bfe67a05fe3a41a47e686bdd2cf3b02f85e`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 2.0 MB (2007856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f5953f7f6533ef92426e5d329b897f1907b7330ff21c1e496fbb13c1b26665`  
		Last Modified: Tue, 12 Jan 2021 15:43:54 GMT  
		Size: 5.9 MB (5905445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2b2ae8ded9d7b7e98010d34f8ee794a0a263558bf21efe4b7d11635912c0d9`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadf145025c1ea60655010dbbec8968401844445366f2b5d747e43c7c5c9d4a`  
		Last Modified: Tue, 12 Jan 2021 15:43:46 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:c52d50d68d3bf72bbc961fae84e92d8cdaa061fc499248160b21f00f75c92e57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41535877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb514975d8dd949f947658497f4cd64bd2d5e5290b67e7536c61242ab41e2160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:35:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 03:35:59 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:35:59 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 03:36:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 03:36:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 03:36:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 03:36:31 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 03:36:31 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 03:36:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 03:36:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 03:36:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae7ed45a540b81c1438ebda1856d950d9f22d471261017cee150ae44932e51`  
		Last Modified: Tue, 12 Jan 2021 03:36:55 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5731e457264a48ebae724947ba8a4074df0cf2c7bb83f2a09bb2719add7a6de5`  
		Last Modified: Tue, 12 Jan 2021 03:36:56 GMT  
		Size: 2.1 MB (2132528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c7122a22a25bc5e765da780d4cb941efbcf58e2ff86d8fa040f99a07ac1e2e`  
		Last Modified: Tue, 12 Jan 2021 03:37:00 GMT  
		Size: 11.6 MB (11633191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388a70059ec0f0ead585cc8fda996f88c967af935dc16e884f488f2419810615`  
		Last Modified: Tue, 12 Jan 2021 03:36:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7120861ce4e70688817e734037c5d8ac88a9d1dd0285babe73f1950c6ece48`  
		Last Modified: Tue, 12 Jan 2021 03:36:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:2c5c7421c8ddb9e24d202b0b0f77f7354cca4312bb92fd52b19e3e3d1deb1455
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33909503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:130497a6932d05f130672da9e0c0c050ccdeed9288a72445f94bb50297b51440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:09:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 16:10:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:10:06 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 16:10:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 16:10:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 16:11:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 16:11:15 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 16:11:16 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 16:11:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 16:11:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 16:11:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa189ea5f1588e15d59aea364d7de5cf737660a7be5b43b7838447509c32fcf5`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8d546d9d0c67dd04e87cf92d1a953c59c48c19c4db573963fe4364487cc71f`  
		Last Modified: Tue, 12 Jan 2021 16:11:45 GMT  
		Size: 1.7 MB (1712346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340c9dd0d095f9bbe833a6c77c9e39053c0f4e19ce8c5d830747f9e30eac6525`  
		Last Modified: Tue, 12 Jan 2021 16:11:50 GMT  
		Size: 6.4 MB (6416289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bd43028d62609898d5fb217183fa9057c98781503e5330eadb3ad69932e4c`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad75ef390a2ace5a55e7f62becd07b6ca302b837691052bef8a2cd259b290d1`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:84ac8fc004070cc9c2effe0bb5054983c3b9ddc67d98f29310d5ccb7b6e0317a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39490582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18323e6de87099c0fdb5d1f21f7d13b343c56015aa0c28f67210e1773adf20fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:15:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 04:17:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:17:15 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 04:17:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 04:17:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 04:25:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:25:48 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 04:25:57 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 04:25:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 04:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 04:26:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46b97146405ece3ed453ad4ebc496b4b66b0fff54fdc49d2f4d3175043dffaf`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74075dd02f1d1e43b4fc1df6e050d800b9cee069d728e418758c5de00c8aab8`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 2.2 MB (2225177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea580c66676d35f6b86a60aed47a5cc5d25cb3a5d40d018953269820a453e5c`  
		Last Modified: Tue, 09 Feb 2021 04:26:41 GMT  
		Size: 6.7 MB (6743685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e9b505e0637e70b6aeacc7c2b4871dae0dc64900ccc75b80a1cb38714f859`  
		Last Modified: Tue, 09 Feb 2021 04:26:39 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37ff63f62cb2d6c72f328cc4550e6e65dc3382a23b9d6dd4e61a8d6752d0ecc`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:e1324194f0c52dc9f439b3ffcbe90f7063ed357377449c6e03ac3b1e99c9b922
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33477883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd7089a6ca9e042116c7af0c6f1e0972068d5dab27a545d24e1442f6a42b11a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:33:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 06:33:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:33:42 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 06:33:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 06:33:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 06:33:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 06:33:59 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 06:33:59 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 06:33:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 06:34:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:032413a44cf56b097e48b8221bf475ca1bec26e7a27f35fe61d699366a335b79`  
		Last Modified: Tue, 09 Feb 2021 02:45:31 GMT  
		Size: 25.7 MB (25710021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b494d8c5eab48f88712e47a52fa76da28e3b84d610e47c02ef6554cc1e57e98a`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee2f8e8efcd7e5d4ee3b434aed6008829ab2a40fc4e406d28c78b30a00a46d`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 1.8 MB (1821962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ff6c2fa7826622f66fc54c0ce06350d1802aaf2e378e77109208395d04b813`  
		Last Modified: Tue, 09 Feb 2021 06:34:20 GMT  
		Size: 5.9 MB (5943696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d941fa4c020c2b7bee864d1838e2a9a16d366a7f438cfb3ca5bf698a54491a7`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156da7b644b5b54170a00a318c3f2c9b93383aff76d10e828cbec301ad2aac2e`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:06db401e6cdc6b37d823da2445cc1aaa7b9117735ed53abdca1f42e125d0585e
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
$ docker pull spiped@sha256:1826c56868f7156c24efa7b2cb94fa135d9edac66e2c507c15599ef1052a58d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3018930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39edadb9afd728bb4c7aa9c9ca136383fa16baa0d779d74aa53cb790a14ba177`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:10:13 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 13:10:14 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 13:10:14 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 13:10:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 13:10:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 13:10:33 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 13:10:33 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 13:10:34 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 13:10:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 13:10:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:10:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9ef1fbc142d53554166678d61dfc37fa8f029854a42bba9b28cee4ee504229`  
		Last Modified: Thu, 17 Dec 2020 13:10:57 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5610467a4772716dbbf21461ebb36f9836506180692281d60007d0048b6c84c1`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29938cad4c5e56e1bd9f448e09072b5861291196e91858d8969a39f8792bbd13`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 211.4 KB (211436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eb7102896c3e5adb2fe2dd8c1b13d58a06a214eb129b1fea092a7259d32f83`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8648cf2d9f203bee37b42ca68305f5f730cef951ac6f80d256b90fa87c425ed2`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:ce639a63f71d2cdec9d8774920ccffba505660024271c0f86879f35c57be4bd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c377ae79c110a989108b20bcf35a34723b0a5e1feedc97affe7edd5d624ebe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:26:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:26:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:26:28 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:26:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:26:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:27:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:27:02 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:27:04 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:27:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:27:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c87433d479dc23c9539100c0f11e9e3b197362507032fbb58a359f9af6938ad`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574dae3bebb6bd72bbc35057f4f5819ad3c993d2f2f2e508d5d1c641cc7b072c`  
		Last Modified: Thu, 17 Dec 2020 08:27:23 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e99931839475dee720e62bd05025bab2f33d61e5504d82ef76579b2216d246f`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 198.4 KB (198364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1cafc00bbb6ac8486335e8aa336895edd9b32ba24b37f6ac5a1550e7b564dd`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910a2a05776ea9cd46dd3a82cf2d75c171e8374474307ec99258637248be19c6`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c553ee2ee63a0a3b81d55b74cccfd0822aa0d39478cbe244da649327d7378877
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2607674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f565d25e6081c4dc1a89fdd2ce41032b5e36b9718e9d6753241aef4d52fd5857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:51:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 07:51:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 07:51:34 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 07:52:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 07:52:06 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 07:52:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 07:52:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ebcee7f306695dc196f62d17026042c5bb965afb99dc3f61cf3660372fb425`  
		Last Modified: Thu, 17 Dec 2020 07:52:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d0f202df8c4f27bbfd60a7efd7b13c22b84068edc0ca36a84f3d0cef40b04`  
		Last Modified: Thu, 17 Dec 2020 07:52:38 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329dcbf8165ef792987d3a3a4d2004c926f230fdc1381cbf6a82bcc10796ce00`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 191.6 KB (191627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0677924e9eeea46e3278a2d85941c9bf37ff241d1c5abc3dd8d7899ddd281f13`  
		Last Modified: Thu, 17 Dec 2020 07:52:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbcee47f8c7d2d898483b927e4cd4e573468cf5c65726dc9d4d6811d43d15b0`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:877752aaceeae2daafd99b99639b48e6e2edfdab8c4eec7ab65073ff51e3aec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2921363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ad953bc3ea727f1b993a5bf8e70f4a74892a11ccd04bd121db0ef4ff8c9923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:38:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 04:38:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 04:38:58 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 04:38:59 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 04:39:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 04:39:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 04:39:36 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 04:39:37 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 04:39:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:39:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:39:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712d49e6440c4dc671fba2339c89f5d20467413745b8be19d70e0caaa651b25`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46c964edde07c97f1a27616640abab3ba174358903d509990270ad0a2c6dc5d`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb0f4f45b7c8150ecdffd49a2be270290efe1d1914ddf26da323f04a09203f1`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 203.8 KB (203819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea32c0c99096d4ce306eaff76344fbcde6b609125bce5cec33ed8cc8aaf3e8e2`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c655ecb1758a97af788cb42b035b9eacbee75d2ffe44c098d8bdeeb2996a42`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:c5d418e34444f6d478d945a55040be05044d7d27d2b7425c865deec7469028ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3023775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673445a2b971548ccffbbfc02bda2826e68cf38a2a6c9a8ab2a453459e9b855a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:04:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:04:42 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:04:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:05:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:05:01 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:05:01 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:05:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:05:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88caf4151d80452ec38c6b73bf733c47dc1dd565b34845918a13055338194cd9`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfd8ff82624c004a1d518dd0620b7c92f26f305c594b393d03986f1df372296`  
		Last Modified: Thu, 17 Dec 2020 08:05:19 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c5b95ca7e1c6efe8446fbf561a280767913d23cb32d9bf8cf59cbcb200a58`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 221.2 KB (221212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd2a8e2aad9b417ba96239e3726bcf40bd04d305d7b370576f5ccee99f30c1`  
		Last Modified: Thu, 17 Dec 2020 08:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421075b71f485fcb355987b77b3982a799a77ca1371cd77182353b5907029769`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27472699e225b3cecb93aff593715a1b1e593b3c5ccaee677f61c0532eb269d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff055d1554a2790d3299ce836ec2184d1da25b67626dff0e7975227bf3b8bf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:36:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 02:36:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 02:36:27 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 02:36:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 02:36:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 02:37:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 02:37:08 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 02:37:13 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 02:37:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 02:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:37:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e42c0a7b0024477cc166777ef19c2e1cd63e0a016df217c81f1ad17d6e867e`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed98d2a30fae7fccd64cce03806134befaaadcf8dd7390c74a3cec0b8c8d55`  
		Last Modified: Thu, 17 Dec 2020 02:37:57 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d69d8e55782510c684534af422909754a79f1945e12e464301f021c043e02de`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 219.0 KB (219044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d639ec471f63a1b41aa949a7db2bf31a68ebb304787e4d0d24a16985a5b8c882`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ccb1b04ca97a7dd2ac55b1dc8fc9f953df9822d19116e86af691d4ded7d0ad`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:22d84d581716a2a5f1de6d10cc10546736d493a1a1845c11cc0f032874ef4b2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2778532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3afb9e2f140472d2b9e0335b33e697b677876f1df6e2c3a8ba34faf287acfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:22:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 01:22:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 01:23:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 01:23:07 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 01:23:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 01:23:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28749ff9b137302419a963c66675081a7a31fb1f635d6857c5d209dcda5a6c`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7f79fb0545a28cb5372937795983c817914013736f6a9846b56e453ec52dd4`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a676d107f0804a389a41a4d1fcb3c102fdceee14a9dffd21de8183a741b432d`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 203.0 KB (203013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d3efd6ce468d1c41c42a12f96a4727eed04b45646906ff3af1dfb105340eb2`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497abbb6277ccc692da7032b7c6a8fa32562381af33b6ee86a4529970ec1aa3`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:06db401e6cdc6b37d823da2445cc1aaa7b9117735ed53abdca1f42e125d0585e
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
$ docker pull spiped@sha256:1826c56868f7156c24efa7b2cb94fa135d9edac66e2c507c15599ef1052a58d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3018930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39edadb9afd728bb4c7aa9c9ca136383fa16baa0d779d74aa53cb790a14ba177`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:10:13 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 13:10:14 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 13:10:14 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 13:10:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 13:10:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 13:10:33 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 13:10:33 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 13:10:34 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 13:10:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 13:10:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:10:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9ef1fbc142d53554166678d61dfc37fa8f029854a42bba9b28cee4ee504229`  
		Last Modified: Thu, 17 Dec 2020 13:10:57 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5610467a4772716dbbf21461ebb36f9836506180692281d60007d0048b6c84c1`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29938cad4c5e56e1bd9f448e09072b5861291196e91858d8969a39f8792bbd13`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 211.4 KB (211436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eb7102896c3e5adb2fe2dd8c1b13d58a06a214eb129b1fea092a7259d32f83`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8648cf2d9f203bee37b42ca68305f5f730cef951ac6f80d256b90fa87c425ed2`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:ce639a63f71d2cdec9d8774920ccffba505660024271c0f86879f35c57be4bd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c377ae79c110a989108b20bcf35a34723b0a5e1feedc97affe7edd5d624ebe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:26:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:26:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:26:28 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:26:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:26:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:27:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:27:02 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:27:04 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:27:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:27:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c87433d479dc23c9539100c0f11e9e3b197362507032fbb58a359f9af6938ad`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574dae3bebb6bd72bbc35057f4f5819ad3c993d2f2f2e508d5d1c641cc7b072c`  
		Last Modified: Thu, 17 Dec 2020 08:27:23 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e99931839475dee720e62bd05025bab2f33d61e5504d82ef76579b2216d246f`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 198.4 KB (198364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1cafc00bbb6ac8486335e8aa336895edd9b32ba24b37f6ac5a1550e7b564dd`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910a2a05776ea9cd46dd3a82cf2d75c171e8374474307ec99258637248be19c6`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c553ee2ee63a0a3b81d55b74cccfd0822aa0d39478cbe244da649327d7378877
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2607674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f565d25e6081c4dc1a89fdd2ce41032b5e36b9718e9d6753241aef4d52fd5857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:51:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 07:51:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 07:51:34 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 07:52:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 07:52:06 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 07:52:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 07:52:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ebcee7f306695dc196f62d17026042c5bb965afb99dc3f61cf3660372fb425`  
		Last Modified: Thu, 17 Dec 2020 07:52:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d0f202df8c4f27bbfd60a7efd7b13c22b84068edc0ca36a84f3d0cef40b04`  
		Last Modified: Thu, 17 Dec 2020 07:52:38 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329dcbf8165ef792987d3a3a4d2004c926f230fdc1381cbf6a82bcc10796ce00`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 191.6 KB (191627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0677924e9eeea46e3278a2d85941c9bf37ff241d1c5abc3dd8d7899ddd281f13`  
		Last Modified: Thu, 17 Dec 2020 07:52:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbcee47f8c7d2d898483b927e4cd4e573468cf5c65726dc9d4d6811d43d15b0`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:877752aaceeae2daafd99b99639b48e6e2edfdab8c4eec7ab65073ff51e3aec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2921363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ad953bc3ea727f1b993a5bf8e70f4a74892a11ccd04bd121db0ef4ff8c9923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:38:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 04:38:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 04:38:58 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 04:38:59 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 04:39:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 04:39:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 04:39:36 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 04:39:37 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 04:39:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:39:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:39:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712d49e6440c4dc671fba2339c89f5d20467413745b8be19d70e0caaa651b25`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46c964edde07c97f1a27616640abab3ba174358903d509990270ad0a2c6dc5d`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb0f4f45b7c8150ecdffd49a2be270290efe1d1914ddf26da323f04a09203f1`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 203.8 KB (203819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea32c0c99096d4ce306eaff76344fbcde6b609125bce5cec33ed8cc8aaf3e8e2`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c655ecb1758a97af788cb42b035b9eacbee75d2ffe44c098d8bdeeb2996a42`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:c5d418e34444f6d478d945a55040be05044d7d27d2b7425c865deec7469028ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3023775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673445a2b971548ccffbbfc02bda2826e68cf38a2a6c9a8ab2a453459e9b855a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:04:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:04:42 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:04:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:05:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:05:01 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:05:01 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:05:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:05:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88caf4151d80452ec38c6b73bf733c47dc1dd565b34845918a13055338194cd9`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfd8ff82624c004a1d518dd0620b7c92f26f305c594b393d03986f1df372296`  
		Last Modified: Thu, 17 Dec 2020 08:05:19 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c5b95ca7e1c6efe8446fbf561a280767913d23cb32d9bf8cf59cbcb200a58`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 221.2 KB (221212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd2a8e2aad9b417ba96239e3726bcf40bd04d305d7b370576f5ccee99f30c1`  
		Last Modified: Thu, 17 Dec 2020 08:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421075b71f485fcb355987b77b3982a799a77ca1371cd77182353b5907029769`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27472699e225b3cecb93aff593715a1b1e593b3c5ccaee677f61c0532eb269d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff055d1554a2790d3299ce836ec2184d1da25b67626dff0e7975227bf3b8bf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:36:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 02:36:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 02:36:27 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 02:36:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 02:36:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 02:37:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 02:37:08 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 02:37:13 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 02:37:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 02:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:37:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e42c0a7b0024477cc166777ef19c2e1cd63e0a016df217c81f1ad17d6e867e`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed98d2a30fae7fccd64cce03806134befaaadcf8dd7390c74a3cec0b8c8d55`  
		Last Modified: Thu, 17 Dec 2020 02:37:57 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d69d8e55782510c684534af422909754a79f1945e12e464301f021c043e02de`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 219.0 KB (219044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d639ec471f63a1b41aa949a7db2bf31a68ebb304787e4d0d24a16985a5b8c882`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ccb1b04ca97a7dd2ac55b1dc8fc9f953df9822d19116e86af691d4ded7d0ad`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:22d84d581716a2a5f1de6d10cc10546736d493a1a1845c11cc0f032874ef4b2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2778532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3afb9e2f140472d2b9e0335b33e697b677876f1df6e2c3a8ba34faf287acfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:22:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 01:22:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 01:23:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 01:23:07 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 01:23:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 01:23:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28749ff9b137302419a963c66675081a7a31fb1f635d6857c5d209dcda5a6c`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7f79fb0545a28cb5372937795983c817914013736f6a9846b56e453ec52dd4`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a676d107f0804a389a41a4d1fcb3c102fdceee14a9dffd21de8183a741b432d`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 203.0 KB (203013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d3efd6ce468d1c41c42a12f96a4727eed04b45646906ff3af1dfb105340eb2`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497abbb6277ccc692da7032b7c6a8fa32562381af33b6ee86a4529970ec1aa3`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:06db401e6cdc6b37d823da2445cc1aaa7b9117735ed53abdca1f42e125d0585e
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
$ docker pull spiped@sha256:1826c56868f7156c24efa7b2cb94fa135d9edac66e2c507c15599ef1052a58d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3018930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39edadb9afd728bb4c7aa9c9ca136383fa16baa0d779d74aa53cb790a14ba177`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:10:13 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 13:10:14 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 13:10:14 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 13:10:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 13:10:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 13:10:33 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 13:10:33 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 13:10:34 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 13:10:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 13:10:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:10:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9ef1fbc142d53554166678d61dfc37fa8f029854a42bba9b28cee4ee504229`  
		Last Modified: Thu, 17 Dec 2020 13:10:57 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5610467a4772716dbbf21461ebb36f9836506180692281d60007d0048b6c84c1`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29938cad4c5e56e1bd9f448e09072b5861291196e91858d8969a39f8792bbd13`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 211.4 KB (211436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eb7102896c3e5adb2fe2dd8c1b13d58a06a214eb129b1fea092a7259d32f83`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8648cf2d9f203bee37b42ca68305f5f730cef951ac6f80d256b90fa87c425ed2`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:ce639a63f71d2cdec9d8774920ccffba505660024271c0f86879f35c57be4bd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c377ae79c110a989108b20bcf35a34723b0a5e1feedc97affe7edd5d624ebe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:26:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:26:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:26:28 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:26:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:26:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:27:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:27:02 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:27:04 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:27:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:27:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c87433d479dc23c9539100c0f11e9e3b197362507032fbb58a359f9af6938ad`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574dae3bebb6bd72bbc35057f4f5819ad3c993d2f2f2e508d5d1c641cc7b072c`  
		Last Modified: Thu, 17 Dec 2020 08:27:23 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e99931839475dee720e62bd05025bab2f33d61e5504d82ef76579b2216d246f`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 198.4 KB (198364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1cafc00bbb6ac8486335e8aa336895edd9b32ba24b37f6ac5a1550e7b564dd`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910a2a05776ea9cd46dd3a82cf2d75c171e8374474307ec99258637248be19c6`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c553ee2ee63a0a3b81d55b74cccfd0822aa0d39478cbe244da649327d7378877
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2607674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f565d25e6081c4dc1a89fdd2ce41032b5e36b9718e9d6753241aef4d52fd5857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:51:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 07:51:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 07:51:34 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 07:52:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 07:52:06 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 07:52:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 07:52:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ebcee7f306695dc196f62d17026042c5bb965afb99dc3f61cf3660372fb425`  
		Last Modified: Thu, 17 Dec 2020 07:52:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d0f202df8c4f27bbfd60a7efd7b13c22b84068edc0ca36a84f3d0cef40b04`  
		Last Modified: Thu, 17 Dec 2020 07:52:38 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329dcbf8165ef792987d3a3a4d2004c926f230fdc1381cbf6a82bcc10796ce00`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 191.6 KB (191627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0677924e9eeea46e3278a2d85941c9bf37ff241d1c5abc3dd8d7899ddd281f13`  
		Last Modified: Thu, 17 Dec 2020 07:52:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbcee47f8c7d2d898483b927e4cd4e573468cf5c65726dc9d4d6811d43d15b0`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:877752aaceeae2daafd99b99639b48e6e2edfdab8c4eec7ab65073ff51e3aec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2921363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ad953bc3ea727f1b993a5bf8e70f4a74892a11ccd04bd121db0ef4ff8c9923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:38:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 04:38:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 04:38:58 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 04:38:59 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 04:39:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 04:39:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 04:39:36 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 04:39:37 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 04:39:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:39:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:39:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712d49e6440c4dc671fba2339c89f5d20467413745b8be19d70e0caaa651b25`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46c964edde07c97f1a27616640abab3ba174358903d509990270ad0a2c6dc5d`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb0f4f45b7c8150ecdffd49a2be270290efe1d1914ddf26da323f04a09203f1`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 203.8 KB (203819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea32c0c99096d4ce306eaff76344fbcde6b609125bce5cec33ed8cc8aaf3e8e2`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c655ecb1758a97af788cb42b035b9eacbee75d2ffe44c098d8bdeeb2996a42`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:c5d418e34444f6d478d945a55040be05044d7d27d2b7425c865deec7469028ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3023775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673445a2b971548ccffbbfc02bda2826e68cf38a2a6c9a8ab2a453459e9b855a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:04:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:04:42 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:04:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:05:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:05:01 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:05:01 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:05:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:05:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88caf4151d80452ec38c6b73bf733c47dc1dd565b34845918a13055338194cd9`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfd8ff82624c004a1d518dd0620b7c92f26f305c594b393d03986f1df372296`  
		Last Modified: Thu, 17 Dec 2020 08:05:19 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c5b95ca7e1c6efe8446fbf561a280767913d23cb32d9bf8cf59cbcb200a58`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 221.2 KB (221212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd2a8e2aad9b417ba96239e3726bcf40bd04d305d7b370576f5ccee99f30c1`  
		Last Modified: Thu, 17 Dec 2020 08:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421075b71f485fcb355987b77b3982a799a77ca1371cd77182353b5907029769`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27472699e225b3cecb93aff593715a1b1e593b3c5ccaee677f61c0532eb269d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff055d1554a2790d3299ce836ec2184d1da25b67626dff0e7975227bf3b8bf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:36:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 02:36:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 02:36:27 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 02:36:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 02:36:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 02:37:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 02:37:08 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 02:37:13 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 02:37:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 02:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:37:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e42c0a7b0024477cc166777ef19c2e1cd63e0a016df217c81f1ad17d6e867e`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed98d2a30fae7fccd64cce03806134befaaadcf8dd7390c74a3cec0b8c8d55`  
		Last Modified: Thu, 17 Dec 2020 02:37:57 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d69d8e55782510c684534af422909754a79f1945e12e464301f021c043e02de`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 219.0 KB (219044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d639ec471f63a1b41aa949a7db2bf31a68ebb304787e4d0d24a16985a5b8c882`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ccb1b04ca97a7dd2ac55b1dc8fc9f953df9822d19116e86af691d4ded7d0ad`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:22d84d581716a2a5f1de6d10cc10546736d493a1a1845c11cc0f032874ef4b2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2778532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3afb9e2f140472d2b9e0335b33e697b677876f1df6e2c3a8ba34faf287acfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:22:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 01:22:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 01:23:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 01:23:07 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 01:23:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 01:23:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28749ff9b137302419a963c66675081a7a31fb1f635d6857c5d209dcda5a6c`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7f79fb0545a28cb5372937795983c817914013736f6a9846b56e453ec52dd4`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a676d107f0804a389a41a4d1fcb3c102fdceee14a9dffd21de8183a741b432d`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 203.0 KB (203013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d3efd6ce468d1c41c42a12f96a4727eed04b45646906ff3af1dfb105340eb2`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497abbb6277ccc692da7032b7c6a8fa32562381af33b6ee86a4529970ec1aa3`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:06db401e6cdc6b37d823da2445cc1aaa7b9117735ed53abdca1f42e125d0585e
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
$ docker pull spiped@sha256:1826c56868f7156c24efa7b2cb94fa135d9edac66e2c507c15599ef1052a58d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3018930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39edadb9afd728bb4c7aa9c9ca136383fa16baa0d779d74aa53cb790a14ba177`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:10:13 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 13:10:14 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 13:10:14 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 13:10:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 13:10:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 13:10:33 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 13:10:33 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 13:10:34 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 13:10:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 13:10:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:10:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9ef1fbc142d53554166678d61dfc37fa8f029854a42bba9b28cee4ee504229`  
		Last Modified: Thu, 17 Dec 2020 13:10:57 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5610467a4772716dbbf21461ebb36f9836506180692281d60007d0048b6c84c1`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29938cad4c5e56e1bd9f448e09072b5861291196e91858d8969a39f8792bbd13`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 211.4 KB (211436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eb7102896c3e5adb2fe2dd8c1b13d58a06a214eb129b1fea092a7259d32f83`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8648cf2d9f203bee37b42ca68305f5f730cef951ac6f80d256b90fa87c425ed2`  
		Last Modified: Thu, 17 Dec 2020 13:10:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:ce639a63f71d2cdec9d8774920ccffba505660024271c0f86879f35c57be4bd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c377ae79c110a989108b20bcf35a34723b0a5e1feedc97affe7edd5d624ebe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:26:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:26:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:26:28 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:26:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:26:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:27:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:27:02 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:27:04 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:27:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:27:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c87433d479dc23c9539100c0f11e9e3b197362507032fbb58a359f9af6938ad`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574dae3bebb6bd72bbc35057f4f5819ad3c993d2f2f2e508d5d1c641cc7b072c`  
		Last Modified: Thu, 17 Dec 2020 08:27:23 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e99931839475dee720e62bd05025bab2f33d61e5504d82ef76579b2216d246f`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 198.4 KB (198364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1cafc00bbb6ac8486335e8aa336895edd9b32ba24b37f6ac5a1550e7b564dd`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910a2a05776ea9cd46dd3a82cf2d75c171e8374474307ec99258637248be19c6`  
		Last Modified: Thu, 17 Dec 2020 08:27:24 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c553ee2ee63a0a3b81d55b74cccfd0822aa0d39478cbe244da649327d7378877
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2607674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f565d25e6081c4dc1a89fdd2ce41032b5e36b9718e9d6753241aef4d52fd5857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:51:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 07:51:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 07:51:34 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 07:51:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 07:52:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 07:52:06 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 07:52:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 07:52:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ebcee7f306695dc196f62d17026042c5bb965afb99dc3f61cf3660372fb425`  
		Last Modified: Thu, 17 Dec 2020 07:52:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d0f202df8c4f27bbfd60a7efd7b13c22b84068edc0ca36a84f3d0cef40b04`  
		Last Modified: Thu, 17 Dec 2020 07:52:38 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329dcbf8165ef792987d3a3a4d2004c926f230fdc1381cbf6a82bcc10796ce00`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 191.6 KB (191627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0677924e9eeea46e3278a2d85941c9bf37ff241d1c5abc3dd8d7899ddd281f13`  
		Last Modified: Thu, 17 Dec 2020 07:52:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbcee47f8c7d2d898483b927e4cd4e573468cf5c65726dc9d4d6811d43d15b0`  
		Last Modified: Thu, 17 Dec 2020 07:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:877752aaceeae2daafd99b99639b48e6e2edfdab8c4eec7ab65073ff51e3aec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2921363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ad953bc3ea727f1b993a5bf8e70f4a74892a11ccd04bd121db0ef4ff8c9923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:38:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 04:38:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 04:38:58 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 04:38:59 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 04:39:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 04:39:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 04:39:36 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 04:39:37 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 04:39:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:39:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:39:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712d49e6440c4dc671fba2339c89f5d20467413745b8be19d70e0caaa651b25`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46c964edde07c97f1a27616640abab3ba174358903d509990270ad0a2c6dc5d`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb0f4f45b7c8150ecdffd49a2be270290efe1d1914ddf26da323f04a09203f1`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 203.8 KB (203819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea32c0c99096d4ce306eaff76344fbcde6b609125bce5cec33ed8cc8aaf3e8e2`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c655ecb1758a97af788cb42b035b9eacbee75d2ffe44c098d8bdeeb2996a42`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:c5d418e34444f6d478d945a55040be05044d7d27d2b7425c865deec7469028ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3023775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673445a2b971548ccffbbfc02bda2826e68cf38a2a6c9a8ab2a453459e9b855a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:04:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 08:04:42 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 08:04:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 08:04:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 08:05:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 08:05:01 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 08:05:01 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 08:05:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:05:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88caf4151d80452ec38c6b73bf733c47dc1dd565b34845918a13055338194cd9`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfd8ff82624c004a1d518dd0620b7c92f26f305c594b393d03986f1df372296`  
		Last Modified: Thu, 17 Dec 2020 08:05:19 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c5b95ca7e1c6efe8446fbf561a280767913d23cb32d9bf8cf59cbcb200a58`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 221.2 KB (221212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd2a8e2aad9b417ba96239e3726bcf40bd04d305d7b370576f5ccee99f30c1`  
		Last Modified: Thu, 17 Dec 2020 08:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421075b71f485fcb355987b77b3982a799a77ca1371cd77182353b5907029769`  
		Last Modified: Thu, 17 Dec 2020 08:05:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27472699e225b3cecb93aff593715a1b1e593b3c5ccaee677f61c0532eb269d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff055d1554a2790d3299ce836ec2184d1da25b67626dff0e7975227bf3b8bf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:36:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 02:36:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 02:36:27 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 02:36:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 02:36:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 02:37:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 02:37:08 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 02:37:13 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 02:37:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 02:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:37:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e42c0a7b0024477cc166777ef19c2e1cd63e0a016df217c81f1ad17d6e867e`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed98d2a30fae7fccd64cce03806134befaaadcf8dd7390c74a3cec0b8c8d55`  
		Last Modified: Thu, 17 Dec 2020 02:37:57 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d69d8e55782510c684534af422909754a79f1945e12e464301f021c043e02de`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 219.0 KB (219044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d639ec471f63a1b41aa949a7db2bf31a68ebb304787e4d0d24a16985a5b8c882`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ccb1b04ca97a7dd2ac55b1dc8fc9f953df9822d19116e86af691d4ded7d0ad`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:22d84d581716a2a5f1de6d10cc10546736d493a1a1845c11cc0f032874ef4b2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2778532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3afb9e2f140472d2b9e0335b33e697b677876f1df6e2c3a8ba34faf287acfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:22:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 01:22:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 01:23:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 01:23:07 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 01:23:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 01:23:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28749ff9b137302419a963c66675081a7a31fb1f635d6857c5d209dcda5a6c`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7f79fb0545a28cb5372937795983c817914013736f6a9846b56e453ec52dd4`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a676d107f0804a389a41a4d1fcb3c102fdceee14a9dffd21de8183a741b432d`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 203.0 KB (203013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d3efd6ce468d1c41c42a12f96a4727eed04b45646906ff3af1dfb105340eb2`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497abbb6277ccc692da7032b7c6a8fa32562381af33b6ee86a4529970ec1aa3`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:c8fed446657ff451ffc9455f0850478c18864fdb2a3b36791e069fedd2d1f182
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
$ docker pull spiped@sha256:813fe508ddf7ef14c654e08581a59df5889155822eb779846196b8e849333938
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36263367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67f39dd2d121caaec0db3bb313564c512f9f974333b8a772963e9a9790a21a3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:21:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 11:21:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:21:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 11:21:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 11:21:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 11:22:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 11:22:13 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 11:22:14 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 11:22:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 11:22:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 11:22:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de752b69da20dffa4f368194c801b91db7f8109eb73f00e28fcf2534595c2391`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29700ba41d506288d95fe910fe16a1412fdf652d9919afe82028b5ee5b3c04ca`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 2.1 MB (2128396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412d577285af429a0e5119c64eb42081167590075ec5fb38a4d4433890b406ba`  
		Last Modified: Tue, 09 Feb 2021 11:22:40 GMT  
		Size: 7.0 MB (7037659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc602331c59adaf25976f51dc954d66801d075f027483281c6b79bd2f12c468`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3991a274f6591f9860d4f7e3d73124d6024fd27dc097414d36cda87813ef0619`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:7f6d7dcae2bcbc63a71c78634690325aa893f07b23ebdf89d495772e2b76e9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32161112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7630b8d3c6a6778b6bf060e33944e07408a5d869c0790a7912fdb44c722221d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:43:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 11:43:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:43:33 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 11:43:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 11:43:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 11:44:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 11:44:28 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 11:44:29 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 11:44:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 11:44:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 11:44:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8e683fcc73f4da7d69ce1d5f4e1d77510aa459490068f38db2d8663698b391a0`  
		Last Modified: Tue, 09 Feb 2021 02:59:07 GMT  
		Size: 24.8 MB (24839297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346f1f77623bfcedac114c95542f4a432dbfac2903c21d7af096733db6f08d7a`  
		Last Modified: Tue, 09 Feb 2021 11:44:58 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46e79f1e8ee1ac5539cad7eefe848b44ce737e874098030fc6156b53ef573a9`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 1.8 MB (1839405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c4f4a4d55f4bff867187ec0fc856d3831a4013bc7b2439663a05c05e0bceba`  
		Last Modified: Tue, 09 Feb 2021 11:45:01 GMT  
		Size: 5.5 MB (5480212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722e4239f41acf1439f868feb56543ec05a7990de0b7e19b785a656ed9cc8245`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3795fccfaef5453c447609dbd35488bfe50615dbc8aabc29d60f5c70747a28`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3ac6871810ed67f5b21e7cd83802fdae6ecb8cc0adcf6f04aaeb1bb55469b360
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29763190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:618f6b2b1cf55feedae7e3db3ca36f7b0e57e0e8df3027fa07ea587c77c1fcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:56:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 16:56:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:56:54 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 16:56:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 16:56:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 16:57:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 16:57:52 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 16:57:54 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 16:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 16:57:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 16:58:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d8c6b0eb8c3c505236b6ba8f4abeac7cb42c568eaf1638d25605157eed1665`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48182b80525569a49c82ed71c8174f895558d9cb63f669e97286a51ffc26a6`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 1.8 MB (1759589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374c08338c9f1b9019e7e9285ef3d48d0f993f4714a4cbdb5d918dbf578488c3`  
		Last Modified: Tue, 12 Jan 2021 16:58:26 GMT  
		Size: 5.3 MB (5285488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3720b24b60513881270a650b3c1d4177311c5c61ba11e7333f0231487e96596`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97338a06275c6f888b2a3c5fe0b46e06182ab49c90fb9eba4c659df33d10c06e`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:969538e0bd3f0f122782eb6c61db00162aff06e57f195fb7ace7ae809105ac13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33780003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12318f64d90b9d0808ffaa7b23d758bc88b955d911c00951492f829cdd34c72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 15:42:12 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 15:42:20 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:42:21 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 15:42:21 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 15:42:22 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 15:43:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 15:43:10 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 15:43:10 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 15:43:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 15:43:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 15:43:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0eb9193d09b9481c9b7e8fb170147ce6e276d8856a469a550dec5cc90f7a03`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2415476e63e7d74ef4ca52faea84bfe67a05fe3a41a47e686bdd2cf3b02f85e`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 2.0 MB (2007856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f5953f7f6533ef92426e5d329b897f1907b7330ff21c1e496fbb13c1b26665`  
		Last Modified: Tue, 12 Jan 2021 15:43:54 GMT  
		Size: 5.9 MB (5905445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2b2ae8ded9d7b7e98010d34f8ee794a0a263558bf21efe4b7d11635912c0d9`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadf145025c1ea60655010dbbec8968401844445366f2b5d747e43c7c5c9d4a`  
		Last Modified: Tue, 12 Jan 2021 15:43:46 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:c52d50d68d3bf72bbc961fae84e92d8cdaa061fc499248160b21f00f75c92e57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41535877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb514975d8dd949f947658497f4cd64bd2d5e5290b67e7536c61242ab41e2160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:35:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 03:35:59 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:35:59 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 03:36:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 03:36:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 03:36:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 03:36:31 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 03:36:31 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 03:36:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 03:36:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 03:36:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae7ed45a540b81c1438ebda1856d950d9f22d471261017cee150ae44932e51`  
		Last Modified: Tue, 12 Jan 2021 03:36:55 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5731e457264a48ebae724947ba8a4074df0cf2c7bb83f2a09bb2719add7a6de5`  
		Last Modified: Tue, 12 Jan 2021 03:36:56 GMT  
		Size: 2.1 MB (2132528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c7122a22a25bc5e765da780d4cb941efbcf58e2ff86d8fa040f99a07ac1e2e`  
		Last Modified: Tue, 12 Jan 2021 03:37:00 GMT  
		Size: 11.6 MB (11633191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388a70059ec0f0ead585cc8fda996f88c967af935dc16e884f488f2419810615`  
		Last Modified: Tue, 12 Jan 2021 03:36:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7120861ce4e70688817e734037c5d8ac88a9d1dd0285babe73f1950c6ece48`  
		Last Modified: Tue, 12 Jan 2021 03:36:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:2c5c7421c8ddb9e24d202b0b0f77f7354cca4312bb92fd52b19e3e3d1deb1455
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33909503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:130497a6932d05f130672da9e0c0c050ccdeed9288a72445f94bb50297b51440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:09:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 16:10:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:10:06 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 16:10:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 16:10:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 16:11:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 16:11:15 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 16:11:16 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 16:11:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 16:11:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 16:11:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa189ea5f1588e15d59aea364d7de5cf737660a7be5b43b7838447509c32fcf5`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8d546d9d0c67dd04e87cf92d1a953c59c48c19c4db573963fe4364487cc71f`  
		Last Modified: Tue, 12 Jan 2021 16:11:45 GMT  
		Size: 1.7 MB (1712346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340c9dd0d095f9bbe833a6c77c9e39053c0f4e19ce8c5d830747f9e30eac6525`  
		Last Modified: Tue, 12 Jan 2021 16:11:50 GMT  
		Size: 6.4 MB (6416289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bd43028d62609898d5fb217183fa9057c98781503e5330eadb3ad69932e4c`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad75ef390a2ace5a55e7f62becd07b6ca302b837691052bef8a2cd259b290d1`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:84ac8fc004070cc9c2effe0bb5054983c3b9ddc67d98f29310d5ccb7b6e0317a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39490582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18323e6de87099c0fdb5d1f21f7d13b343c56015aa0c28f67210e1773adf20fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:15:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 04:17:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:17:15 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 04:17:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 04:17:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 04:25:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:25:48 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 04:25:57 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 04:25:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 04:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 04:26:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46b97146405ece3ed453ad4ebc496b4b66b0fff54fdc49d2f4d3175043dffaf`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74075dd02f1d1e43b4fc1df6e050d800b9cee069d728e418758c5de00c8aab8`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 2.2 MB (2225177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea580c66676d35f6b86a60aed47a5cc5d25cb3a5d40d018953269820a453e5c`  
		Last Modified: Tue, 09 Feb 2021 04:26:41 GMT  
		Size: 6.7 MB (6743685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e9b505e0637e70b6aeacc7c2b4871dae0dc64900ccc75b80a1cb38714f859`  
		Last Modified: Tue, 09 Feb 2021 04:26:39 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37ff63f62cb2d6c72f328cc4550e6e65dc3382a23b9d6dd4e61a8d6752d0ecc`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:e1324194f0c52dc9f439b3ffcbe90f7063ed357377449c6e03ac3b1e99c9b922
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33477883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd7089a6ca9e042116c7af0c6f1e0972068d5dab27a545d24e1442f6a42b11a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:33:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 06:33:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:33:42 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 06:33:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 06:33:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 06:33:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 06:33:59 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 06:33:59 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 06:33:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 06:34:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:032413a44cf56b097e48b8221bf475ca1bec26e7a27f35fe61d699366a335b79`  
		Last Modified: Tue, 09 Feb 2021 02:45:31 GMT  
		Size: 25.7 MB (25710021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b494d8c5eab48f88712e47a52fa76da28e3b84d610e47c02ef6554cc1e57e98a`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee2f8e8efcd7e5d4ee3b434aed6008829ab2a40fc4e406d28c78b30a00a46d`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 1.8 MB (1821962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ff6c2fa7826622f66fc54c0ce06350d1802aaf2e378e77109208395d04b813`  
		Last Modified: Tue, 09 Feb 2021 06:34:20 GMT  
		Size: 5.9 MB (5943696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d941fa4c020c2b7bee864d1838e2a9a16d366a7f438cfb3ca5bf698a54491a7`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156da7b644b5b54170a00a318c3f2c9b93383aff76d10e828cbec301ad2aac2e`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
