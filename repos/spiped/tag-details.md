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
$ docker pull spiped@sha256:94da41acd9830f0839fe9cef81671adca1226272fa6da884c0a38ceaf9e9d943
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
$ docker pull spiped@sha256:7343758d9507624e239aaabd2c41388ea95ad4518b908ee90e466051119474ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42233860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d70d5061814f8d6b3f407f4606b44a9113ffaa5c5ee5bf65338718258df71877`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:19 GMT
ADD file:85c9e03c1d9121ebda028664176bf97f6e7a92eeea16af33bce6c2f6a1c4cb02 in / 
# Thu, 22 Jul 2021 00:45:19 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:41:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:41:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:41:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 17:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 17:41:54 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 17:41:55 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 17:41:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 17:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 17:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3ac06a45bc97f56a7ff01e34ad67b7ae7cb0bd2823542469d32bd69a1e5605e8`  
		Last Modified: Thu, 22 Jul 2021 00:49:49 GMT  
		Size: 31.4 MB (31355625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e190b64c0a941ff33122d59fcc9ca9c4bcbb12700f79cf2f78b5f5e5fab46c20`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b1ed4c69a01d247d265d16062afe1cd7e60557acc1b28fb86aba224e4f4cbb`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494e50df394c3910430e8505f9168527ac826dfa0527886f037b0a231c1677a2`  
		Last Modified: Mon, 16 Aug 2021 17:42:16 GMT  
		Size: 10.9 MB (10874973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8dbe476943b4eb81bf8428b43ad621f36c2ef1be3d0ecbdfeee489df2dbe9a`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8b322c0318160c75c2934bd723ebeb554cc62986a6a4393f0024107083dd7`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:61c15542f1bea87abd48bd3bf833da795a972cf790d4090ea55a6d290bad9c5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37955318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90f879e23779f5103c9fd072d33cb1d4b7e3917b6215bb83a2583537083c7dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:49:09 GMT
ADD file:19091df04c177de355e46137382ab24c0e316a9b4c2e139412ba581a0a18d1e1 in / 
# Thu, 22 Jul 2021 00:49:10 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 00:35:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 00:36:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 00:36:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 00:37:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 00:37:18 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 00:37:18 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 00:37:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 00:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 00:37:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0a1ff7527eb0e8de8a2887d94706915f958c570e660834bd28859b3960dfb63`  
		Last Modified: Thu, 22 Jul 2021 01:00:40 GMT  
		Size: 28.9 MB (28897022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c6a58e7c1e3b68268e686bf0343778937c559d986a842393f8c806a7b34c60`  
		Last Modified: Tue, 17 Aug 2021 00:37:53 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602dfd2e4e096b5fecaa80c0afe9f091248cc80db9faebcf4100c8ad7af8b66e`  
		Last Modified: Tue, 17 Aug 2021 00:37:53 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01e2c8fef9a743fb0e87a421e68eeb5d4193eafd2ddb5bc2d70cf50c9286406`  
		Last Modified: Tue, 17 Aug 2021 00:37:59 GMT  
		Size: 9.1 MB (9055037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4368a9c4fa462485f558d66b0ccc608abe9f207ed1c41ca67cdea3ac5c5bad`  
		Last Modified: Tue, 17 Aug 2021 00:37:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ad6b637824049b38a29d44e4ae702d3a67291db446652c10eb6ccc0741b47d`  
		Last Modified: Tue, 17 Aug 2021 00:37:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:602580d76c8e4de59befe6d3ffe34ace025b139a98799b4ab1b90c1e98d89265
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35115909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1753eeba61a486635abe267f9ad9f46edf7f54f190e49e06dbe9af598d8b92a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 02:02:47 GMT
ADD file:619a96435fb34ae415b7d8a447084f69a98366932e39c923941062bf09d73669 in / 
# Thu, 22 Jul 2021 02:02:48 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 00:43:01 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 00:43:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 00:43:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 00:44:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 00:44:12 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 00:44:13 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 00:44:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 00:44:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 00:44:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05bef09f82badb5e62c3bbcef85c8dff06a3270383173eb2906ed5541afbccc7`  
		Last Modified: Thu, 22 Jul 2021 02:14:54 GMT  
		Size: 26.6 MB (26559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06612b931c442de7e15ef227e99e1847d12bebabe0b54f96ca06ad0e63be9c0a`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aced7073612d1c2891301f8d2f5301f3ee9ef5180f3556aecd81a3919117cc`  
		Last Modified: Tue, 17 Aug 2021 00:45:19 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf204f2ca25c4cbd38de83228b3c595f681de4e2e0507e3e6c5d0efb842935`  
		Last Modified: Tue, 17 Aug 2021 00:45:25 GMT  
		Size: 8.6 MB (8553224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c33c91768fafd84f55b3fde36321612c24acdd00db9f0b1b7ba4aaa3a677cb9`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac6a1d40c98cce7a8a51740c2a289617146bbf2bc20161fa8e6e732fe6284e8`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
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
$ docker pull spiped@sha256:d3dd642f96becc516fb8a62318cd8a362a4402f1a8d82ee935a2954c670b968b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44762249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c5114d4e9a40f9df3298e5dbd3ceea3fd51dee675454b9f0aaba00eb679108`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:20 GMT
ADD file:7ca10cf9ec4ee7b61d4386a7797bbaa321cfff2a193f3834a78241e8674a2780 in / 
# Thu, 22 Jul 2021 00:39:20 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 16:38:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 16:39:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 16:39:01 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 16:39:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 16:39:32 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 16:39:32 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 16:39:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 16:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 16:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0a65268b957466841a0a37aa90035698fb76f15266e0baa350a093adb365ade6`  
		Last Modified: Thu, 22 Jul 2021 00:45:36 GMT  
		Size: 32.4 MB (32369313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb5ffc7bfeb22c3800b48e46c4bc03f33fea8109f52d44c22beec48e4a73d34`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd8452f42d0e0ed8e1a1ed6f8a02abf7138f2432dd06c2e9e4b9f4ba1627cd`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6499ccb36a18222e115fb8fa1e6e4d7f7d0c15a4bc07ef4ca72a88b00814a5e`  
		Last Modified: Mon, 16 Aug 2021 16:40:08 GMT  
		Size: 12.4 MB (12389675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd0b6e8e7624e147bc0aeeb4670850146880b335192adf9bfbfb35bb3eebb95`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88234b5b88b75b2e870ae1172bd4d6cbb02693e4dad0936ba9377c190860628f`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:1397de7ec9c127fa0852f12d7db9d76a690751fc21aa3c7adec345e0feef80e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39610648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b00d535f71e3926a86c308676925d0c7f6877d8b16062ab02e1444691bc7e8c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:08:58 GMT
ADD file:f1ef9d6eb38d477987532d95d608bc6d1127338387a50511169a91a11d284165 in / 
# Thu, 22 Jul 2021 00:08:58 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:08:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:09:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:09:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 17:10:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 17:10:32 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 17:10:32 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 17:10:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 17:10:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 17:10:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afeffcc83d23f7cc9022cb5ed0daac395407e585382b2889b160fb5c74e29485`  
		Last Modified: Thu, 22 Jul 2021 00:14:45 GMT  
		Size: 29.6 MB (29613402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f721acf9d11173e6aa3db0a45792ff954d8d6c5f381dd2808bae2cbe04967dc2`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784b7cb17c82bda53b2c459bf16b58c817ee954bfbbad39153e287cb17b277e6`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbec7c5c450a243dfb69ea49297c872d49ab220bfdf0ac9684a13d213944a3f`  
		Last Modified: Mon, 16 Aug 2021 17:11:06 GMT  
		Size: 10.0 MB (9994042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23eb944c6425598422492c0d1d2822fed3ba14ea2b4a643569d378f3ed99f7b1`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aeb292bdeb7661176ec0222602d00d8efba1f7f0d8b32ef24f7b49c9f9ce270`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:81e8760a45700aeccd739da2eb620ad6d31d246b398d6e5fc29568ce470ecacc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47012081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9452d89ef58183c25a133ee3196c58ebc6aa4f38da5c40764ad5be068b8246c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:17:53 GMT
ADD file:9d09cde9d8a95f1b791e4ef04a38d0e4df5c3705b2cb1fa0a1bfc71257fdab65 in / 
# Thu, 22 Jul 2021 00:18:02 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:58:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:58:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:58:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 18:06:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 18:07:03 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 18:07:15 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 18:07:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 18:07:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 18:07:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ea427ff41c744dd614b4a3c50a2c46429cf10eb87fd0bb2e2ac3e1dc4eb4d4a`  
		Last Modified: Thu, 22 Jul 2021 00:26:50 GMT  
		Size: 35.3 MB (35257797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30da9503b53aa23f533f4695a0542dd872e0aa6d5cdc3f394e885314791f745f`  
		Last Modified: Mon, 16 Aug 2021 18:08:11 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828794291318f59cfcf0a088b13d5d901cc49862fcccc66274da4e88d82eb1f`  
		Last Modified: Mon, 16 Aug 2021 18:08:11 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8f1699fb6e755f427535d5cf30286c55c7eb9cb2be984e4e49d50c9a219dd1`  
		Last Modified: Mon, 16 Aug 2021 18:08:13 GMT  
		Size: 11.8 MB (11751005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27bf8ac594a209b045a0a26d6ba9d334b17ff2aedb7162e7f7ce641fd9403ce`  
		Last Modified: Mon, 16 Aug 2021 18:08:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d13542ac8cb520531ca2742045af4f850ccf28d4106d88d56714c18821bbb47`  
		Last Modified: Mon, 16 Aug 2021 18:08:10 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:e7dbba32f20064755cf05c473ae6e9b44a3eea8a6cd5e81fdc51e22bc6028fd4
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
$ docker pull spiped@sha256:81959987e9809ba3bedbd6901a88e9fe28f2b16377bc8d3e43604661d48c2d15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3034576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d417cc665c58c81ae417555e8357d1f37bf78df7aaf23da4dcc13659df5a95a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:25:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 22:25:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 22:25:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 22:26:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 22:26:12 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 22:26:13 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 22:26:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:26:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 22:26:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9c880241f8602d0cc47e4fabf713180b354b6d9819786e78aaf3a9665b7767`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bccb485a15a7ccb6581c8d02974f14fd68b58810d648f7295647a532772b0`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 7.3 KB (7279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7741dee13e8d6c91732585334d7cef9f489ff0ba3dda16074f7cf05e58ed528a`  
		Last Modified: Fri, 06 Aug 2021 22:26:33 GMT  
		Size: 212.6 KB (212550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0337b646a0031aa1e94edce7b03cdab87816253a6850b30bf5fcfe39128e09`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc226b22f034d312b242c20826de8afa099040078d13d904d45dfeb771850e6`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:5106236450e3abdcba7735635894ff0393e5f0ce938d3fab894ece612e116c92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2837884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cdb6952199964783a11e1091cc96fa94684fd9e645edcea0376c4fef959217`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 23:52:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 23:52:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 23:52:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 23:53:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 23:53:27 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 23:53:28 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 23:53:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 23:53:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2adf0d4d8cc8b9e29d8414cae24c000412da47df5cb21a2a05ddf2e10dce570`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33562af158cbe4a36f2391938531bae4126685733de295b7ed766183da4b65ef`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23d92f94fd24201f1627f9cdbd4e09c0eced2bcbb6ebf6edd1cd206d43e2989`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 202.5 KB (202496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e821b43798aa5a90978114728243266a0f589a4f572c8034852cb0d17ce7c803`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ba2a665cda34f66fc655e2d76ea1f17e791687438e3675a6ca88c09fa438d`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b39dd207a36df0ab651368a23dd5f7fb85cb40c73169a18ed6a650c9e1e9fc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2634162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80c87f5ffe5257a7577c370989dbed14396b7ee0a5768d7e330b488935c5205`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:50:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 19:50:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 19:50:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 19:51:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 19:51:30 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 19:51:31 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 19:51:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 19:51:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d7a90d848ed25f9597b7555466d565e3c10725a9f17b4863bb5543b964fbef`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56efc9f5e430a2d91ff87e40f30089c0015233688200b25c6c645b9c75917480`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7705d09d2948f05566c3ad4b7184193f719c33fb432e05f9e9d134e1850c51f2`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 195.8 KB (195768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576177e1db2fc775ca441543afa32e5f65ec818813bbb783b5cfea5edcb0da7d`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd82adbb730f7bc7d4c11d373678c8f08c809f2f46e9cd79ae1f11169ec1f8b`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:11f573b8237bb1841a7175c9c9b77f7b8c680623ab91182c3b15186ce6d0a684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11d2305d4144c6a7caf39b8b6ca94a94d25dce28a8b4d51cbf4904172d0d3d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:20:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:20:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:20:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:20:46 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:20:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:20:47 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:20:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:20:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0faf3295f84c6343ed4bedec1bceca8f73e65a202fab2dde2578d5032f0264`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909cb3a09ec0e0c7512a5e0803fb90d9fa40a1331ebd44ac5923e377ef619c88`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 7.3 KB (7293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73e2091b0f5e799ac0526b25f8ee65662172dccf092bfcebac9a4f451801e2`  
		Last Modified: Sat, 07 Aug 2021 01:21:19 GMT  
		Size: 204.6 KB (204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3f2992d2b842a28dfa27d50163a579400dcff25c9326252f55415706303af`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac232dfb34c3889ce2beb5d4442d4a3b927e0ece42f3ab8a81de9779d579cba`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:f99c513faad87e225c2e474c95f7ceace240bcfdc0f161e74943db703f489f36
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3054380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355bc30b5b850a5b153236ee5157aa164f2754488c4565a7142fb520abe22f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 17:57:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 17:57:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 17:57:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 17:58:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 17:58:08 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 17:58:08 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 17:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 17:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 17:58:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9f8235dc8f7a2cb2e106af5945d974007f182ef18717b1358dc418b51672e7`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c8e66016715cac7eea56fb6278759a154b998e9cc867cfd9e699f45749f938`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 7.3 KB (7288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b143265a7e8e4e62818a693cb546d0cdbedb96dac486cdfaa3326b27c5669`  
		Last Modified: Fri, 06 Aug 2021 17:58:43 GMT  
		Size: 223.4 KB (223442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac32f75f64f9f329d462d69b46dad0bde0e7c7356333e99089593e3e0359d85`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d678fb9c378cbc3489d13a25fa17ca3d91d2319e6ffef53f6f84101025d21`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:fb4e68d177bc77f575c1a12ed21a941cb1ac2e423be4e1231ec7f327802e88a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3041425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8692281a7b48476e4611c785ef1f090697d8d28d64eca5cd85eabdf3842f44aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:30:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:31:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:31:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:31:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:31:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:31:54 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:31:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:32:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:32:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e1daa083c0d4e8922acb4a3735a2446ec516ebedf8992b97d0d8ac09474f9e`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ab775043317669024edb01d89328f75341409396938066bd82d18bcfa0f1b6`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9821113c32743f01e0620003d0630b6021c4148138f74add3efc51d82916a`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 221.2 KB (221239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2760cfc3e6b029ffb984aafe5b489eac1b215d0fe413a43cd00255dac46393`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b6d8de58c0e97f9000849b6c5be64af02ae4149134d50dedcb8e40e121b5e2`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:94da41acd9830f0839fe9cef81671adca1226272fa6da884c0a38ceaf9e9d943
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
$ docker pull spiped@sha256:7343758d9507624e239aaabd2c41388ea95ad4518b908ee90e466051119474ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42233860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d70d5061814f8d6b3f407f4606b44a9113ffaa5c5ee5bf65338718258df71877`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:19 GMT
ADD file:85c9e03c1d9121ebda028664176bf97f6e7a92eeea16af33bce6c2f6a1c4cb02 in / 
# Thu, 22 Jul 2021 00:45:19 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:41:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:41:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:41:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 17:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 17:41:54 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 17:41:55 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 17:41:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 17:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 17:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3ac06a45bc97f56a7ff01e34ad67b7ae7cb0bd2823542469d32bd69a1e5605e8`  
		Last Modified: Thu, 22 Jul 2021 00:49:49 GMT  
		Size: 31.4 MB (31355625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e190b64c0a941ff33122d59fcc9ca9c4bcbb12700f79cf2f78b5f5e5fab46c20`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b1ed4c69a01d247d265d16062afe1cd7e60557acc1b28fb86aba224e4f4cbb`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494e50df394c3910430e8505f9168527ac826dfa0527886f037b0a231c1677a2`  
		Last Modified: Mon, 16 Aug 2021 17:42:16 GMT  
		Size: 10.9 MB (10874973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8dbe476943b4eb81bf8428b43ad621f36c2ef1be3d0ecbdfeee489df2dbe9a`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8b322c0318160c75c2934bd723ebeb554cc62986a6a4393f0024107083dd7`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:61c15542f1bea87abd48bd3bf833da795a972cf790d4090ea55a6d290bad9c5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37955318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90f879e23779f5103c9fd072d33cb1d4b7e3917b6215bb83a2583537083c7dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:49:09 GMT
ADD file:19091df04c177de355e46137382ab24c0e316a9b4c2e139412ba581a0a18d1e1 in / 
# Thu, 22 Jul 2021 00:49:10 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 00:35:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 00:36:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 00:36:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 00:37:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 00:37:18 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 00:37:18 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 00:37:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 00:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 00:37:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0a1ff7527eb0e8de8a2887d94706915f958c570e660834bd28859b3960dfb63`  
		Last Modified: Thu, 22 Jul 2021 01:00:40 GMT  
		Size: 28.9 MB (28897022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c6a58e7c1e3b68268e686bf0343778937c559d986a842393f8c806a7b34c60`  
		Last Modified: Tue, 17 Aug 2021 00:37:53 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602dfd2e4e096b5fecaa80c0afe9f091248cc80db9faebcf4100c8ad7af8b66e`  
		Last Modified: Tue, 17 Aug 2021 00:37:53 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01e2c8fef9a743fb0e87a421e68eeb5d4193eafd2ddb5bc2d70cf50c9286406`  
		Last Modified: Tue, 17 Aug 2021 00:37:59 GMT  
		Size: 9.1 MB (9055037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4368a9c4fa462485f558d66b0ccc608abe9f207ed1c41ca67cdea3ac5c5bad`  
		Last Modified: Tue, 17 Aug 2021 00:37:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ad6b637824049b38a29d44e4ae702d3a67291db446652c10eb6ccc0741b47d`  
		Last Modified: Tue, 17 Aug 2021 00:37:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:602580d76c8e4de59befe6d3ffe34ace025b139a98799b4ab1b90c1e98d89265
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35115909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1753eeba61a486635abe267f9ad9f46edf7f54f190e49e06dbe9af598d8b92a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 02:02:47 GMT
ADD file:619a96435fb34ae415b7d8a447084f69a98366932e39c923941062bf09d73669 in / 
# Thu, 22 Jul 2021 02:02:48 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 00:43:01 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 00:43:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 00:43:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 00:44:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 00:44:12 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 00:44:13 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 00:44:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 00:44:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 00:44:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05bef09f82badb5e62c3bbcef85c8dff06a3270383173eb2906ed5541afbccc7`  
		Last Modified: Thu, 22 Jul 2021 02:14:54 GMT  
		Size: 26.6 MB (26559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06612b931c442de7e15ef227e99e1847d12bebabe0b54f96ca06ad0e63be9c0a`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aced7073612d1c2891301f8d2f5301f3ee9ef5180f3556aecd81a3919117cc`  
		Last Modified: Tue, 17 Aug 2021 00:45:19 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf204f2ca25c4cbd38de83228b3c595f681de4e2e0507e3e6c5d0efb842935`  
		Last Modified: Tue, 17 Aug 2021 00:45:25 GMT  
		Size: 8.6 MB (8553224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c33c91768fafd84f55b3fde36321612c24acdd00db9f0b1b7ba4aaa3a677cb9`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac6a1d40c98cce7a8a51740c2a289617146bbf2bc20161fa8e6e732fe6284e8`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
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
$ docker pull spiped@sha256:d3dd642f96becc516fb8a62318cd8a362a4402f1a8d82ee935a2954c670b968b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44762249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c5114d4e9a40f9df3298e5dbd3ceea3fd51dee675454b9f0aaba00eb679108`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:20 GMT
ADD file:7ca10cf9ec4ee7b61d4386a7797bbaa321cfff2a193f3834a78241e8674a2780 in / 
# Thu, 22 Jul 2021 00:39:20 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 16:38:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 16:39:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 16:39:01 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 16:39:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 16:39:32 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 16:39:32 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 16:39:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 16:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 16:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0a65268b957466841a0a37aa90035698fb76f15266e0baa350a093adb365ade6`  
		Last Modified: Thu, 22 Jul 2021 00:45:36 GMT  
		Size: 32.4 MB (32369313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb5ffc7bfeb22c3800b48e46c4bc03f33fea8109f52d44c22beec48e4a73d34`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd8452f42d0e0ed8e1a1ed6f8a02abf7138f2432dd06c2e9e4b9f4ba1627cd`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6499ccb36a18222e115fb8fa1e6e4d7f7d0c15a4bc07ef4ca72a88b00814a5e`  
		Last Modified: Mon, 16 Aug 2021 16:40:08 GMT  
		Size: 12.4 MB (12389675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd0b6e8e7624e147bc0aeeb4670850146880b335192adf9bfbfb35bb3eebb95`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88234b5b88b75b2e870ae1172bd4d6cbb02693e4dad0936ba9377c190860628f`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:1397de7ec9c127fa0852f12d7db9d76a690751fc21aa3c7adec345e0feef80e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39610648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b00d535f71e3926a86c308676925d0c7f6877d8b16062ab02e1444691bc7e8c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:08:58 GMT
ADD file:f1ef9d6eb38d477987532d95d608bc6d1127338387a50511169a91a11d284165 in / 
# Thu, 22 Jul 2021 00:08:58 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:08:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:09:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:09:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 17:10:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 17:10:32 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 17:10:32 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 17:10:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 17:10:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 17:10:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afeffcc83d23f7cc9022cb5ed0daac395407e585382b2889b160fb5c74e29485`  
		Last Modified: Thu, 22 Jul 2021 00:14:45 GMT  
		Size: 29.6 MB (29613402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f721acf9d11173e6aa3db0a45792ff954d8d6c5f381dd2808bae2cbe04967dc2`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784b7cb17c82bda53b2c459bf16b58c817ee954bfbbad39153e287cb17b277e6`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbec7c5c450a243dfb69ea49297c872d49ab220bfdf0ac9684a13d213944a3f`  
		Last Modified: Mon, 16 Aug 2021 17:11:06 GMT  
		Size: 10.0 MB (9994042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23eb944c6425598422492c0d1d2822fed3ba14ea2b4a643569d378f3ed99f7b1`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aeb292bdeb7661176ec0222602d00d8efba1f7f0d8b32ef24f7b49c9f9ce270`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:81e8760a45700aeccd739da2eb620ad6d31d246b398d6e5fc29568ce470ecacc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47012081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9452d89ef58183c25a133ee3196c58ebc6aa4f38da5c40764ad5be068b8246c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:17:53 GMT
ADD file:9d09cde9d8a95f1b791e4ef04a38d0e4df5c3705b2cb1fa0a1bfc71257fdab65 in / 
# Thu, 22 Jul 2021 00:18:02 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:58:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:58:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:58:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 18:06:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 18:07:03 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 18:07:15 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 18:07:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 18:07:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 18:07:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ea427ff41c744dd614b4a3c50a2c46429cf10eb87fd0bb2e2ac3e1dc4eb4d4a`  
		Last Modified: Thu, 22 Jul 2021 00:26:50 GMT  
		Size: 35.3 MB (35257797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30da9503b53aa23f533f4695a0542dd872e0aa6d5cdc3f394e885314791f745f`  
		Last Modified: Mon, 16 Aug 2021 18:08:11 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828794291318f59cfcf0a088b13d5d901cc49862fcccc66274da4e88d82eb1f`  
		Last Modified: Mon, 16 Aug 2021 18:08:11 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8f1699fb6e755f427535d5cf30286c55c7eb9cb2be984e4e49d50c9a219dd1`  
		Last Modified: Mon, 16 Aug 2021 18:08:13 GMT  
		Size: 11.8 MB (11751005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27bf8ac594a209b045a0a26d6ba9d334b17ff2aedb7162e7f7ce641fd9403ce`  
		Last Modified: Mon, 16 Aug 2021 18:08:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d13542ac8cb520531ca2742045af4f850ccf28d4106d88d56714c18821bbb47`  
		Last Modified: Mon, 16 Aug 2021 18:08:10 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:e7dbba32f20064755cf05c473ae6e9b44a3eea8a6cd5e81fdc51e22bc6028fd4
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
$ docker pull spiped@sha256:81959987e9809ba3bedbd6901a88e9fe28f2b16377bc8d3e43604661d48c2d15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3034576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d417cc665c58c81ae417555e8357d1f37bf78df7aaf23da4dcc13659df5a95a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:25:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 22:25:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 22:25:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 22:26:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 22:26:12 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 22:26:13 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 22:26:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:26:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 22:26:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9c880241f8602d0cc47e4fabf713180b354b6d9819786e78aaf3a9665b7767`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bccb485a15a7ccb6581c8d02974f14fd68b58810d648f7295647a532772b0`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 7.3 KB (7279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7741dee13e8d6c91732585334d7cef9f489ff0ba3dda16074f7cf05e58ed528a`  
		Last Modified: Fri, 06 Aug 2021 22:26:33 GMT  
		Size: 212.6 KB (212550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0337b646a0031aa1e94edce7b03cdab87816253a6850b30bf5fcfe39128e09`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc226b22f034d312b242c20826de8afa099040078d13d904d45dfeb771850e6`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:5106236450e3abdcba7735635894ff0393e5f0ce938d3fab894ece612e116c92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2837884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cdb6952199964783a11e1091cc96fa94684fd9e645edcea0376c4fef959217`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 23:52:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 23:52:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 23:52:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 23:53:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 23:53:27 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 23:53:28 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 23:53:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 23:53:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2adf0d4d8cc8b9e29d8414cae24c000412da47df5cb21a2a05ddf2e10dce570`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33562af158cbe4a36f2391938531bae4126685733de295b7ed766183da4b65ef`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23d92f94fd24201f1627f9cdbd4e09c0eced2bcbb6ebf6edd1cd206d43e2989`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 202.5 KB (202496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e821b43798aa5a90978114728243266a0f589a4f572c8034852cb0d17ce7c803`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ba2a665cda34f66fc655e2d76ea1f17e791687438e3675a6ca88c09fa438d`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b39dd207a36df0ab651368a23dd5f7fb85cb40c73169a18ed6a650c9e1e9fc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2634162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80c87f5ffe5257a7577c370989dbed14396b7ee0a5768d7e330b488935c5205`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:50:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 19:50:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 19:50:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 19:51:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 19:51:30 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 19:51:31 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 19:51:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 19:51:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d7a90d848ed25f9597b7555466d565e3c10725a9f17b4863bb5543b964fbef`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56efc9f5e430a2d91ff87e40f30089c0015233688200b25c6c645b9c75917480`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7705d09d2948f05566c3ad4b7184193f719c33fb432e05f9e9d134e1850c51f2`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 195.8 KB (195768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576177e1db2fc775ca441543afa32e5f65ec818813bbb783b5cfea5edcb0da7d`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd82adbb730f7bc7d4c11d373678c8f08c809f2f46e9cd79ae1f11169ec1f8b`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:11f573b8237bb1841a7175c9c9b77f7b8c680623ab91182c3b15186ce6d0a684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11d2305d4144c6a7caf39b8b6ca94a94d25dce28a8b4d51cbf4904172d0d3d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:20:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:20:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:20:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:20:46 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:20:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:20:47 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:20:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:20:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0faf3295f84c6343ed4bedec1bceca8f73e65a202fab2dde2578d5032f0264`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909cb3a09ec0e0c7512a5e0803fb90d9fa40a1331ebd44ac5923e377ef619c88`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 7.3 KB (7293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73e2091b0f5e799ac0526b25f8ee65662172dccf092bfcebac9a4f451801e2`  
		Last Modified: Sat, 07 Aug 2021 01:21:19 GMT  
		Size: 204.6 KB (204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3f2992d2b842a28dfa27d50163a579400dcff25c9326252f55415706303af`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac232dfb34c3889ce2beb5d4442d4a3b927e0ece42f3ab8a81de9779d579cba`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:f99c513faad87e225c2e474c95f7ceace240bcfdc0f161e74943db703f489f36
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3054380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355bc30b5b850a5b153236ee5157aa164f2754488c4565a7142fb520abe22f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 17:57:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 17:57:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 17:57:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 17:58:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 17:58:08 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 17:58:08 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 17:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 17:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 17:58:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9f8235dc8f7a2cb2e106af5945d974007f182ef18717b1358dc418b51672e7`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c8e66016715cac7eea56fb6278759a154b998e9cc867cfd9e699f45749f938`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 7.3 KB (7288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b143265a7e8e4e62818a693cb546d0cdbedb96dac486cdfaa3326b27c5669`  
		Last Modified: Fri, 06 Aug 2021 17:58:43 GMT  
		Size: 223.4 KB (223442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac32f75f64f9f329d462d69b46dad0bde0e7c7356333e99089593e3e0359d85`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d678fb9c378cbc3489d13a25fa17ca3d91d2319e6ffef53f6f84101025d21`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:fb4e68d177bc77f575c1a12ed21a941cb1ac2e423be4e1231ec7f327802e88a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3041425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8692281a7b48476e4611c785ef1f090697d8d28d64eca5cd85eabdf3842f44aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:30:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:31:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:31:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:31:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:31:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:31:54 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:31:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:32:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:32:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e1daa083c0d4e8922acb4a3735a2446ec516ebedf8992b97d0d8ac09474f9e`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ab775043317669024edb01d89328f75341409396938066bd82d18bcfa0f1b6`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9821113c32743f01e0620003d0630b6021c4148138f74add3efc51d82916a`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 221.2 KB (221239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2760cfc3e6b029ffb984aafe5b489eac1b215d0fe413a43cd00255dac46393`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b6d8de58c0e97f9000849b6c5be64af02ae4149134d50dedcb8e40e121b5e2`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:94da41acd9830f0839fe9cef81671adca1226272fa6da884c0a38ceaf9e9d943
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
$ docker pull spiped@sha256:7343758d9507624e239aaabd2c41388ea95ad4518b908ee90e466051119474ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42233860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d70d5061814f8d6b3f407f4606b44a9113ffaa5c5ee5bf65338718258df71877`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:19 GMT
ADD file:85c9e03c1d9121ebda028664176bf97f6e7a92eeea16af33bce6c2f6a1c4cb02 in / 
# Thu, 22 Jul 2021 00:45:19 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:41:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:41:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:41:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 17:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 17:41:54 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 17:41:55 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 17:41:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 17:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 17:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3ac06a45bc97f56a7ff01e34ad67b7ae7cb0bd2823542469d32bd69a1e5605e8`  
		Last Modified: Thu, 22 Jul 2021 00:49:49 GMT  
		Size: 31.4 MB (31355625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e190b64c0a941ff33122d59fcc9ca9c4bcbb12700f79cf2f78b5f5e5fab46c20`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b1ed4c69a01d247d265d16062afe1cd7e60557acc1b28fb86aba224e4f4cbb`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494e50df394c3910430e8505f9168527ac826dfa0527886f037b0a231c1677a2`  
		Last Modified: Mon, 16 Aug 2021 17:42:16 GMT  
		Size: 10.9 MB (10874973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8dbe476943b4eb81bf8428b43ad621f36c2ef1be3d0ecbdfeee489df2dbe9a`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8b322c0318160c75c2934bd723ebeb554cc62986a6a4393f0024107083dd7`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:61c15542f1bea87abd48bd3bf833da795a972cf790d4090ea55a6d290bad9c5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37955318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90f879e23779f5103c9fd072d33cb1d4b7e3917b6215bb83a2583537083c7dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:49:09 GMT
ADD file:19091df04c177de355e46137382ab24c0e316a9b4c2e139412ba581a0a18d1e1 in / 
# Thu, 22 Jul 2021 00:49:10 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 00:35:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 00:36:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 00:36:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 00:37:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 00:37:18 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 00:37:18 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 00:37:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 00:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 00:37:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0a1ff7527eb0e8de8a2887d94706915f958c570e660834bd28859b3960dfb63`  
		Last Modified: Thu, 22 Jul 2021 01:00:40 GMT  
		Size: 28.9 MB (28897022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c6a58e7c1e3b68268e686bf0343778937c559d986a842393f8c806a7b34c60`  
		Last Modified: Tue, 17 Aug 2021 00:37:53 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602dfd2e4e096b5fecaa80c0afe9f091248cc80db9faebcf4100c8ad7af8b66e`  
		Last Modified: Tue, 17 Aug 2021 00:37:53 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01e2c8fef9a743fb0e87a421e68eeb5d4193eafd2ddb5bc2d70cf50c9286406`  
		Last Modified: Tue, 17 Aug 2021 00:37:59 GMT  
		Size: 9.1 MB (9055037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4368a9c4fa462485f558d66b0ccc608abe9f207ed1c41ca67cdea3ac5c5bad`  
		Last Modified: Tue, 17 Aug 2021 00:37:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ad6b637824049b38a29d44e4ae702d3a67291db446652c10eb6ccc0741b47d`  
		Last Modified: Tue, 17 Aug 2021 00:37:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:602580d76c8e4de59befe6d3ffe34ace025b139a98799b4ab1b90c1e98d89265
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35115909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1753eeba61a486635abe267f9ad9f46edf7f54f190e49e06dbe9af598d8b92a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 02:02:47 GMT
ADD file:619a96435fb34ae415b7d8a447084f69a98366932e39c923941062bf09d73669 in / 
# Thu, 22 Jul 2021 02:02:48 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 00:43:01 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 00:43:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 00:43:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 00:44:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 00:44:12 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 00:44:13 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 00:44:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 00:44:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 00:44:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05bef09f82badb5e62c3bbcef85c8dff06a3270383173eb2906ed5541afbccc7`  
		Last Modified: Thu, 22 Jul 2021 02:14:54 GMT  
		Size: 26.6 MB (26559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06612b931c442de7e15ef227e99e1847d12bebabe0b54f96ca06ad0e63be9c0a`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aced7073612d1c2891301f8d2f5301f3ee9ef5180f3556aecd81a3919117cc`  
		Last Modified: Tue, 17 Aug 2021 00:45:19 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf204f2ca25c4cbd38de83228b3c595f681de4e2e0507e3e6c5d0efb842935`  
		Last Modified: Tue, 17 Aug 2021 00:45:25 GMT  
		Size: 8.6 MB (8553224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c33c91768fafd84f55b3fde36321612c24acdd00db9f0b1b7ba4aaa3a677cb9`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac6a1d40c98cce7a8a51740c2a289617146bbf2bc20161fa8e6e732fe6284e8`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
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
$ docker pull spiped@sha256:d3dd642f96becc516fb8a62318cd8a362a4402f1a8d82ee935a2954c670b968b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44762249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c5114d4e9a40f9df3298e5dbd3ceea3fd51dee675454b9f0aaba00eb679108`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:20 GMT
ADD file:7ca10cf9ec4ee7b61d4386a7797bbaa321cfff2a193f3834a78241e8674a2780 in / 
# Thu, 22 Jul 2021 00:39:20 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 16:38:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 16:39:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 16:39:01 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 16:39:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 16:39:32 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 16:39:32 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 16:39:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 16:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 16:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0a65268b957466841a0a37aa90035698fb76f15266e0baa350a093adb365ade6`  
		Last Modified: Thu, 22 Jul 2021 00:45:36 GMT  
		Size: 32.4 MB (32369313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb5ffc7bfeb22c3800b48e46c4bc03f33fea8109f52d44c22beec48e4a73d34`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd8452f42d0e0ed8e1a1ed6f8a02abf7138f2432dd06c2e9e4b9f4ba1627cd`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6499ccb36a18222e115fb8fa1e6e4d7f7d0c15a4bc07ef4ca72a88b00814a5e`  
		Last Modified: Mon, 16 Aug 2021 16:40:08 GMT  
		Size: 12.4 MB (12389675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd0b6e8e7624e147bc0aeeb4670850146880b335192adf9bfbfb35bb3eebb95`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88234b5b88b75b2e870ae1172bd4d6cbb02693e4dad0936ba9377c190860628f`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:1397de7ec9c127fa0852f12d7db9d76a690751fc21aa3c7adec345e0feef80e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39610648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b00d535f71e3926a86c308676925d0c7f6877d8b16062ab02e1444691bc7e8c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:08:58 GMT
ADD file:f1ef9d6eb38d477987532d95d608bc6d1127338387a50511169a91a11d284165 in / 
# Thu, 22 Jul 2021 00:08:58 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:08:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:09:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:09:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 17:10:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 17:10:32 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 17:10:32 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 17:10:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 17:10:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 17:10:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afeffcc83d23f7cc9022cb5ed0daac395407e585382b2889b160fb5c74e29485`  
		Last Modified: Thu, 22 Jul 2021 00:14:45 GMT  
		Size: 29.6 MB (29613402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f721acf9d11173e6aa3db0a45792ff954d8d6c5f381dd2808bae2cbe04967dc2`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784b7cb17c82bda53b2c459bf16b58c817ee954bfbbad39153e287cb17b277e6`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbec7c5c450a243dfb69ea49297c872d49ab220bfdf0ac9684a13d213944a3f`  
		Last Modified: Mon, 16 Aug 2021 17:11:06 GMT  
		Size: 10.0 MB (9994042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23eb944c6425598422492c0d1d2822fed3ba14ea2b4a643569d378f3ed99f7b1`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aeb292bdeb7661176ec0222602d00d8efba1f7f0d8b32ef24f7b49c9f9ce270`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:81e8760a45700aeccd739da2eb620ad6d31d246b398d6e5fc29568ce470ecacc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47012081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9452d89ef58183c25a133ee3196c58ebc6aa4f38da5c40764ad5be068b8246c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:17:53 GMT
ADD file:9d09cde9d8a95f1b791e4ef04a38d0e4df5c3705b2cb1fa0a1bfc71257fdab65 in / 
# Thu, 22 Jul 2021 00:18:02 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:58:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:58:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:58:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 18:06:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 18:07:03 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 18:07:15 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 18:07:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 18:07:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 18:07:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ea427ff41c744dd614b4a3c50a2c46429cf10eb87fd0bb2e2ac3e1dc4eb4d4a`  
		Last Modified: Thu, 22 Jul 2021 00:26:50 GMT  
		Size: 35.3 MB (35257797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30da9503b53aa23f533f4695a0542dd872e0aa6d5cdc3f394e885314791f745f`  
		Last Modified: Mon, 16 Aug 2021 18:08:11 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828794291318f59cfcf0a088b13d5d901cc49862fcccc66274da4e88d82eb1f`  
		Last Modified: Mon, 16 Aug 2021 18:08:11 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8f1699fb6e755f427535d5cf30286c55c7eb9cb2be984e4e49d50c9a219dd1`  
		Last Modified: Mon, 16 Aug 2021 18:08:13 GMT  
		Size: 11.8 MB (11751005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27bf8ac594a209b045a0a26d6ba9d334b17ff2aedb7162e7f7ce641fd9403ce`  
		Last Modified: Mon, 16 Aug 2021 18:08:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d13542ac8cb520531ca2742045af4f850ccf28d4106d88d56714c18821bbb47`  
		Last Modified: Mon, 16 Aug 2021 18:08:10 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:e7dbba32f20064755cf05c473ae6e9b44a3eea8a6cd5e81fdc51e22bc6028fd4
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
$ docker pull spiped@sha256:81959987e9809ba3bedbd6901a88e9fe28f2b16377bc8d3e43604661d48c2d15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3034576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d417cc665c58c81ae417555e8357d1f37bf78df7aaf23da4dcc13659df5a95a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:25:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 22:25:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 22:25:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 22:26:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 22:26:12 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 22:26:13 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 22:26:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:26:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 22:26:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9c880241f8602d0cc47e4fabf713180b354b6d9819786e78aaf3a9665b7767`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bccb485a15a7ccb6581c8d02974f14fd68b58810d648f7295647a532772b0`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 7.3 KB (7279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7741dee13e8d6c91732585334d7cef9f489ff0ba3dda16074f7cf05e58ed528a`  
		Last Modified: Fri, 06 Aug 2021 22:26:33 GMT  
		Size: 212.6 KB (212550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0337b646a0031aa1e94edce7b03cdab87816253a6850b30bf5fcfe39128e09`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc226b22f034d312b242c20826de8afa099040078d13d904d45dfeb771850e6`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:5106236450e3abdcba7735635894ff0393e5f0ce938d3fab894ece612e116c92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2837884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cdb6952199964783a11e1091cc96fa94684fd9e645edcea0376c4fef959217`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 23:52:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 23:52:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 23:52:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 23:53:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 23:53:27 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 23:53:28 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 23:53:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 23:53:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2adf0d4d8cc8b9e29d8414cae24c000412da47df5cb21a2a05ddf2e10dce570`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33562af158cbe4a36f2391938531bae4126685733de295b7ed766183da4b65ef`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23d92f94fd24201f1627f9cdbd4e09c0eced2bcbb6ebf6edd1cd206d43e2989`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 202.5 KB (202496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e821b43798aa5a90978114728243266a0f589a4f572c8034852cb0d17ce7c803`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ba2a665cda34f66fc655e2d76ea1f17e791687438e3675a6ca88c09fa438d`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b39dd207a36df0ab651368a23dd5f7fb85cb40c73169a18ed6a650c9e1e9fc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2634162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80c87f5ffe5257a7577c370989dbed14396b7ee0a5768d7e330b488935c5205`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:50:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 19:50:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 19:50:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 19:51:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 19:51:30 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 19:51:31 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 19:51:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 19:51:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d7a90d848ed25f9597b7555466d565e3c10725a9f17b4863bb5543b964fbef`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56efc9f5e430a2d91ff87e40f30089c0015233688200b25c6c645b9c75917480`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7705d09d2948f05566c3ad4b7184193f719c33fb432e05f9e9d134e1850c51f2`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 195.8 KB (195768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576177e1db2fc775ca441543afa32e5f65ec818813bbb783b5cfea5edcb0da7d`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd82adbb730f7bc7d4c11d373678c8f08c809f2f46e9cd79ae1f11169ec1f8b`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:11f573b8237bb1841a7175c9c9b77f7b8c680623ab91182c3b15186ce6d0a684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11d2305d4144c6a7caf39b8b6ca94a94d25dce28a8b4d51cbf4904172d0d3d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:20:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:20:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:20:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:20:46 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:20:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:20:47 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:20:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:20:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0faf3295f84c6343ed4bedec1bceca8f73e65a202fab2dde2578d5032f0264`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909cb3a09ec0e0c7512a5e0803fb90d9fa40a1331ebd44ac5923e377ef619c88`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 7.3 KB (7293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73e2091b0f5e799ac0526b25f8ee65662172dccf092bfcebac9a4f451801e2`  
		Last Modified: Sat, 07 Aug 2021 01:21:19 GMT  
		Size: 204.6 KB (204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3f2992d2b842a28dfa27d50163a579400dcff25c9326252f55415706303af`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac232dfb34c3889ce2beb5d4442d4a3b927e0ece42f3ab8a81de9779d579cba`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:f99c513faad87e225c2e474c95f7ceace240bcfdc0f161e74943db703f489f36
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3054380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355bc30b5b850a5b153236ee5157aa164f2754488c4565a7142fb520abe22f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 17:57:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 17:57:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 17:57:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 17:58:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 17:58:08 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 17:58:08 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 17:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 17:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 17:58:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9f8235dc8f7a2cb2e106af5945d974007f182ef18717b1358dc418b51672e7`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c8e66016715cac7eea56fb6278759a154b998e9cc867cfd9e699f45749f938`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 7.3 KB (7288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b143265a7e8e4e62818a693cb546d0cdbedb96dac486cdfaa3326b27c5669`  
		Last Modified: Fri, 06 Aug 2021 17:58:43 GMT  
		Size: 223.4 KB (223442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac32f75f64f9f329d462d69b46dad0bde0e7c7356333e99089593e3e0359d85`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d678fb9c378cbc3489d13a25fa17ca3d91d2319e6ffef53f6f84101025d21`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:fb4e68d177bc77f575c1a12ed21a941cb1ac2e423be4e1231ec7f327802e88a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3041425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8692281a7b48476e4611c785ef1f090697d8d28d64eca5cd85eabdf3842f44aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:30:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:31:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:31:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:31:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:31:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:31:54 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:31:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:32:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:32:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e1daa083c0d4e8922acb4a3735a2446ec516ebedf8992b97d0d8ac09474f9e`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ab775043317669024edb01d89328f75341409396938066bd82d18bcfa0f1b6`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9821113c32743f01e0620003d0630b6021c4148138f74add3efc51d82916a`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 221.2 KB (221239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2760cfc3e6b029ffb984aafe5b489eac1b215d0fe413a43cd00255dac46393`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b6d8de58c0e97f9000849b6c5be64af02ae4149134d50dedcb8e40e121b5e2`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:e7dbba32f20064755cf05c473ae6e9b44a3eea8a6cd5e81fdc51e22bc6028fd4
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
$ docker pull spiped@sha256:81959987e9809ba3bedbd6901a88e9fe28f2b16377bc8d3e43604661d48c2d15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3034576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d417cc665c58c81ae417555e8357d1f37bf78df7aaf23da4dcc13659df5a95a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:25:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 22:25:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 22:25:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 22:26:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 22:26:12 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 22:26:13 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 22:26:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:26:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 22:26:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9c880241f8602d0cc47e4fabf713180b354b6d9819786e78aaf3a9665b7767`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bccb485a15a7ccb6581c8d02974f14fd68b58810d648f7295647a532772b0`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 7.3 KB (7279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7741dee13e8d6c91732585334d7cef9f489ff0ba3dda16074f7cf05e58ed528a`  
		Last Modified: Fri, 06 Aug 2021 22:26:33 GMT  
		Size: 212.6 KB (212550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0337b646a0031aa1e94edce7b03cdab87816253a6850b30bf5fcfe39128e09`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc226b22f034d312b242c20826de8afa099040078d13d904d45dfeb771850e6`  
		Last Modified: Fri, 06 Aug 2021 22:26:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:5106236450e3abdcba7735635894ff0393e5f0ce938d3fab894ece612e116c92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2837884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cdb6952199964783a11e1091cc96fa94684fd9e645edcea0376c4fef959217`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 23:52:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 23:52:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 23:52:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 23:53:27 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 23:53:27 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 23:53:28 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 23:53:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 23:53:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2adf0d4d8cc8b9e29d8414cae24c000412da47df5cb21a2a05ddf2e10dce570`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33562af158cbe4a36f2391938531bae4126685733de295b7ed766183da4b65ef`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23d92f94fd24201f1627f9cdbd4e09c0eced2bcbb6ebf6edd1cd206d43e2989`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 202.5 KB (202496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e821b43798aa5a90978114728243266a0f589a4f572c8034852cb0d17ce7c803`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ba2a665cda34f66fc655e2d76ea1f17e791687438e3675a6ca88c09fa438d`  
		Last Modified: Fri, 06 Aug 2021 23:54:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:4b39dd207a36df0ab651368a23dd5f7fb85cb40c73169a18ed6a650c9e1e9fc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2634162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80c87f5ffe5257a7577c370989dbed14396b7ee0a5768d7e330b488935c5205`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:50:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 19:50:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 19:50:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 19:51:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 19:51:30 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 19:51:31 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 19:51:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 19:51:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d7a90d848ed25f9597b7555466d565e3c10725a9f17b4863bb5543b964fbef`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56efc9f5e430a2d91ff87e40f30089c0015233688200b25c6c645b9c75917480`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7705d09d2948f05566c3ad4b7184193f719c33fb432e05f9e9d134e1850c51f2`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 195.8 KB (195768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576177e1db2fc775ca441543afa32e5f65ec818813bbb783b5cfea5edcb0da7d`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd82adbb730f7bc7d4c11d373678c8f08c809f2f46e9cd79ae1f11169ec1f8b`  
		Last Modified: Fri, 06 Aug 2021 19:52:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:11f573b8237bb1841a7175c9c9b77f7b8c680623ab91182c3b15186ce6d0a684
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11d2305d4144c6a7caf39b8b6ca94a94d25dce28a8b4d51cbf4904172d0d3d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:20:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:20:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:20:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:20:46 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:20:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:20:47 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:20:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:20:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0faf3295f84c6343ed4bedec1bceca8f73e65a202fab2dde2578d5032f0264`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909cb3a09ec0e0c7512a5e0803fb90d9fa40a1331ebd44ac5923e377ef619c88`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 7.3 KB (7293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da73e2091b0f5e799ac0526b25f8ee65662172dccf092bfcebac9a4f451801e2`  
		Last Modified: Sat, 07 Aug 2021 01:21:19 GMT  
		Size: 204.6 KB (204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3f2992d2b842a28dfa27d50163a579400dcff25c9326252f55415706303af`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac232dfb34c3889ce2beb5d4442d4a3b927e0ece42f3ab8a81de9779d579cba`  
		Last Modified: Sat, 07 Aug 2021 01:21:18 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:f99c513faad87e225c2e474c95f7ceace240bcfdc0f161e74943db703f489f36
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3054380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355bc30b5b850a5b153236ee5157aa164f2754488c4565a7142fb520abe22f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 17:57:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 06 Aug 2021 17:57:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 06 Aug 2021 17:57:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 06 Aug 2021 17:58:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 06 Aug 2021 17:58:08 GMT
VOLUME [/spiped]
# Fri, 06 Aug 2021 17:58:08 GMT
WORKDIR /spiped
# Fri, 06 Aug 2021 17:58:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 06 Aug 2021 17:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 17:58:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9f8235dc8f7a2cb2e106af5945d974007f182ef18717b1358dc418b51672e7`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c8e66016715cac7eea56fb6278759a154b998e9cc867cfd9e699f45749f938`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 7.3 KB (7288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b143265a7e8e4e62818a693cb546d0cdbedb96dac486cdfaa3326b27c5669`  
		Last Modified: Fri, 06 Aug 2021 17:58:43 GMT  
		Size: 223.4 KB (223442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac32f75f64f9f329d462d69b46dad0bde0e7c7356333e99089593e3e0359d85`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d678fb9c378cbc3489d13a25fa17ca3d91d2319e6ffef53f6f84101025d21`  
		Last Modified: Fri, 06 Aug 2021 17:58:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:fb4e68d177bc77f575c1a12ed21a941cb1ac2e423be4e1231ec7f327802e88a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3041425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8692281a7b48476e4611c785ef1f090697d8d28d64eca5cd85eabdf3842f44aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:30:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 07 Aug 2021 01:31:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 07 Aug 2021 01:31:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 07 Aug 2021 01:31:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 07 Aug 2021 01:31:47 GMT
VOLUME [/spiped]
# Sat, 07 Aug 2021 01:31:54 GMT
WORKDIR /spiped
# Sat, 07 Aug 2021 01:31:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:32:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:32:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e1daa083c0d4e8922acb4a3735a2446ec516ebedf8992b97d0d8ac09474f9e`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ab775043317669024edb01d89328f75341409396938066bd82d18bcfa0f1b6`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9821113c32743f01e0620003d0630b6021c4148138f74add3efc51d82916a`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 221.2 KB (221239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2760cfc3e6b029ffb984aafe5b489eac1b215d0fe413a43cd00255dac46393`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b6d8de58c0e97f9000849b6c5be64af02ae4149134d50dedcb8e40e121b5e2`  
		Last Modified: Sat, 07 Aug 2021 01:32:50 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:94da41acd9830f0839fe9cef81671adca1226272fa6da884c0a38ceaf9e9d943
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
$ docker pull spiped@sha256:7343758d9507624e239aaabd2c41388ea95ad4518b908ee90e466051119474ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42233860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d70d5061814f8d6b3f407f4606b44a9113ffaa5c5ee5bf65338718258df71877`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:19 GMT
ADD file:85c9e03c1d9121ebda028664176bf97f6e7a92eeea16af33bce6c2f6a1c4cb02 in / 
# Thu, 22 Jul 2021 00:45:19 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:41:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:41:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:41:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 17:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 17:41:54 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 17:41:55 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 17:41:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 17:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 17:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3ac06a45bc97f56a7ff01e34ad67b7ae7cb0bd2823542469d32bd69a1e5605e8`  
		Last Modified: Thu, 22 Jul 2021 00:49:49 GMT  
		Size: 31.4 MB (31355625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e190b64c0a941ff33122d59fcc9ca9c4bcbb12700f79cf2f78b5f5e5fab46c20`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b1ed4c69a01d247d265d16062afe1cd7e60557acc1b28fb86aba224e4f4cbb`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494e50df394c3910430e8505f9168527ac826dfa0527886f037b0a231c1677a2`  
		Last Modified: Mon, 16 Aug 2021 17:42:16 GMT  
		Size: 10.9 MB (10874973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8dbe476943b4eb81bf8428b43ad621f36c2ef1be3d0ecbdfeee489df2dbe9a`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8b322c0318160c75c2934bd723ebeb554cc62986a6a4393f0024107083dd7`  
		Last Modified: Mon, 16 Aug 2021 17:42:14 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:61c15542f1bea87abd48bd3bf833da795a972cf790d4090ea55a6d290bad9c5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37955318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90f879e23779f5103c9fd072d33cb1d4b7e3917b6215bb83a2583537083c7dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:49:09 GMT
ADD file:19091df04c177de355e46137382ab24c0e316a9b4c2e139412ba581a0a18d1e1 in / 
# Thu, 22 Jul 2021 00:49:10 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 00:35:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 00:36:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 00:36:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 00:37:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 00:37:18 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 00:37:18 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 00:37:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 00:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 00:37:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0a1ff7527eb0e8de8a2887d94706915f958c570e660834bd28859b3960dfb63`  
		Last Modified: Thu, 22 Jul 2021 01:00:40 GMT  
		Size: 28.9 MB (28897022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c6a58e7c1e3b68268e686bf0343778937c559d986a842393f8c806a7b34c60`  
		Last Modified: Tue, 17 Aug 2021 00:37:53 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602dfd2e4e096b5fecaa80c0afe9f091248cc80db9faebcf4100c8ad7af8b66e`  
		Last Modified: Tue, 17 Aug 2021 00:37:53 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01e2c8fef9a743fb0e87a421e68eeb5d4193eafd2ddb5bc2d70cf50c9286406`  
		Last Modified: Tue, 17 Aug 2021 00:37:59 GMT  
		Size: 9.1 MB (9055037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4368a9c4fa462485f558d66b0ccc608abe9f207ed1c41ca67cdea3ac5c5bad`  
		Last Modified: Tue, 17 Aug 2021 00:37:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ad6b637824049b38a29d44e4ae702d3a67291db446652c10eb6ccc0741b47d`  
		Last Modified: Tue, 17 Aug 2021 00:37:52 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:602580d76c8e4de59befe6d3ffe34ace025b139a98799b4ab1b90c1e98d89265
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35115909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1753eeba61a486635abe267f9ad9f46edf7f54f190e49e06dbe9af598d8b92a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 02:02:47 GMT
ADD file:619a96435fb34ae415b7d8a447084f69a98366932e39c923941062bf09d73669 in / 
# Thu, 22 Jul 2021 02:02:48 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 00:43:01 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Aug 2021 00:43:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 00:43:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Aug 2021 00:44:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Aug 2021 00:44:12 GMT
VOLUME [/spiped]
# Tue, 17 Aug 2021 00:44:13 GMT
WORKDIR /spiped
# Tue, 17 Aug 2021 00:44:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Aug 2021 00:44:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Aug 2021 00:44:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05bef09f82badb5e62c3bbcef85c8dff06a3270383173eb2906ed5541afbccc7`  
		Last Modified: Thu, 22 Jul 2021 02:14:54 GMT  
		Size: 26.6 MB (26559426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06612b931c442de7e15ef227e99e1847d12bebabe0b54f96ca06ad0e63be9c0a`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aced7073612d1c2891301f8d2f5301f3ee9ef5180f3556aecd81a3919117cc`  
		Last Modified: Tue, 17 Aug 2021 00:45:19 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf204f2ca25c4cbd38de83228b3c595f681de4e2e0507e3e6c5d0efb842935`  
		Last Modified: Tue, 17 Aug 2021 00:45:25 GMT  
		Size: 8.6 MB (8553224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c33c91768fafd84f55b3fde36321612c24acdd00db9f0b1b7ba4aaa3a677cb9`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac6a1d40c98cce7a8a51740c2a289617146bbf2bc20161fa8e6e732fe6284e8`  
		Last Modified: Tue, 17 Aug 2021 00:45:18 GMT  
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
$ docker pull spiped@sha256:d3dd642f96becc516fb8a62318cd8a362a4402f1a8d82ee935a2954c670b968b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44762249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c5114d4e9a40f9df3298e5dbd3ceea3fd51dee675454b9f0aaba00eb679108`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:20 GMT
ADD file:7ca10cf9ec4ee7b61d4386a7797bbaa321cfff2a193f3834a78241e8674a2780 in / 
# Thu, 22 Jul 2021 00:39:20 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 16:38:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 16:39:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 16:39:01 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 16:39:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 16:39:32 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 16:39:32 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 16:39:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 16:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 16:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0a65268b957466841a0a37aa90035698fb76f15266e0baa350a093adb365ade6`  
		Last Modified: Thu, 22 Jul 2021 00:45:36 GMT  
		Size: 32.4 MB (32369313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb5ffc7bfeb22c3800b48e46c4bc03f33fea8109f52d44c22beec48e4a73d34`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd8452f42d0e0ed8e1a1ed6f8a02abf7138f2432dd06c2e9e4b9f4ba1627cd`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6499ccb36a18222e115fb8fa1e6e4d7f7d0c15a4bc07ef4ca72a88b00814a5e`  
		Last Modified: Mon, 16 Aug 2021 16:40:08 GMT  
		Size: 12.4 MB (12389675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd0b6e8e7624e147bc0aeeb4670850146880b335192adf9bfbfb35bb3eebb95`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88234b5b88b75b2e870ae1172bd4d6cbb02693e4dad0936ba9377c190860628f`  
		Last Modified: Mon, 16 Aug 2021 16:40:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:1397de7ec9c127fa0852f12d7db9d76a690751fc21aa3c7adec345e0feef80e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39610648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b00d535f71e3926a86c308676925d0c7f6877d8b16062ab02e1444691bc7e8c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:08:58 GMT
ADD file:f1ef9d6eb38d477987532d95d608bc6d1127338387a50511169a91a11d284165 in / 
# Thu, 22 Jul 2021 00:08:58 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:08:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:09:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:09:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 17:10:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 17:10:32 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 17:10:32 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 17:10:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 17:10:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 17:10:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afeffcc83d23f7cc9022cb5ed0daac395407e585382b2889b160fb5c74e29485`  
		Last Modified: Thu, 22 Jul 2021 00:14:45 GMT  
		Size: 29.6 MB (29613402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f721acf9d11173e6aa3db0a45792ff954d8d6c5f381dd2808bae2cbe04967dc2`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784b7cb17c82bda53b2c459bf16b58c817ee954bfbbad39153e287cb17b277e6`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbec7c5c450a243dfb69ea49297c872d49ab220bfdf0ac9684a13d213944a3f`  
		Last Modified: Mon, 16 Aug 2021 17:11:06 GMT  
		Size: 10.0 MB (9994042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23eb944c6425598422492c0d1d2822fed3ba14ea2b4a643569d378f3ed99f7b1`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aeb292bdeb7661176ec0222602d00d8efba1f7f0d8b32ef24f7b49c9f9ce270`  
		Last Modified: Mon, 16 Aug 2021 17:10:58 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:81e8760a45700aeccd739da2eb620ad6d31d246b398d6e5fc29568ce470ecacc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47012081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9452d89ef58183c25a133ee3196c58ebc6aa4f38da5c40764ad5be068b8246c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Jul 2021 00:17:53 GMT
ADD file:9d09cde9d8a95f1b791e4ef04a38d0e4df5c3705b2cb1fa0a1bfc71257fdab65 in / 
# Thu, 22 Jul 2021 00:18:02 GMT
CMD ["bash"]
# Mon, 16 Aug 2021 17:58:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 16 Aug 2021 17:58:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 16 Aug 2021 17:58:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 16 Aug 2021 18:06:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 16 Aug 2021 18:07:03 GMT
VOLUME [/spiped]
# Mon, 16 Aug 2021 18:07:15 GMT
WORKDIR /spiped
# Mon, 16 Aug 2021 18:07:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 16 Aug 2021 18:07:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Aug 2021 18:07:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ea427ff41c744dd614b4a3c50a2c46429cf10eb87fd0bb2e2ac3e1dc4eb4d4a`  
		Last Modified: Thu, 22 Jul 2021 00:26:50 GMT  
		Size: 35.3 MB (35257797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30da9503b53aa23f533f4695a0542dd872e0aa6d5cdc3f394e885314791f745f`  
		Last Modified: Mon, 16 Aug 2021 18:08:11 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9828794291318f59cfcf0a088b13d5d901cc49862fcccc66274da4e88d82eb1f`  
		Last Modified: Mon, 16 Aug 2021 18:08:11 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8f1699fb6e755f427535d5cf30286c55c7eb9cb2be984e4e49d50c9a219dd1`  
		Last Modified: Mon, 16 Aug 2021 18:08:13 GMT  
		Size: 11.8 MB (11751005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27bf8ac594a209b045a0a26d6ba9d334b17ff2aedb7162e7f7ce641fd9403ce`  
		Last Modified: Mon, 16 Aug 2021 18:08:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d13542ac8cb520531ca2742045af4f850ccf28d4106d88d56714c18821bbb47`  
		Last Modified: Mon, 16 Aug 2021 18:08:10 GMT  
		Size: 345.0 B  
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
