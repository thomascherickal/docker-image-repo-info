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
$ docker pull spiped@sha256:cde9e4f1555323e51360ff710044aee086cbdd898bfb0fedd6c40ae721ca7074
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
$ docker pull spiped@sha256:06d3a90eababe7a10ab3aca2c67daf41893a351802ba319beecfe9ed752483cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36276212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d92174c45b324b29b7e88abb4eb1684caf02874e5ac2d4f17c7216462a31f5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 19:04:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 19:04:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:04:56 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 19:04:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 19:04:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 19:05:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 19:05:36 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 19:05:36 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 19:05:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 19:05:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 19:05:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa6da2fcdba0615425a10a7476eacc596cf8e7eefa675a98f5bde79ced32cd8`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b22cf825b4fe47ca058426beb71cb3ff18273aee3e32bd89881912e726db5d`  
		Last Modified: Tue, 12 Jan 2021 19:06:03 GMT  
		Size: 2.1 MB (2128411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded296a693f0eb4b77e16db9ec7a4c9751ecb5f8a53ed59576352d9b9220c402`  
		Last Modified: Tue, 12 Jan 2021 19:06:05 GMT  
		Size: 7.0 MB (7037562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7940bfb150d14dbc1e6abd29a077b7c06321150e49c08097449ef62c6bc6724d`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467c5ffa5950fc15c6929703e9ae99c0a816cda85f18a52401b599dc0f8aa058`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:5bd55a1a73670e68370f209d9dd01c217eb5b6c67598f25bac68f60e27549889
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32173489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811e01c7a839fa25b3fa40b7bffd77378fd7aba6ca8bf106e7f581006320d266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:42:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 10:43:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:43:04 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 10:43:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 10:43:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 10:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 10:44:01 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 10:44:02 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 10:44:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 10:44:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 10:44:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f88dec7258b86e4e8c96100efc159399e0850fae2548f42d46fef4c3ae47f6`  
		Last Modified: Tue, 12 Jan 2021 10:44:33 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92eb800b9e7b936c989b77428553ebd597012e1fd451c62077a5b319c5c5381c`  
		Last Modified: Tue, 12 Jan 2021 10:44:32 GMT  
		Size: 1.8 MB (1839430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192c478305b485d2d6512913428673bf7ccb9da73b48f2fbde43de07bde0b00d`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 5.5 MB (5479951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1e5fcf0c5c7851002a65cbff0bc261cf64ef0cb1e856adf7f699ba5aa83b8`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a0ef96e7bb574336736be33888eadcff04b2105f2d98247d8083da825c65f`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:1ac2a48f4093de84e993dc766d9b9533116ef5b96143b8627502ec0e308d1748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39503719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc39787a552c5d318cef4a3487de1ac8f5ae4e07b32759ac6b13197a8739f99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 15:20:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 15:21:21 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:21:27 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 15:21:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 15:21:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 15:27:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 15:27:44 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 15:27:48 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 15:27:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 15:27:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 15:27:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee4568d92ca67ebb39b4c46eba2c4ae2f896e934c8070bdc0c481404018c390`  
		Last Modified: Tue, 12 Jan 2021 15:28:29 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f9ff8423f2713cccf087b1cdb69e12ccfb4c861cc0dc1214c443d3091e6eac`  
		Last Modified: Tue, 12 Jan 2021 15:28:30 GMT  
		Size: 2.2 MB (2225166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fdad5551173536a86727e4250b94e34355d83020147ceb5ec0f412518e20c4`  
		Last Modified: Tue, 12 Jan 2021 15:28:31 GMT  
		Size: 6.7 MB (6743500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e427569d726352f8287dd512ad5c9b0f1bd0f0ba9b2e8a9d5d9e18b12d48de`  
		Last Modified: Tue, 12 Jan 2021 15:28:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed1f874132ad81fab1ac2244587626a668c8a55413bb109d61fe8983f352624`  
		Last Modified: Tue, 12 Jan 2021 15:28:30 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:d25fc36058d984ef1de9c0061022bd803224e14c6b1a28073a97ac913f5b75e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33491139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be176b022a0a3121121756080606d3f10045f77c7c551fd766467beb596c525`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:22 GMT
ADD file:c01d899d503187f788db0a7d658bf3f2b6541026a4c654707d3272f6d3ffaf58 in / 
# Tue, 12 Jan 2021 00:42:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:54:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 02:54:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:54:11 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 02:54:12 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 02:54:12 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 02:54:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 02:54:39 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 02:54:39 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 02:54:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 02:54:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 02:54:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0e3e06c0bd0347fefe8bde60780e7e551c0cdf1cbcf40be3d052e823d5ec118`  
		Last Modified: Tue, 12 Jan 2021 00:52:32 GMT  
		Size: 25.7 MB (25723406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17512f7809b0e3dc11ab91a97504e20e1aece1b4d7ffd53c61541e59cefb02d`  
		Last Modified: Tue, 12 Jan 2021 02:55:27 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee602ea1b5f7a93780a8ee5fe5f394864b6475f785bc7125fd004e931b106eb`  
		Last Modified: Tue, 12 Jan 2021 02:55:30 GMT  
		Size: 1.8 MB (1822021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93d111b3adf8d1a2c9ad404a750c4c92fe5ee90b0b9d690dd130ce5bf970930`  
		Last Modified: Tue, 12 Jan 2021 02:55:28 GMT  
		Size: 5.9 MB (5943508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af24d5ea6121cd5d4a68c533f97899d07b55a3e356026c5a34d50ca9a7c64070`  
		Last Modified: Tue, 12 Jan 2021 02:55:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81b1a70da6be82ba066d625c23c7da6e01af6578e243e4dcd3c27baf189aba3`  
		Last Modified: Tue, 12 Jan 2021 02:55:31 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:cde9e4f1555323e51360ff710044aee086cbdd898bfb0fedd6c40ae721ca7074
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
$ docker pull spiped@sha256:06d3a90eababe7a10ab3aca2c67daf41893a351802ba319beecfe9ed752483cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36276212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d92174c45b324b29b7e88abb4eb1684caf02874e5ac2d4f17c7216462a31f5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 19:04:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 19:04:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:04:56 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 19:04:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 19:04:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 19:05:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 19:05:36 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 19:05:36 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 19:05:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 19:05:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 19:05:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa6da2fcdba0615425a10a7476eacc596cf8e7eefa675a98f5bde79ced32cd8`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b22cf825b4fe47ca058426beb71cb3ff18273aee3e32bd89881912e726db5d`  
		Last Modified: Tue, 12 Jan 2021 19:06:03 GMT  
		Size: 2.1 MB (2128411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded296a693f0eb4b77e16db9ec7a4c9751ecb5f8a53ed59576352d9b9220c402`  
		Last Modified: Tue, 12 Jan 2021 19:06:05 GMT  
		Size: 7.0 MB (7037562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7940bfb150d14dbc1e6abd29a077b7c06321150e49c08097449ef62c6bc6724d`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467c5ffa5950fc15c6929703e9ae99c0a816cda85f18a52401b599dc0f8aa058`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:5bd55a1a73670e68370f209d9dd01c217eb5b6c67598f25bac68f60e27549889
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32173489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811e01c7a839fa25b3fa40b7bffd77378fd7aba6ca8bf106e7f581006320d266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:42:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 10:43:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:43:04 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 10:43:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 10:43:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 10:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 10:44:01 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 10:44:02 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 10:44:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 10:44:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 10:44:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f88dec7258b86e4e8c96100efc159399e0850fae2548f42d46fef4c3ae47f6`  
		Last Modified: Tue, 12 Jan 2021 10:44:33 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92eb800b9e7b936c989b77428553ebd597012e1fd451c62077a5b319c5c5381c`  
		Last Modified: Tue, 12 Jan 2021 10:44:32 GMT  
		Size: 1.8 MB (1839430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192c478305b485d2d6512913428673bf7ccb9da73b48f2fbde43de07bde0b00d`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 5.5 MB (5479951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1e5fcf0c5c7851002a65cbff0bc261cf64ef0cb1e856adf7f699ba5aa83b8`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a0ef96e7bb574336736be33888eadcff04b2105f2d98247d8083da825c65f`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:1ac2a48f4093de84e993dc766d9b9533116ef5b96143b8627502ec0e308d1748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39503719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc39787a552c5d318cef4a3487de1ac8f5ae4e07b32759ac6b13197a8739f99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 15:20:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 15:21:21 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:21:27 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 15:21:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 15:21:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 15:27:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 15:27:44 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 15:27:48 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 15:27:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 15:27:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 15:27:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee4568d92ca67ebb39b4c46eba2c4ae2f896e934c8070bdc0c481404018c390`  
		Last Modified: Tue, 12 Jan 2021 15:28:29 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f9ff8423f2713cccf087b1cdb69e12ccfb4c861cc0dc1214c443d3091e6eac`  
		Last Modified: Tue, 12 Jan 2021 15:28:30 GMT  
		Size: 2.2 MB (2225166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fdad5551173536a86727e4250b94e34355d83020147ceb5ec0f412518e20c4`  
		Last Modified: Tue, 12 Jan 2021 15:28:31 GMT  
		Size: 6.7 MB (6743500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e427569d726352f8287dd512ad5c9b0f1bd0f0ba9b2e8a9d5d9e18b12d48de`  
		Last Modified: Tue, 12 Jan 2021 15:28:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed1f874132ad81fab1ac2244587626a668c8a55413bb109d61fe8983f352624`  
		Last Modified: Tue, 12 Jan 2021 15:28:30 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:d25fc36058d984ef1de9c0061022bd803224e14c6b1a28073a97ac913f5b75e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33491139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be176b022a0a3121121756080606d3f10045f77c7c551fd766467beb596c525`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:22 GMT
ADD file:c01d899d503187f788db0a7d658bf3f2b6541026a4c654707d3272f6d3ffaf58 in / 
# Tue, 12 Jan 2021 00:42:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:54:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 02:54:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:54:11 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 02:54:12 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 02:54:12 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 02:54:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 02:54:39 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 02:54:39 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 02:54:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 02:54:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 02:54:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0e3e06c0bd0347fefe8bde60780e7e551c0cdf1cbcf40be3d052e823d5ec118`  
		Last Modified: Tue, 12 Jan 2021 00:52:32 GMT  
		Size: 25.7 MB (25723406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17512f7809b0e3dc11ab91a97504e20e1aece1b4d7ffd53c61541e59cefb02d`  
		Last Modified: Tue, 12 Jan 2021 02:55:27 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee602ea1b5f7a93780a8ee5fe5f394864b6475f785bc7125fd004e931b106eb`  
		Last Modified: Tue, 12 Jan 2021 02:55:30 GMT  
		Size: 1.8 MB (1822021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93d111b3adf8d1a2c9ad404a750c4c92fe5ee90b0b9d690dd130ce5bf970930`  
		Last Modified: Tue, 12 Jan 2021 02:55:28 GMT  
		Size: 5.9 MB (5943508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af24d5ea6121cd5d4a68c533f97899d07b55a3e356026c5a34d50ca9a7c64070`  
		Last Modified: Tue, 12 Jan 2021 02:55:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81b1a70da6be82ba066d625c23c7da6e01af6578e243e4dcd3c27baf189aba3`  
		Last Modified: Tue, 12 Jan 2021 02:55:31 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:cde9e4f1555323e51360ff710044aee086cbdd898bfb0fedd6c40ae721ca7074
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
$ docker pull spiped@sha256:06d3a90eababe7a10ab3aca2c67daf41893a351802ba319beecfe9ed752483cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36276212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d92174c45b324b29b7e88abb4eb1684caf02874e5ac2d4f17c7216462a31f5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 19:04:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 19:04:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:04:56 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 19:04:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 19:04:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 19:05:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 19:05:36 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 19:05:36 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 19:05:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 19:05:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 19:05:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa6da2fcdba0615425a10a7476eacc596cf8e7eefa675a98f5bde79ced32cd8`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b22cf825b4fe47ca058426beb71cb3ff18273aee3e32bd89881912e726db5d`  
		Last Modified: Tue, 12 Jan 2021 19:06:03 GMT  
		Size: 2.1 MB (2128411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded296a693f0eb4b77e16db9ec7a4c9751ecb5f8a53ed59576352d9b9220c402`  
		Last Modified: Tue, 12 Jan 2021 19:06:05 GMT  
		Size: 7.0 MB (7037562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7940bfb150d14dbc1e6abd29a077b7c06321150e49c08097449ef62c6bc6724d`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467c5ffa5950fc15c6929703e9ae99c0a816cda85f18a52401b599dc0f8aa058`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:5bd55a1a73670e68370f209d9dd01c217eb5b6c67598f25bac68f60e27549889
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32173489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811e01c7a839fa25b3fa40b7bffd77378fd7aba6ca8bf106e7f581006320d266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:42:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 10:43:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:43:04 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 10:43:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 10:43:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 10:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 10:44:01 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 10:44:02 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 10:44:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 10:44:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 10:44:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f88dec7258b86e4e8c96100efc159399e0850fae2548f42d46fef4c3ae47f6`  
		Last Modified: Tue, 12 Jan 2021 10:44:33 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92eb800b9e7b936c989b77428553ebd597012e1fd451c62077a5b319c5c5381c`  
		Last Modified: Tue, 12 Jan 2021 10:44:32 GMT  
		Size: 1.8 MB (1839430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192c478305b485d2d6512913428673bf7ccb9da73b48f2fbde43de07bde0b00d`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 5.5 MB (5479951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1e5fcf0c5c7851002a65cbff0bc261cf64ef0cb1e856adf7f699ba5aa83b8`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a0ef96e7bb574336736be33888eadcff04b2105f2d98247d8083da825c65f`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:1ac2a48f4093de84e993dc766d9b9533116ef5b96143b8627502ec0e308d1748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39503719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc39787a552c5d318cef4a3487de1ac8f5ae4e07b32759ac6b13197a8739f99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 15:20:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 15:21:21 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:21:27 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 15:21:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 15:21:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 15:27:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 15:27:44 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 15:27:48 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 15:27:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 15:27:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 15:27:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee4568d92ca67ebb39b4c46eba2c4ae2f896e934c8070bdc0c481404018c390`  
		Last Modified: Tue, 12 Jan 2021 15:28:29 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f9ff8423f2713cccf087b1cdb69e12ccfb4c861cc0dc1214c443d3091e6eac`  
		Last Modified: Tue, 12 Jan 2021 15:28:30 GMT  
		Size: 2.2 MB (2225166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fdad5551173536a86727e4250b94e34355d83020147ceb5ec0f412518e20c4`  
		Last Modified: Tue, 12 Jan 2021 15:28:31 GMT  
		Size: 6.7 MB (6743500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e427569d726352f8287dd512ad5c9b0f1bd0f0ba9b2e8a9d5d9e18b12d48de`  
		Last Modified: Tue, 12 Jan 2021 15:28:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed1f874132ad81fab1ac2244587626a668c8a55413bb109d61fe8983f352624`  
		Last Modified: Tue, 12 Jan 2021 15:28:30 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:d25fc36058d984ef1de9c0061022bd803224e14c6b1a28073a97ac913f5b75e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33491139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be176b022a0a3121121756080606d3f10045f77c7c551fd766467beb596c525`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:22 GMT
ADD file:c01d899d503187f788db0a7d658bf3f2b6541026a4c654707d3272f6d3ffaf58 in / 
# Tue, 12 Jan 2021 00:42:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:54:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 02:54:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:54:11 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 02:54:12 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 02:54:12 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 02:54:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 02:54:39 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 02:54:39 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 02:54:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 02:54:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 02:54:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0e3e06c0bd0347fefe8bde60780e7e551c0cdf1cbcf40be3d052e823d5ec118`  
		Last Modified: Tue, 12 Jan 2021 00:52:32 GMT  
		Size: 25.7 MB (25723406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17512f7809b0e3dc11ab91a97504e20e1aece1b4d7ffd53c61541e59cefb02d`  
		Last Modified: Tue, 12 Jan 2021 02:55:27 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee602ea1b5f7a93780a8ee5fe5f394864b6475f785bc7125fd004e931b106eb`  
		Last Modified: Tue, 12 Jan 2021 02:55:30 GMT  
		Size: 1.8 MB (1822021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93d111b3adf8d1a2c9ad404a750c4c92fe5ee90b0b9d690dd130ce5bf970930`  
		Last Modified: Tue, 12 Jan 2021 02:55:28 GMT  
		Size: 5.9 MB (5943508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af24d5ea6121cd5d4a68c533f97899d07b55a3e356026c5a34d50ca9a7c64070`  
		Last Modified: Tue, 12 Jan 2021 02:55:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81b1a70da6be82ba066d625c23c7da6e01af6578e243e4dcd3c27baf189aba3`  
		Last Modified: Tue, 12 Jan 2021 02:55:31 GMT  
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
$ docker pull spiped@sha256:cde9e4f1555323e51360ff710044aee086cbdd898bfb0fedd6c40ae721ca7074
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
$ docker pull spiped@sha256:06d3a90eababe7a10ab3aca2c67daf41893a351802ba319beecfe9ed752483cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36276212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d92174c45b324b29b7e88abb4eb1684caf02874e5ac2d4f17c7216462a31f5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 19:04:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 19:04:56 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:04:56 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 19:04:57 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 19:04:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 19:05:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 19:05:36 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 19:05:36 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 19:05:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 19:05:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 19:05:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa6da2fcdba0615425a10a7476eacc596cf8e7eefa675a98f5bde79ced32cd8`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b22cf825b4fe47ca058426beb71cb3ff18273aee3e32bd89881912e726db5d`  
		Last Modified: Tue, 12 Jan 2021 19:06:03 GMT  
		Size: 2.1 MB (2128411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded296a693f0eb4b77e16db9ec7a4c9751ecb5f8a53ed59576352d9b9220c402`  
		Last Modified: Tue, 12 Jan 2021 19:06:05 GMT  
		Size: 7.0 MB (7037562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7940bfb150d14dbc1e6abd29a077b7c06321150e49c08097449ef62c6bc6724d`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467c5ffa5950fc15c6929703e9ae99c0a816cda85f18a52401b599dc0f8aa058`  
		Last Modified: Tue, 12 Jan 2021 19:06:02 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:5bd55a1a73670e68370f209d9dd01c217eb5b6c67598f25bac68f60e27549889
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32173489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811e01c7a839fa25b3fa40b7bffd77378fd7aba6ca8bf106e7f581006320d266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:42:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 10:43:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:43:04 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 10:43:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 10:43:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 10:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 10:44:01 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 10:44:02 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 10:44:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 10:44:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 10:44:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f88dec7258b86e4e8c96100efc159399e0850fae2548f42d46fef4c3ae47f6`  
		Last Modified: Tue, 12 Jan 2021 10:44:33 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92eb800b9e7b936c989b77428553ebd597012e1fd451c62077a5b319c5c5381c`  
		Last Modified: Tue, 12 Jan 2021 10:44:32 GMT  
		Size: 1.8 MB (1839430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192c478305b485d2d6512913428673bf7ccb9da73b48f2fbde43de07bde0b00d`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 5.5 MB (5479951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1e5fcf0c5c7851002a65cbff0bc261cf64ef0cb1e856adf7f699ba5aa83b8`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a0ef96e7bb574336736be33888eadcff04b2105f2d98247d8083da825c65f`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:1ac2a48f4093de84e993dc766d9b9533116ef5b96143b8627502ec0e308d1748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39503719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc39787a552c5d318cef4a3487de1ac8f5ae4e07b32759ac6b13197a8739f99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 15:20:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 15:21:21 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:21:27 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 15:21:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 15:21:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 15:27:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 15:27:44 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 15:27:48 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 15:27:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 15:27:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 15:27:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee4568d92ca67ebb39b4c46eba2c4ae2f896e934c8070bdc0c481404018c390`  
		Last Modified: Tue, 12 Jan 2021 15:28:29 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f9ff8423f2713cccf087b1cdb69e12ccfb4c861cc0dc1214c443d3091e6eac`  
		Last Modified: Tue, 12 Jan 2021 15:28:30 GMT  
		Size: 2.2 MB (2225166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fdad5551173536a86727e4250b94e34355d83020147ceb5ec0f412518e20c4`  
		Last Modified: Tue, 12 Jan 2021 15:28:31 GMT  
		Size: 6.7 MB (6743500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e427569d726352f8287dd512ad5c9b0f1bd0f0ba9b2e8a9d5d9e18b12d48de`  
		Last Modified: Tue, 12 Jan 2021 15:28:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed1f874132ad81fab1ac2244587626a668c8a55413bb109d61fe8983f352624`  
		Last Modified: Tue, 12 Jan 2021 15:28:30 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:d25fc36058d984ef1de9c0061022bd803224e14c6b1a28073a97ac913f5b75e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33491139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be176b022a0a3121121756080606d3f10045f77c7c551fd766467beb596c525`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:22 GMT
ADD file:c01d899d503187f788db0a7d658bf3f2b6541026a4c654707d3272f6d3ffaf58 in / 
# Tue, 12 Jan 2021 00:42:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:54:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 02:54:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:54:11 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 02:54:12 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 02:54:12 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 02:54:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 02:54:39 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 02:54:39 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 02:54:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 02:54:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 02:54:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0e3e06c0bd0347fefe8bde60780e7e551c0cdf1cbcf40be3d052e823d5ec118`  
		Last Modified: Tue, 12 Jan 2021 00:52:32 GMT  
		Size: 25.7 MB (25723406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17512f7809b0e3dc11ab91a97504e20e1aece1b4d7ffd53c61541e59cefb02d`  
		Last Modified: Tue, 12 Jan 2021 02:55:27 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee602ea1b5f7a93780a8ee5fe5f394864b6475f785bc7125fd004e931b106eb`  
		Last Modified: Tue, 12 Jan 2021 02:55:30 GMT  
		Size: 1.8 MB (1822021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93d111b3adf8d1a2c9ad404a750c4c92fe5ee90b0b9d690dd130ce5bf970930`  
		Last Modified: Tue, 12 Jan 2021 02:55:28 GMT  
		Size: 5.9 MB (5943508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af24d5ea6121cd5d4a68c533f97899d07b55a3e356026c5a34d50ca9a7c64070`  
		Last Modified: Tue, 12 Jan 2021 02:55:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81b1a70da6be82ba066d625c23c7da6e01af6578e243e4dcd3c27baf189aba3`  
		Last Modified: Tue, 12 Jan 2021 02:55:31 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
