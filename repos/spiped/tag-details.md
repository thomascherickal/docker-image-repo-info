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
$ docker pull spiped@sha256:5e2e850f6f530e9a0679dcf2041ca43f1309326c2a2e974eeb1fc461f1f714a6
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
$ docker pull spiped@sha256:70439d6dbe88f21aa856aaab7a7298438cc12ba3be7549ebd4420f806d307037
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5380b2b56cd6ec9efbd9d681f7e5bc0f685ddcae2e0e1ac3d3d091805925047d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 07:45:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Aug 2020 07:45:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 05 Aug 2020 07:45:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Aug 2020 07:45:42 GMT
VOLUME [/spiped]
# Wed, 05 Aug 2020 07:45:42 GMT
WORKDIR /spiped
# Wed, 05 Aug 2020 07:45:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Aug 2020 07:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Aug 2020 07:45:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb460858f95f33833e9855747ba0a53d32cf243e9954e4b4a93fcaf7a1050c`  
		Last Modified: Wed, 05 Aug 2020 07:45:59 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386f27b678cc082575d2ebea9a65f8283c777429d9b1bb236ca3616f656cd500`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 2.1 MB (2128098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e579e4436d85d2674a21e0f2ba66a749c8a8f532d966769790061dddd49e52b`  
		Last Modified: Wed, 05 Aug 2020 07:46:00 GMT  
		Size: 7.0 MB (7037434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a652d9418b3d88fef1c5affe9eb20fdf3d4ec7bd9a9820e69be93a1ab7e53f`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7067335ae1b8e78625cb1fe80b7848b2978cd642958bbda66f28298b3da12`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:0ffa7209cfe814b6558ab1e948cc440a965eb77f3af74f0e20e97e346d3b521f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d6fefca0c0605222f639cdc3d28477e5036c67425fb388f16b2d1d0f3bb3df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:49 GMT
ADD file:34835d84d87e3ee1178aa150793d75a4d4a7a28c013ca3495dbcca2b570270bf in / 
# Wed, 09 Sep 2020 23:53:53 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:24:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:24:31 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:24:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:24:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:24:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:25:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:25:32 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:25:34 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:25:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0a51b5143468e1b44dafa16fea3541e28e369071f6837337ee95e37f0ad81d99`  
		Last Modified: Thu, 10 Sep 2020 00:02:48 GMT  
		Size: 24.8 MB (24835974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16e60014503eeb6a9de0642540ffe398b65110a92e105ea725fe64050f133c7`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0bd36d1f55b67f92e906287f170c5ff225fa133082c4ac65bf0b026c8c1c61`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 1.8 MB (1839179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ddea53fb3a57a5e46a257e877538608b0b699eabf62195c6787df35c041c0`  
		Last Modified: Thu, 10 Sep 2020 00:26:00 GMT  
		Size: 5.5 MB (5479920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcc0f7c2e8d86cd9038ca26d518798de530b02f9d6a2625dea4fa37168eaf3f`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416e4e1edd36cc0942d8b1f16299321dcea276b757a77e44a69544b5f2716446`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3aacb61c327b386ee34f6b93b1fa0fd5374f619e4e2892eeb89bf106fedd68f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29746982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f0c17703a1231aa28de1d610bbe7c71e9c4359c858c6b17e874c5c0046df2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:05:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 23:05:39 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:05:40 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 23:05:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 23:05:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 23:06:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 23:06:42 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 23:06:46 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 23:06:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:06:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069f16da332ada6f1ad07545e36cc298d95cc8aa48b90b032fa05c40ade00eb1`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10508b92cc5c67114d8c737d41e90f8fb787bfcf5b323b188f73fdb862db6a00`  
		Last Modified: Tue, 04 Aug 2020 23:07:17 GMT  
		Size: 1.8 MB (1759470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fd1ca266440f3d238e6839e5219c41bab5dd0d88b8ddbdaa24f8e00cfcb5a0`  
		Last Modified: Tue, 04 Aug 2020 23:07:19 GMT  
		Size: 5.3 MB (5285516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea228d83d648f1c8eae77bf202795643d64ff1ae73be870802716fc868c03c80`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33943a537cfaba6127939b8cd88291a552d5f04b4d35e8a0b5c88662f3b14cf3`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b5559218e09ea14be189bc4849e65862923f193c32a411414000ab9ef9d78958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc4164d7a19420c2ade4b8da35eb1ee139c6222f7e1294f5fc19e5fcb9c210b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 15:37:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 15:37:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:37:13 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 15:37:13 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 15:37:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 15:38:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 15:38:04 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 15:38:05 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 15:38:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 15:38:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 15:38:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc32d378107720f326e540f83d46bf60a4bce7af8244906ed9526271eee31c3`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079ffe8630aa7835a3caef3a636edbb7a12d5ecddb5a60bfe8818de2559b2006`  
		Last Modified: Tue, 04 Aug 2020 15:38:39 GMT  
		Size: 2.0 MB (2007894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cd7433660d1423b7657db5c6d63e3a85c7d5f6f29c722623c496c5894962b2`  
		Last Modified: Tue, 04 Aug 2020 15:38:44 GMT  
		Size: 5.9 MB (5905348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d359b34f38b7c91489868441f4924bf12eb7ce4f499d08e9f6f27df6e1c315c8`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a9286120d5d507f14efb6bee85440a27254031d85a1aecd582401d1dd9adab`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:7705a0fc3f3476409ebb0bc24d6d37d7fba3e5592d82ee6d2839e364a950456e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989705c9829172d17a6ede941662c041e3cf4cac305a6d4b388b20e91453b1b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:16:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:16:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:17:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:17:11 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:17:11 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:17:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:17:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:17:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860dd30325c96ffc8b96efe07adbb91c1bf07d1fbe88c2cde7cecd89da76d72`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4331fe8000d00915ae0827ce99d7946202943c5616440cd4fe768d9d7ed71a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 2.1 MB (2132352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c89212a59a8a3b09219d62baf7cfc20311e828bbf52b010ae9db5bc78c5b83`  
		Last Modified: Thu, 10 Sep 2020 00:17:29 GMT  
		Size: 11.6 MB (11633000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54072dfa562a77a02b96e37ade7b47dfdf8a9a27d4eee6db49dc154a2c89cf0a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe5b51ab58e39aa04cbe7d1f927049252d4d7b476925effe2c5e213e905108`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:016da36b9f7998b09d92b6cc8852d341e82ef59a357e95663cf2a912e99bf1c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195c77f25ce68e53cef2621cd2de83604d84f91dc5bdcebf623cfc31ce8aa130`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:18:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 11:18:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 11:19:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 11:19:31 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 11:19:32 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 11:19:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d54e34357c9f5fa48267296e6c6c1f76e35953b78ff71274dbf93d620fe713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808939bfa0b439c22bc52e424703f683009d54bc7b0e929bb95642a17e4cf346`  
		Last Modified: Tue, 04 Aug 2020 11:19:57 GMT  
		Size: 1.7 MB (1712064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1430e0259ffd64f678312f8e44b2331f9b36c5dfc010756f03d0b4b1d5278b`  
		Last Modified: Tue, 04 Aug 2020 11:20:02 GMT  
		Size: 6.4 MB (6416279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160144f3a0adf67512994233d3b27e3cf11991c2929b9ceb5fcbccce56af823`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a1586309f94ae81d1d5501572c464e6cf0b95721f6d0e54fad359886abb713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:1a26f6d748b9c6cd0cd3c33bd6326198eac44ee6695d90e32fa92c33d0efab15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffa18892130ac57caaa0c35c5e223f1f80929f3bca5753dfbbebd98c9d1a1ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:44:13 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 12:44:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 12:44:36 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 12:44:39 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 12:44:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 12:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 12:48:05 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 12:48:08 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 12:48:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 12:48:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 12:48:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec976cf945c4c5a0725ce160b23b8fc7453ab53f7645cb507f81cc8f97ba1f`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b3868607138d28e33ab153c8f68521f00f2c00ee48d5542c62fef3ee508bcf`  
		Last Modified: Tue, 04 Aug 2020 12:48:52 GMT  
		Size: 2.2 MB (2224970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc4d03de8274dc06c34b37b24e819fe01a0d313e538a7a809f519e3a63d9418`  
		Last Modified: Tue, 04 Aug 2020 12:48:53 GMT  
		Size: 6.7 MB (6743232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff8e76a3ee77f253306f6c4c94eaf5df2e55c449d2a812c3bb843851031bc47`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58b79d7f675a5211c5c171567c5ff5762c0755bef406ed884efd50c9df4a3d1`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:3d77e561a1da58512f8944775139df6b4c0837d6f38a3f57a18522f0acc1824e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33474968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e3a3c55ec7ac4f5ce17bb3f14dc3268a611714368d8f3c15bdf715638359f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:42:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 01:42:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 01:43:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 01:43:02 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 01:43:03 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 01:43:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 01:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 01:43:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:07e4a6dbced6eed74bdb331987f95c00aa5b46543570b7adc1575121e66102dd`  
		Last Modified: Wed, 09 Sep 2020 23:46:28 GMT  
		Size: 25.7 MB (25707597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814983a66e3ee433d454db4a5b4e1062cf563e9decb8c477bba4cd96bc413ef1`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e1d72214ff5a65c75ec20c8756f56e1739f0aa5c8124641f55b46448070adf`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 1.8 MB (1821787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd27f6e5680762c3bf63ebc1825797061f461bd985220db2634dd60509dfcc7d`  
		Last Modified: Thu, 10 Sep 2020 01:43:20 GMT  
		Size: 5.9 MB (5943372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a566492192d8af2e7358649988f9e50908dbe4afa87c84c6fa890eb6235c6924`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd28ff600e747098b28280c12af1bfd52c57a500440f4376ba567e79defc6c`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:5e2e850f6f530e9a0679dcf2041ca43f1309326c2a2e974eeb1fc461f1f714a6
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
$ docker pull spiped@sha256:70439d6dbe88f21aa856aaab7a7298438cc12ba3be7549ebd4420f806d307037
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5380b2b56cd6ec9efbd9d681f7e5bc0f685ddcae2e0e1ac3d3d091805925047d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 07:45:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Aug 2020 07:45:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 05 Aug 2020 07:45:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Aug 2020 07:45:42 GMT
VOLUME [/spiped]
# Wed, 05 Aug 2020 07:45:42 GMT
WORKDIR /spiped
# Wed, 05 Aug 2020 07:45:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Aug 2020 07:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Aug 2020 07:45:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb460858f95f33833e9855747ba0a53d32cf243e9954e4b4a93fcaf7a1050c`  
		Last Modified: Wed, 05 Aug 2020 07:45:59 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386f27b678cc082575d2ebea9a65f8283c777429d9b1bb236ca3616f656cd500`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 2.1 MB (2128098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e579e4436d85d2674a21e0f2ba66a749c8a8f532d966769790061dddd49e52b`  
		Last Modified: Wed, 05 Aug 2020 07:46:00 GMT  
		Size: 7.0 MB (7037434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a652d9418b3d88fef1c5affe9eb20fdf3d4ec7bd9a9820e69be93a1ab7e53f`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7067335ae1b8e78625cb1fe80b7848b2978cd642958bbda66f28298b3da12`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:0ffa7209cfe814b6558ab1e948cc440a965eb77f3af74f0e20e97e346d3b521f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d6fefca0c0605222f639cdc3d28477e5036c67425fb388f16b2d1d0f3bb3df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:49 GMT
ADD file:34835d84d87e3ee1178aa150793d75a4d4a7a28c013ca3495dbcca2b570270bf in / 
# Wed, 09 Sep 2020 23:53:53 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:24:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:24:31 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:24:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:24:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:24:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:25:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:25:32 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:25:34 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:25:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0a51b5143468e1b44dafa16fea3541e28e369071f6837337ee95e37f0ad81d99`  
		Last Modified: Thu, 10 Sep 2020 00:02:48 GMT  
		Size: 24.8 MB (24835974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16e60014503eeb6a9de0642540ffe398b65110a92e105ea725fe64050f133c7`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0bd36d1f55b67f92e906287f170c5ff225fa133082c4ac65bf0b026c8c1c61`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 1.8 MB (1839179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ddea53fb3a57a5e46a257e877538608b0b699eabf62195c6787df35c041c0`  
		Last Modified: Thu, 10 Sep 2020 00:26:00 GMT  
		Size: 5.5 MB (5479920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcc0f7c2e8d86cd9038ca26d518798de530b02f9d6a2625dea4fa37168eaf3f`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416e4e1edd36cc0942d8b1f16299321dcea276b757a77e44a69544b5f2716446`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3aacb61c327b386ee34f6b93b1fa0fd5374f619e4e2892eeb89bf106fedd68f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29746982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f0c17703a1231aa28de1d610bbe7c71e9c4359c858c6b17e874c5c0046df2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:05:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 23:05:39 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:05:40 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 23:05:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 23:05:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 23:06:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 23:06:42 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 23:06:46 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 23:06:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:06:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069f16da332ada6f1ad07545e36cc298d95cc8aa48b90b032fa05c40ade00eb1`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10508b92cc5c67114d8c737d41e90f8fb787bfcf5b323b188f73fdb862db6a00`  
		Last Modified: Tue, 04 Aug 2020 23:07:17 GMT  
		Size: 1.8 MB (1759470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fd1ca266440f3d238e6839e5219c41bab5dd0d88b8ddbdaa24f8e00cfcb5a0`  
		Last Modified: Tue, 04 Aug 2020 23:07:19 GMT  
		Size: 5.3 MB (5285516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea228d83d648f1c8eae77bf202795643d64ff1ae73be870802716fc868c03c80`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33943a537cfaba6127939b8cd88291a552d5f04b4d35e8a0b5c88662f3b14cf3`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b5559218e09ea14be189bc4849e65862923f193c32a411414000ab9ef9d78958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc4164d7a19420c2ade4b8da35eb1ee139c6222f7e1294f5fc19e5fcb9c210b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 15:37:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 15:37:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:37:13 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 15:37:13 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 15:37:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 15:38:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 15:38:04 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 15:38:05 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 15:38:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 15:38:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 15:38:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc32d378107720f326e540f83d46bf60a4bce7af8244906ed9526271eee31c3`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079ffe8630aa7835a3caef3a636edbb7a12d5ecddb5a60bfe8818de2559b2006`  
		Last Modified: Tue, 04 Aug 2020 15:38:39 GMT  
		Size: 2.0 MB (2007894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cd7433660d1423b7657db5c6d63e3a85c7d5f6f29c722623c496c5894962b2`  
		Last Modified: Tue, 04 Aug 2020 15:38:44 GMT  
		Size: 5.9 MB (5905348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d359b34f38b7c91489868441f4924bf12eb7ce4f499d08e9f6f27df6e1c315c8`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a9286120d5d507f14efb6bee85440a27254031d85a1aecd582401d1dd9adab`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:7705a0fc3f3476409ebb0bc24d6d37d7fba3e5592d82ee6d2839e364a950456e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989705c9829172d17a6ede941662c041e3cf4cac305a6d4b388b20e91453b1b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:16:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:16:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:17:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:17:11 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:17:11 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:17:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:17:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:17:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860dd30325c96ffc8b96efe07adbb91c1bf07d1fbe88c2cde7cecd89da76d72`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4331fe8000d00915ae0827ce99d7946202943c5616440cd4fe768d9d7ed71a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 2.1 MB (2132352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c89212a59a8a3b09219d62baf7cfc20311e828bbf52b010ae9db5bc78c5b83`  
		Last Modified: Thu, 10 Sep 2020 00:17:29 GMT  
		Size: 11.6 MB (11633000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54072dfa562a77a02b96e37ade7b47dfdf8a9a27d4eee6db49dc154a2c89cf0a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe5b51ab58e39aa04cbe7d1f927049252d4d7b476925effe2c5e213e905108`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:016da36b9f7998b09d92b6cc8852d341e82ef59a357e95663cf2a912e99bf1c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195c77f25ce68e53cef2621cd2de83604d84f91dc5bdcebf623cfc31ce8aa130`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:18:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 11:18:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 11:19:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 11:19:31 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 11:19:32 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 11:19:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d54e34357c9f5fa48267296e6c6c1f76e35953b78ff71274dbf93d620fe713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808939bfa0b439c22bc52e424703f683009d54bc7b0e929bb95642a17e4cf346`  
		Last Modified: Tue, 04 Aug 2020 11:19:57 GMT  
		Size: 1.7 MB (1712064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1430e0259ffd64f678312f8e44b2331f9b36c5dfc010756f03d0b4b1d5278b`  
		Last Modified: Tue, 04 Aug 2020 11:20:02 GMT  
		Size: 6.4 MB (6416279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160144f3a0adf67512994233d3b27e3cf11991c2929b9ceb5fcbccce56af823`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a1586309f94ae81d1d5501572c464e6cf0b95721f6d0e54fad359886abb713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:1a26f6d748b9c6cd0cd3c33bd6326198eac44ee6695d90e32fa92c33d0efab15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffa18892130ac57caaa0c35c5e223f1f80929f3bca5753dfbbebd98c9d1a1ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:44:13 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 12:44:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 12:44:36 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 12:44:39 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 12:44:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 12:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 12:48:05 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 12:48:08 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 12:48:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 12:48:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 12:48:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec976cf945c4c5a0725ce160b23b8fc7453ab53f7645cb507f81cc8f97ba1f`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b3868607138d28e33ab153c8f68521f00f2c00ee48d5542c62fef3ee508bcf`  
		Last Modified: Tue, 04 Aug 2020 12:48:52 GMT  
		Size: 2.2 MB (2224970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc4d03de8274dc06c34b37b24e819fe01a0d313e538a7a809f519e3a63d9418`  
		Last Modified: Tue, 04 Aug 2020 12:48:53 GMT  
		Size: 6.7 MB (6743232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff8e76a3ee77f253306f6c4c94eaf5df2e55c449d2a812c3bb843851031bc47`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58b79d7f675a5211c5c171567c5ff5762c0755bef406ed884efd50c9df4a3d1`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:3d77e561a1da58512f8944775139df6b4c0837d6f38a3f57a18522f0acc1824e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33474968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e3a3c55ec7ac4f5ce17bb3f14dc3268a611714368d8f3c15bdf715638359f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:42:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 01:42:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 01:43:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 01:43:02 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 01:43:03 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 01:43:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 01:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 01:43:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:07e4a6dbced6eed74bdb331987f95c00aa5b46543570b7adc1575121e66102dd`  
		Last Modified: Wed, 09 Sep 2020 23:46:28 GMT  
		Size: 25.7 MB (25707597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814983a66e3ee433d454db4a5b4e1062cf563e9decb8c477bba4cd96bc413ef1`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e1d72214ff5a65c75ec20c8756f56e1739f0aa5c8124641f55b46448070adf`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 1.8 MB (1821787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd27f6e5680762c3bf63ebc1825797061f461bd985220db2634dd60509dfcc7d`  
		Last Modified: Thu, 10 Sep 2020 01:43:20 GMT  
		Size: 5.9 MB (5943372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a566492192d8af2e7358649988f9e50908dbe4afa87c84c6fa890eb6235c6924`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd28ff600e747098b28280c12af1bfd52c57a500440f4376ba567e79defc6c`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:5e2e850f6f530e9a0679dcf2041ca43f1309326c2a2e974eeb1fc461f1f714a6
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
$ docker pull spiped@sha256:70439d6dbe88f21aa856aaab7a7298438cc12ba3be7549ebd4420f806d307037
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5380b2b56cd6ec9efbd9d681f7e5bc0f685ddcae2e0e1ac3d3d091805925047d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 07:45:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Aug 2020 07:45:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 05 Aug 2020 07:45:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Aug 2020 07:45:42 GMT
VOLUME [/spiped]
# Wed, 05 Aug 2020 07:45:42 GMT
WORKDIR /spiped
# Wed, 05 Aug 2020 07:45:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Aug 2020 07:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Aug 2020 07:45:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb460858f95f33833e9855747ba0a53d32cf243e9954e4b4a93fcaf7a1050c`  
		Last Modified: Wed, 05 Aug 2020 07:45:59 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386f27b678cc082575d2ebea9a65f8283c777429d9b1bb236ca3616f656cd500`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 2.1 MB (2128098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e579e4436d85d2674a21e0f2ba66a749c8a8f532d966769790061dddd49e52b`  
		Last Modified: Wed, 05 Aug 2020 07:46:00 GMT  
		Size: 7.0 MB (7037434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a652d9418b3d88fef1c5affe9eb20fdf3d4ec7bd9a9820e69be93a1ab7e53f`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7067335ae1b8e78625cb1fe80b7848b2978cd642958bbda66f28298b3da12`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:0ffa7209cfe814b6558ab1e948cc440a965eb77f3af74f0e20e97e346d3b521f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d6fefca0c0605222f639cdc3d28477e5036c67425fb388f16b2d1d0f3bb3df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:49 GMT
ADD file:34835d84d87e3ee1178aa150793d75a4d4a7a28c013ca3495dbcca2b570270bf in / 
# Wed, 09 Sep 2020 23:53:53 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:24:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:24:31 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:24:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:24:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:24:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:25:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:25:32 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:25:34 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:25:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0a51b5143468e1b44dafa16fea3541e28e369071f6837337ee95e37f0ad81d99`  
		Last Modified: Thu, 10 Sep 2020 00:02:48 GMT  
		Size: 24.8 MB (24835974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16e60014503eeb6a9de0642540ffe398b65110a92e105ea725fe64050f133c7`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0bd36d1f55b67f92e906287f170c5ff225fa133082c4ac65bf0b026c8c1c61`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 1.8 MB (1839179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ddea53fb3a57a5e46a257e877538608b0b699eabf62195c6787df35c041c0`  
		Last Modified: Thu, 10 Sep 2020 00:26:00 GMT  
		Size: 5.5 MB (5479920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcc0f7c2e8d86cd9038ca26d518798de530b02f9d6a2625dea4fa37168eaf3f`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416e4e1edd36cc0942d8b1f16299321dcea276b757a77e44a69544b5f2716446`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3aacb61c327b386ee34f6b93b1fa0fd5374f619e4e2892eeb89bf106fedd68f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29746982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f0c17703a1231aa28de1d610bbe7c71e9c4359c858c6b17e874c5c0046df2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:05:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 23:05:39 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:05:40 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 23:05:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 23:05:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 23:06:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 23:06:42 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 23:06:46 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 23:06:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:06:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069f16da332ada6f1ad07545e36cc298d95cc8aa48b90b032fa05c40ade00eb1`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10508b92cc5c67114d8c737d41e90f8fb787bfcf5b323b188f73fdb862db6a00`  
		Last Modified: Tue, 04 Aug 2020 23:07:17 GMT  
		Size: 1.8 MB (1759470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fd1ca266440f3d238e6839e5219c41bab5dd0d88b8ddbdaa24f8e00cfcb5a0`  
		Last Modified: Tue, 04 Aug 2020 23:07:19 GMT  
		Size: 5.3 MB (5285516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea228d83d648f1c8eae77bf202795643d64ff1ae73be870802716fc868c03c80`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33943a537cfaba6127939b8cd88291a552d5f04b4d35e8a0b5c88662f3b14cf3`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b5559218e09ea14be189bc4849e65862923f193c32a411414000ab9ef9d78958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc4164d7a19420c2ade4b8da35eb1ee139c6222f7e1294f5fc19e5fcb9c210b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 15:37:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 15:37:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:37:13 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 15:37:13 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 15:37:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 15:38:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 15:38:04 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 15:38:05 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 15:38:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 15:38:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 15:38:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc32d378107720f326e540f83d46bf60a4bce7af8244906ed9526271eee31c3`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079ffe8630aa7835a3caef3a636edbb7a12d5ecddb5a60bfe8818de2559b2006`  
		Last Modified: Tue, 04 Aug 2020 15:38:39 GMT  
		Size: 2.0 MB (2007894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cd7433660d1423b7657db5c6d63e3a85c7d5f6f29c722623c496c5894962b2`  
		Last Modified: Tue, 04 Aug 2020 15:38:44 GMT  
		Size: 5.9 MB (5905348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d359b34f38b7c91489868441f4924bf12eb7ce4f499d08e9f6f27df6e1c315c8`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a9286120d5d507f14efb6bee85440a27254031d85a1aecd582401d1dd9adab`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:7705a0fc3f3476409ebb0bc24d6d37d7fba3e5592d82ee6d2839e364a950456e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989705c9829172d17a6ede941662c041e3cf4cac305a6d4b388b20e91453b1b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:16:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:16:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:17:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:17:11 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:17:11 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:17:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:17:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:17:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860dd30325c96ffc8b96efe07adbb91c1bf07d1fbe88c2cde7cecd89da76d72`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4331fe8000d00915ae0827ce99d7946202943c5616440cd4fe768d9d7ed71a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 2.1 MB (2132352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c89212a59a8a3b09219d62baf7cfc20311e828bbf52b010ae9db5bc78c5b83`  
		Last Modified: Thu, 10 Sep 2020 00:17:29 GMT  
		Size: 11.6 MB (11633000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54072dfa562a77a02b96e37ade7b47dfdf8a9a27d4eee6db49dc154a2c89cf0a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe5b51ab58e39aa04cbe7d1f927049252d4d7b476925effe2c5e213e905108`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:016da36b9f7998b09d92b6cc8852d341e82ef59a357e95663cf2a912e99bf1c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195c77f25ce68e53cef2621cd2de83604d84f91dc5bdcebf623cfc31ce8aa130`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:18:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 11:18:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 11:19:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 11:19:31 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 11:19:32 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 11:19:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d54e34357c9f5fa48267296e6c6c1f76e35953b78ff71274dbf93d620fe713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808939bfa0b439c22bc52e424703f683009d54bc7b0e929bb95642a17e4cf346`  
		Last Modified: Tue, 04 Aug 2020 11:19:57 GMT  
		Size: 1.7 MB (1712064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1430e0259ffd64f678312f8e44b2331f9b36c5dfc010756f03d0b4b1d5278b`  
		Last Modified: Tue, 04 Aug 2020 11:20:02 GMT  
		Size: 6.4 MB (6416279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160144f3a0adf67512994233d3b27e3cf11991c2929b9ceb5fcbccce56af823`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a1586309f94ae81d1d5501572c464e6cf0b95721f6d0e54fad359886abb713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:1a26f6d748b9c6cd0cd3c33bd6326198eac44ee6695d90e32fa92c33d0efab15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffa18892130ac57caaa0c35c5e223f1f80929f3bca5753dfbbebd98c9d1a1ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:44:13 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 12:44:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 12:44:36 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 12:44:39 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 12:44:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 12:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 12:48:05 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 12:48:08 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 12:48:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 12:48:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 12:48:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec976cf945c4c5a0725ce160b23b8fc7453ab53f7645cb507f81cc8f97ba1f`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b3868607138d28e33ab153c8f68521f00f2c00ee48d5542c62fef3ee508bcf`  
		Last Modified: Tue, 04 Aug 2020 12:48:52 GMT  
		Size: 2.2 MB (2224970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc4d03de8274dc06c34b37b24e819fe01a0d313e538a7a809f519e3a63d9418`  
		Last Modified: Tue, 04 Aug 2020 12:48:53 GMT  
		Size: 6.7 MB (6743232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff8e76a3ee77f253306f6c4c94eaf5df2e55c449d2a812c3bb843851031bc47`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58b79d7f675a5211c5c171567c5ff5762c0755bef406ed884efd50c9df4a3d1`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:3d77e561a1da58512f8944775139df6b4c0837d6f38a3f57a18522f0acc1824e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33474968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e3a3c55ec7ac4f5ce17bb3f14dc3268a611714368d8f3c15bdf715638359f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:42:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 01:42:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 01:43:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 01:43:02 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 01:43:03 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 01:43:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 01:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 01:43:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:07e4a6dbced6eed74bdb331987f95c00aa5b46543570b7adc1575121e66102dd`  
		Last Modified: Wed, 09 Sep 2020 23:46:28 GMT  
		Size: 25.7 MB (25707597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814983a66e3ee433d454db4a5b4e1062cf563e9decb8c477bba4cd96bc413ef1`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e1d72214ff5a65c75ec20c8756f56e1739f0aa5c8124641f55b46448070adf`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 1.8 MB (1821787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd27f6e5680762c3bf63ebc1825797061f461bd985220db2634dd60509dfcc7d`  
		Last Modified: Thu, 10 Sep 2020 01:43:20 GMT  
		Size: 5.9 MB (5943372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a566492192d8af2e7358649988f9e50908dbe4afa87c84c6fa890eb6235c6924`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd28ff600e747098b28280c12af1bfd52c57a500440f4376ba567e79defc6c`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:5e2e850f6f530e9a0679dcf2041ca43f1309326c2a2e974eeb1fc461f1f714a6
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
$ docker pull spiped@sha256:70439d6dbe88f21aa856aaab7a7298438cc12ba3be7549ebd4420f806d307037
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5380b2b56cd6ec9efbd9d681f7e5bc0f685ddcae2e0e1ac3d3d091805925047d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 07:45:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Aug 2020 07:45:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 05 Aug 2020 07:45:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Aug 2020 07:45:42 GMT
VOLUME [/spiped]
# Wed, 05 Aug 2020 07:45:42 GMT
WORKDIR /spiped
# Wed, 05 Aug 2020 07:45:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Aug 2020 07:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Aug 2020 07:45:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb460858f95f33833e9855747ba0a53d32cf243e9954e4b4a93fcaf7a1050c`  
		Last Modified: Wed, 05 Aug 2020 07:45:59 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386f27b678cc082575d2ebea9a65f8283c777429d9b1bb236ca3616f656cd500`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 2.1 MB (2128098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e579e4436d85d2674a21e0f2ba66a749c8a8f532d966769790061dddd49e52b`  
		Last Modified: Wed, 05 Aug 2020 07:46:00 GMT  
		Size: 7.0 MB (7037434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a652d9418b3d88fef1c5affe9eb20fdf3d4ec7bd9a9820e69be93a1ab7e53f`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7067335ae1b8e78625cb1fe80b7848b2978cd642958bbda66f28298b3da12`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:0ffa7209cfe814b6558ab1e948cc440a965eb77f3af74f0e20e97e346d3b521f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d6fefca0c0605222f639cdc3d28477e5036c67425fb388f16b2d1d0f3bb3df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:49 GMT
ADD file:34835d84d87e3ee1178aa150793d75a4d4a7a28c013ca3495dbcca2b570270bf in / 
# Wed, 09 Sep 2020 23:53:53 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:24:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:24:31 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:24:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:24:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:24:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:25:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:25:32 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:25:34 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:25:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0a51b5143468e1b44dafa16fea3541e28e369071f6837337ee95e37f0ad81d99`  
		Last Modified: Thu, 10 Sep 2020 00:02:48 GMT  
		Size: 24.8 MB (24835974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16e60014503eeb6a9de0642540ffe398b65110a92e105ea725fe64050f133c7`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0bd36d1f55b67f92e906287f170c5ff225fa133082c4ac65bf0b026c8c1c61`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 1.8 MB (1839179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ddea53fb3a57a5e46a257e877538608b0b699eabf62195c6787df35c041c0`  
		Last Modified: Thu, 10 Sep 2020 00:26:00 GMT  
		Size: 5.5 MB (5479920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcc0f7c2e8d86cd9038ca26d518798de530b02f9d6a2625dea4fa37168eaf3f`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416e4e1edd36cc0942d8b1f16299321dcea276b757a77e44a69544b5f2716446`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3aacb61c327b386ee34f6b93b1fa0fd5374f619e4e2892eeb89bf106fedd68f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29746982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f0c17703a1231aa28de1d610bbe7c71e9c4359c858c6b17e874c5c0046df2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:05:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 23:05:39 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:05:40 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 23:05:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 23:05:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 23:06:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 23:06:42 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 23:06:46 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 23:06:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:06:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069f16da332ada6f1ad07545e36cc298d95cc8aa48b90b032fa05c40ade00eb1`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10508b92cc5c67114d8c737d41e90f8fb787bfcf5b323b188f73fdb862db6a00`  
		Last Modified: Tue, 04 Aug 2020 23:07:17 GMT  
		Size: 1.8 MB (1759470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fd1ca266440f3d238e6839e5219c41bab5dd0d88b8ddbdaa24f8e00cfcb5a0`  
		Last Modified: Tue, 04 Aug 2020 23:07:19 GMT  
		Size: 5.3 MB (5285516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea228d83d648f1c8eae77bf202795643d64ff1ae73be870802716fc868c03c80`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33943a537cfaba6127939b8cd88291a552d5f04b4d35e8a0b5c88662f3b14cf3`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b5559218e09ea14be189bc4849e65862923f193c32a411414000ab9ef9d78958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc4164d7a19420c2ade4b8da35eb1ee139c6222f7e1294f5fc19e5fcb9c210b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 15:37:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 15:37:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:37:13 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 15:37:13 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 15:37:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 15:38:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 15:38:04 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 15:38:05 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 15:38:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 15:38:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 15:38:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc32d378107720f326e540f83d46bf60a4bce7af8244906ed9526271eee31c3`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079ffe8630aa7835a3caef3a636edbb7a12d5ecddb5a60bfe8818de2559b2006`  
		Last Modified: Tue, 04 Aug 2020 15:38:39 GMT  
		Size: 2.0 MB (2007894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cd7433660d1423b7657db5c6d63e3a85c7d5f6f29c722623c496c5894962b2`  
		Last Modified: Tue, 04 Aug 2020 15:38:44 GMT  
		Size: 5.9 MB (5905348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d359b34f38b7c91489868441f4924bf12eb7ce4f499d08e9f6f27df6e1c315c8`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a9286120d5d507f14efb6bee85440a27254031d85a1aecd582401d1dd9adab`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:7705a0fc3f3476409ebb0bc24d6d37d7fba3e5592d82ee6d2839e364a950456e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989705c9829172d17a6ede941662c041e3cf4cac305a6d4b388b20e91453b1b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:16:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:16:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:17:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:17:11 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:17:11 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:17:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:17:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:17:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860dd30325c96ffc8b96efe07adbb91c1bf07d1fbe88c2cde7cecd89da76d72`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4331fe8000d00915ae0827ce99d7946202943c5616440cd4fe768d9d7ed71a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 2.1 MB (2132352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c89212a59a8a3b09219d62baf7cfc20311e828bbf52b010ae9db5bc78c5b83`  
		Last Modified: Thu, 10 Sep 2020 00:17:29 GMT  
		Size: 11.6 MB (11633000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54072dfa562a77a02b96e37ade7b47dfdf8a9a27d4eee6db49dc154a2c89cf0a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe5b51ab58e39aa04cbe7d1f927049252d4d7b476925effe2c5e213e905108`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:016da36b9f7998b09d92b6cc8852d341e82ef59a357e95663cf2a912e99bf1c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195c77f25ce68e53cef2621cd2de83604d84f91dc5bdcebf623cfc31ce8aa130`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:18:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 11:18:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 11:19:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 11:19:31 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 11:19:32 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 11:19:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d54e34357c9f5fa48267296e6c6c1f76e35953b78ff71274dbf93d620fe713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808939bfa0b439c22bc52e424703f683009d54bc7b0e929bb95642a17e4cf346`  
		Last Modified: Tue, 04 Aug 2020 11:19:57 GMT  
		Size: 1.7 MB (1712064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1430e0259ffd64f678312f8e44b2331f9b36c5dfc010756f03d0b4b1d5278b`  
		Last Modified: Tue, 04 Aug 2020 11:20:02 GMT  
		Size: 6.4 MB (6416279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160144f3a0adf67512994233d3b27e3cf11991c2929b9ceb5fcbccce56af823`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a1586309f94ae81d1d5501572c464e6cf0b95721f6d0e54fad359886abb713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:1a26f6d748b9c6cd0cd3c33bd6326198eac44ee6695d90e32fa92c33d0efab15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffa18892130ac57caaa0c35c5e223f1f80929f3bca5753dfbbebd98c9d1a1ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:44:13 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 12:44:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 12:44:36 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 12:44:39 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 12:44:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 12:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 12:48:05 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 12:48:08 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 12:48:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 12:48:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 12:48:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec976cf945c4c5a0725ce160b23b8fc7453ab53f7645cb507f81cc8f97ba1f`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b3868607138d28e33ab153c8f68521f00f2c00ee48d5542c62fef3ee508bcf`  
		Last Modified: Tue, 04 Aug 2020 12:48:52 GMT  
		Size: 2.2 MB (2224970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc4d03de8274dc06c34b37b24e819fe01a0d313e538a7a809f519e3a63d9418`  
		Last Modified: Tue, 04 Aug 2020 12:48:53 GMT  
		Size: 6.7 MB (6743232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff8e76a3ee77f253306f6c4c94eaf5df2e55c449d2a812c3bb843851031bc47`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58b79d7f675a5211c5c171567c5ff5762c0755bef406ed884efd50c9df4a3d1`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:3d77e561a1da58512f8944775139df6b4c0837d6f38a3f57a18522f0acc1824e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33474968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e3a3c55ec7ac4f5ce17bb3f14dc3268a611714368d8f3c15bdf715638359f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:42:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 01:42:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 01:43:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 01:43:02 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 01:43:03 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 01:43:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 01:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 01:43:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:07e4a6dbced6eed74bdb331987f95c00aa5b46543570b7adc1575121e66102dd`  
		Last Modified: Wed, 09 Sep 2020 23:46:28 GMT  
		Size: 25.7 MB (25707597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814983a66e3ee433d454db4a5b4e1062cf563e9decb8c477bba4cd96bc413ef1`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e1d72214ff5a65c75ec20c8756f56e1739f0aa5c8124641f55b46448070adf`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 1.8 MB (1821787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd27f6e5680762c3bf63ebc1825797061f461bd985220db2634dd60509dfcc7d`  
		Last Modified: Thu, 10 Sep 2020 01:43:20 GMT  
		Size: 5.9 MB (5943372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a566492192d8af2e7358649988f9e50908dbe4afa87c84c6fa890eb6235c6924`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd28ff600e747098b28280c12af1bfd52c57a500440f4376ba567e79defc6c`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
