<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1.6.2`](#spiped162)
-	[`spiped:1.6.2-alpine`](#spiped162-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:215445d24c925f2338dec5724d5a3b4eb410440fa72077c01da8f0a9b5a2d060
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
$ docker pull spiped@sha256:515eeff0790a66d6f804a47e6066d0dc088ebce04e8b14f9d25c1907ae717db2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8398d3028b7e7e89842d7546b1b809800bb5fdaf11ae1a3eb9ea880c93fc6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:03:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:03:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:03:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:03:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:03:56 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:03:56 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:03:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:03:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec62ed2a44d78c21ab72e8eee1fbc27cb1392fa8cf508574175d315ea02cc2b0`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75e86d7e6035b646443c975a02019d31e645279762165d8a50f2c67f932c079`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2a87693b0022c3ad8f9fab9c55b79e7493e4f5f6bfe661963a18bcf230ad13`  
		Last Modified: Tue, 06 Dec 2022 08:04:15 GMT  
		Size: 6.0 MB (5998429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02692279b0822562e0d73effc9e6e2658002863fa714173db9d3c646773ad1df`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f02843045aeaf0a03708f693de0cd7996b5ad9880831a2bcad1532f6baf19`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:4c7d2251d333f8d0431820c3b578f7ae41917ca1093c5935c2388b147706ae15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aa0014abccf756d84170e4ca178cb8a05c991898f66e6fb02fe20b62f8d0df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:26 GMT
ADD file:3333e32449573e158be62ea6948788daec95a151f49035d65db8d7cb72b42c53 in / 
# Tue, 06 Dec 2022 01:49:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:43:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:44:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:44:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:44:21 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:44:21 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:44:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:44:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98c2ef299f89748b9c6075c728521ba8fe6e236fa46f50c465894cdb0ce69b35`  
		Last Modified: Tue, 06 Dec 2022 01:54:34 GMT  
		Size: 28.9 MB (28914353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ea1113a1be6fc2a9627ef082e720ff371fc45d6716fe7f722ca707538c7b1`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3887c862b2195ae4cc2a426d5f5da6cc1a1eb1aeb3a9cda029ab716e93d0a4c8`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3fd5451d1949d361ab4448641dae3c1482c3b583f689519a217b67e38dc17`  
		Last Modified: Tue, 06 Dec 2022 08:44:44 GMT  
		Size: 5.0 MB (5029310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecf2c8c904629c3af4f6d49c73ef023d6a3578840593d5c4b34d1fb74127e11`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e19dee5dfc587991ed9321301a47c108d9e1bcd7bb2fc6f545c025b18ad05b2`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:40b754b0ea2e65a750e0ca29e975bb772e33487bff62b443d2d3a52383d1f856
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31328552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665b2cb1f145cf0fe91e25c0b3bfc3f426e923bf58b844f0a566c36f00cbdd15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:44:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 09:44:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:44:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 09:45:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 09:45:11 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 09:45:11 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 09:45:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 09:45:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 09:45:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31137077cb0a083a399832c97ab11acd4066178e346b5813f3ad88e22a0565de`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77617815911ed6c386761a2b71808839da34856eb521da23c158122c5dc681c`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8da531098fead18d0722a7917658b99135017faf865e63f16660a7651b2c`  
		Last Modified: Tue, 06 Dec 2022 09:45:50 GMT  
		Size: 4.7 MB (4749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fc380b3e32f8df7a1f5caf7c53ade9e62badfc4b800cde9f8d6cac51d680ea`  
		Last Modified: Tue, 06 Dec 2022 09:45:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40dad1f3cce34a30fa25661aae54c80af7db819079b217cd779e7f27b025fada`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d2c74a0140b5ff5c4ac410868ab4e933c8fd4074b898f4f90f2b7115d320d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35335991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e5c42236284f6ec20094f338bf351249ecc7f86a22321f73b1d77ad606aaab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:35:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 10:35:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:35:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 10:35:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 10:35:25 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 10:35:25 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 10:35:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 10:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:35:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ceaf30e109e8e4905e43890b83c26829fd61fa10f17e13462ee8790b4468b8`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec2a36ae512de467eae80692b0847767fcc2b7aec528063f2b6d41bb85baa4`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ad1673176eebc504a201540453eeaee3186931383a394a3e546a276d55ef41`  
		Last Modified: Tue, 06 Dec 2022 10:35:42 GMT  
		Size: 5.3 MB (5272419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3062f7c67c493a547b2454cf88fa51cab1cc38c8df1f504ecf30d28076ead221`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29a78cb947b3e22331e5dab5bbd5b0a972a02304c8d4a269d4f140e5a2b6ffb`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:21683409c40b45caaa9892eeeb0265739531b0a7f2a5ad90060ce6e64ef3a900
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0f9496a0be91eeaf73c055cac1402e38a9a2d802d459d2f34207377e2bdd5f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:52 GMT
ADD file:3912079114d3e8e334fdf795a4793a492f37989804e1148b98fafbd4eaa00b7e in / 
# Tue, 06 Dec 2022 01:39:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:32:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 12:32:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:32:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 12:33:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 12:33:03 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 12:33:04 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 12:33:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 12:33:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:01cb95e209fce595702ddb2b5ed266e2a01b6687efe67d201d74a5aee9595995`  
		Last Modified: Tue, 06 Dec 2022 01:45:41 GMT  
		Size: 32.4 MB (32393046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc0276e5e23210f0ae119a521bb5a36c9ac6ea1ba05ec37d3890a6070d146b8`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 1.6 KB (1605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9445491c104304bdf9ba228d314dd6158c7df0b9ea50fe7795afede47acfbf`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48657d4f8cc4df23d15e90b2a96432e39cf70c9a31d6ce4b6140f7c586cb1e59`  
		Last Modified: Tue, 06 Dec 2022 12:33:38 GMT  
		Size: 7.9 MB (7890570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109e82677ad67afecdcd5f24b41d2ee08bb69eb7fd7c5f6e4d2c7004079d405e`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9774e02f7ad0b016cf2fdd82b9f5767f3f351d9643f501876bacf0bfbf485918`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:be565c6c7ce72ae179a63cc9e7907b4a895291fa066e73ecf38c64f5be74d964
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74342145bdc223560b3369661df6752c36d1bee5036d309a065bebe9ea22f992`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:55:32 GMT
ADD file:d8937be4ad87f6bed7208bb29e2f735fd2a0b27daa20617862416d53a6b9ff89 in / 
# Tue, 06 Dec 2022 01:55:36 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 16:09:14 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 16:09:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 16:09:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 16:10:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 16:11:00 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 16:11:02 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 16:11:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 16:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 16:11:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6311b5f9f3fe3987fe4883793179a21fe55ebdadf1eed52849d93fba8258d036`  
		Last Modified: Tue, 06 Dec 2022 02:03:40 GMT  
		Size: 29.6 MB (29635557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4997a4feadad1da90481ed1a8a95bcab68b8f84295bfd743a911b29207085c3e`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 1.6 KB (1612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2680706d8fc90022e9f5571d29d5a6df182256d3a36f4ffc798fd10cd86ee208`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3132b0d1095b5180c5072d286a92c426e36bb63ea144738f72305b7b2804f35a`  
		Last Modified: Tue, 06 Dec 2022 16:11:33 GMT  
		Size: 5.7 MB (5706354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced02f3e44e20f9257cdd2eda510a40ad99e1e0d7f4b40c0176be16ea82fd029`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364eb0109486bf6b0094da773dd10bf56bc9e79cfe8232ea20e021eff0cc4ade`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:7dc6c63cf3a5c782ff8771d4fc8cdb70c66a6431370a50f4ed21e8de4e72c62e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1038b04ea2f70d259f739f5db46a604ebc27dce654270a95b8bb1bf072c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:46:38 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:46:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:46:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:47:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:47:23 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:47:24 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:47:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:47:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bcd78f9b26ad833839cd08fb046f430437fd8d32e1bc5ecd748ede40c46f38`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e30172f52bc26550dbd4c93f5279187368a3e481306d39c13b4b2028c85b48`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a63688c8b5e78f3b418ecf36a67c6aa74de5018a1779b4fd3fd591630ad5b5`  
		Last Modified: Tue, 06 Dec 2022 08:48:02 GMT  
		Size: 6.0 MB (5999792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435887ede215333bcadcb79291fdc78590675fb277cfc74a82e59e86bdd7810`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711be9812e0b91d8c132be82304a099526684f5ef3ad39ff68e68e23206a2c6`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:dabf67b68c578220856eae3d1aa6e259e705dccdf5cdf67bf94231a7386985ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07220f39cb55897edd960624e94261bf233db44df4f80922a81668b1a269f18f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:43:03 GMT
ADD file:f9243ad65309c3c458bf646b21aced55c055f7601340b3bda80ec30ff2f62159 in / 
# Tue, 06 Dec 2022 01:43:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:30:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 09:30:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:30:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 09:31:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 09:31:16 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 09:31:17 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 09:31:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 09:31:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 09:31:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:66bc250ceea32b3e395aec7bb63aad4ac079791df67a2732692841e8dfacac94`  
		Last Modified: Tue, 06 Dec 2022 01:48:46 GMT  
		Size: 29.6 MB (29643886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993125537188e3ea3515bbe7e54d76f4ffc24e5c5474ab91a4cff3b9f46e3fef`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c24621fa0a7df7b3d38b83959bca65e9c73c5fda9d37fa4f47d47a3d9689f73`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156a325b8e0aad84615bca1bf738ec6e4b90c59878446cc5e3c396b38b9f294f`  
		Last Modified: Tue, 06 Dec 2022 09:32:01 GMT  
		Size: 5.2 MB (5188064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412db3e471810a565457df0caac8b5a3316d99d9086b660612fea84953773282`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ea7d77964979ec04e96d7b369b49c2e0cbbf2004d37a40bbace3c7e21f1c9b`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:e4d289144fcc0917b7c4c078e905c7eae170e8d4de2841151dabe16cd9fe14b4
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
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:1e0b653e4b6eedfa07996ee1e7d2e3a41cbae23c4c29b6410f1c3c08a843c249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ab2799394268dbce2bd74e3feebd3689100d332af8d83cfe7484a22513fc60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:56:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:56:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:56:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:56:56 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:56:57 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:56:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:56:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e26897aae3e43075b9a0367a71b2f95b6488424bfd4663f3c6c405d7096e763`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7157993d28b1a69d4025ddcdc525d561a93315db9cc66a1b0344a71ebbd264b`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 1.5 MB (1483730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86180b4c4f5e9690553a97e5582591fa162e4c4c05db84d63d77166026b4c54c`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 231.4 KB (231390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0282dbd195ef1b9176b8b02809bed658ecca6c1a8adc61249d2b82db65f5fccb`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250c8914cb765807d1d184edc38436bd02e30a85a7d66cb0632c3b4e9ee07cd`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:215445d24c925f2338dec5724d5a3b4eb410440fa72077c01da8f0a9b5a2d060
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
$ docker pull spiped@sha256:515eeff0790a66d6f804a47e6066d0dc088ebce04e8b14f9d25c1907ae717db2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8398d3028b7e7e89842d7546b1b809800bb5fdaf11ae1a3eb9ea880c93fc6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:03:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:03:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:03:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:03:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:03:56 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:03:56 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:03:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:03:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec62ed2a44d78c21ab72e8eee1fbc27cb1392fa8cf508574175d315ea02cc2b0`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75e86d7e6035b646443c975a02019d31e645279762165d8a50f2c67f932c079`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2a87693b0022c3ad8f9fab9c55b79e7493e4f5f6bfe661963a18bcf230ad13`  
		Last Modified: Tue, 06 Dec 2022 08:04:15 GMT  
		Size: 6.0 MB (5998429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02692279b0822562e0d73effc9e6e2658002863fa714173db9d3c646773ad1df`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f02843045aeaf0a03708f693de0cd7996b5ad9880831a2bcad1532f6baf19`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:4c7d2251d333f8d0431820c3b578f7ae41917ca1093c5935c2388b147706ae15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aa0014abccf756d84170e4ca178cb8a05c991898f66e6fb02fe20b62f8d0df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:26 GMT
ADD file:3333e32449573e158be62ea6948788daec95a151f49035d65db8d7cb72b42c53 in / 
# Tue, 06 Dec 2022 01:49:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:43:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:44:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:44:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:44:21 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:44:21 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:44:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:44:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98c2ef299f89748b9c6075c728521ba8fe6e236fa46f50c465894cdb0ce69b35`  
		Last Modified: Tue, 06 Dec 2022 01:54:34 GMT  
		Size: 28.9 MB (28914353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ea1113a1be6fc2a9627ef082e720ff371fc45d6716fe7f722ca707538c7b1`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3887c862b2195ae4cc2a426d5f5da6cc1a1eb1aeb3a9cda029ab716e93d0a4c8`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3fd5451d1949d361ab4448641dae3c1482c3b583f689519a217b67e38dc17`  
		Last Modified: Tue, 06 Dec 2022 08:44:44 GMT  
		Size: 5.0 MB (5029310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecf2c8c904629c3af4f6d49c73ef023d6a3578840593d5c4b34d1fb74127e11`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e19dee5dfc587991ed9321301a47c108d9e1bcd7bb2fc6f545c025b18ad05b2`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:40b754b0ea2e65a750e0ca29e975bb772e33487bff62b443d2d3a52383d1f856
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31328552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665b2cb1f145cf0fe91e25c0b3bfc3f426e923bf58b844f0a566c36f00cbdd15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:44:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 09:44:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:44:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 09:45:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 09:45:11 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 09:45:11 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 09:45:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 09:45:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 09:45:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31137077cb0a083a399832c97ab11acd4066178e346b5813f3ad88e22a0565de`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77617815911ed6c386761a2b71808839da34856eb521da23c158122c5dc681c`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8da531098fead18d0722a7917658b99135017faf865e63f16660a7651b2c`  
		Last Modified: Tue, 06 Dec 2022 09:45:50 GMT  
		Size: 4.7 MB (4749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fc380b3e32f8df7a1f5caf7c53ade9e62badfc4b800cde9f8d6cac51d680ea`  
		Last Modified: Tue, 06 Dec 2022 09:45:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40dad1f3cce34a30fa25661aae54c80af7db819079b217cd779e7f27b025fada`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d2c74a0140b5ff5c4ac410868ab4e933c8fd4074b898f4f90f2b7115d320d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35335991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e5c42236284f6ec20094f338bf351249ecc7f86a22321f73b1d77ad606aaab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:35:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 10:35:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:35:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 10:35:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 10:35:25 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 10:35:25 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 10:35:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 10:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:35:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ceaf30e109e8e4905e43890b83c26829fd61fa10f17e13462ee8790b4468b8`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec2a36ae512de467eae80692b0847767fcc2b7aec528063f2b6d41bb85baa4`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ad1673176eebc504a201540453eeaee3186931383a394a3e546a276d55ef41`  
		Last Modified: Tue, 06 Dec 2022 10:35:42 GMT  
		Size: 5.3 MB (5272419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3062f7c67c493a547b2454cf88fa51cab1cc38c8df1f504ecf30d28076ead221`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29a78cb947b3e22331e5dab5bbd5b0a972a02304c8d4a269d4f140e5a2b6ffb`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:21683409c40b45caaa9892eeeb0265739531b0a7f2a5ad90060ce6e64ef3a900
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0f9496a0be91eeaf73c055cac1402e38a9a2d802d459d2f34207377e2bdd5f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:52 GMT
ADD file:3912079114d3e8e334fdf795a4793a492f37989804e1148b98fafbd4eaa00b7e in / 
# Tue, 06 Dec 2022 01:39:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:32:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 12:32:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:32:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 12:33:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 12:33:03 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 12:33:04 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 12:33:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 12:33:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:01cb95e209fce595702ddb2b5ed266e2a01b6687efe67d201d74a5aee9595995`  
		Last Modified: Tue, 06 Dec 2022 01:45:41 GMT  
		Size: 32.4 MB (32393046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc0276e5e23210f0ae119a521bb5a36c9ac6ea1ba05ec37d3890a6070d146b8`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 1.6 KB (1605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9445491c104304bdf9ba228d314dd6158c7df0b9ea50fe7795afede47acfbf`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48657d4f8cc4df23d15e90b2a96432e39cf70c9a31d6ce4b6140f7c586cb1e59`  
		Last Modified: Tue, 06 Dec 2022 12:33:38 GMT  
		Size: 7.9 MB (7890570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109e82677ad67afecdcd5f24b41d2ee08bb69eb7fd7c5f6e4d2c7004079d405e`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9774e02f7ad0b016cf2fdd82b9f5767f3f351d9643f501876bacf0bfbf485918`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:be565c6c7ce72ae179a63cc9e7907b4a895291fa066e73ecf38c64f5be74d964
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74342145bdc223560b3369661df6752c36d1bee5036d309a065bebe9ea22f992`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:55:32 GMT
ADD file:d8937be4ad87f6bed7208bb29e2f735fd2a0b27daa20617862416d53a6b9ff89 in / 
# Tue, 06 Dec 2022 01:55:36 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 16:09:14 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 16:09:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 16:09:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 16:10:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 16:11:00 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 16:11:02 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 16:11:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 16:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 16:11:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6311b5f9f3fe3987fe4883793179a21fe55ebdadf1eed52849d93fba8258d036`  
		Last Modified: Tue, 06 Dec 2022 02:03:40 GMT  
		Size: 29.6 MB (29635557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4997a4feadad1da90481ed1a8a95bcab68b8f84295bfd743a911b29207085c3e`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 1.6 KB (1612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2680706d8fc90022e9f5571d29d5a6df182256d3a36f4ffc798fd10cd86ee208`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3132b0d1095b5180c5072d286a92c426e36bb63ea144738f72305b7b2804f35a`  
		Last Modified: Tue, 06 Dec 2022 16:11:33 GMT  
		Size: 5.7 MB (5706354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced02f3e44e20f9257cdd2eda510a40ad99e1e0d7f4b40c0176be16ea82fd029`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364eb0109486bf6b0094da773dd10bf56bc9e79cfe8232ea20e021eff0cc4ade`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:7dc6c63cf3a5c782ff8771d4fc8cdb70c66a6431370a50f4ed21e8de4e72c62e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1038b04ea2f70d259f739f5db46a604ebc27dce654270a95b8bb1bf072c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:46:38 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:46:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:46:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:47:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:47:23 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:47:24 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:47:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:47:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bcd78f9b26ad833839cd08fb046f430437fd8d32e1bc5ecd748ede40c46f38`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e30172f52bc26550dbd4c93f5279187368a3e481306d39c13b4b2028c85b48`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a63688c8b5e78f3b418ecf36a67c6aa74de5018a1779b4fd3fd591630ad5b5`  
		Last Modified: Tue, 06 Dec 2022 08:48:02 GMT  
		Size: 6.0 MB (5999792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435887ede215333bcadcb79291fdc78590675fb277cfc74a82e59e86bdd7810`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711be9812e0b91d8c132be82304a099526684f5ef3ad39ff68e68e23206a2c6`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:dabf67b68c578220856eae3d1aa6e259e705dccdf5cdf67bf94231a7386985ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07220f39cb55897edd960624e94261bf233db44df4f80922a81668b1a269f18f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:43:03 GMT
ADD file:f9243ad65309c3c458bf646b21aced55c055f7601340b3bda80ec30ff2f62159 in / 
# Tue, 06 Dec 2022 01:43:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:30:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 09:30:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:30:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 09:31:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 09:31:16 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 09:31:17 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 09:31:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 09:31:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 09:31:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:66bc250ceea32b3e395aec7bb63aad4ac079791df67a2732692841e8dfacac94`  
		Last Modified: Tue, 06 Dec 2022 01:48:46 GMT  
		Size: 29.6 MB (29643886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993125537188e3ea3515bbe7e54d76f4ffc24e5c5474ab91a4cff3b9f46e3fef`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c24621fa0a7df7b3d38b83959bca65e9c73c5fda9d37fa4f47d47a3d9689f73`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156a325b8e0aad84615bca1bf738ec6e4b90c59878446cc5e3c396b38b9f294f`  
		Last Modified: Tue, 06 Dec 2022 09:32:01 GMT  
		Size: 5.2 MB (5188064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412db3e471810a565457df0caac8b5a3316d99d9086b660612fea84953773282`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ea7d77964979ec04e96d7b369b49c2e0cbbf2004d37a40bbace3c7e21f1c9b`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:e4d289144fcc0917b7c4c078e905c7eae170e8d4de2841151dabe16cd9fe14b4
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
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:1e0b653e4b6eedfa07996ee1e7d2e3a41cbae23c4c29b6410f1c3c08a843c249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ab2799394268dbce2bd74e3feebd3689100d332af8d83cfe7484a22513fc60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:56:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:56:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:56:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:56:56 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:56:57 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:56:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:56:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e26897aae3e43075b9a0367a71b2f95b6488424bfd4663f3c6c405d7096e763`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7157993d28b1a69d4025ddcdc525d561a93315db9cc66a1b0344a71ebbd264b`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 1.5 MB (1483730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86180b4c4f5e9690553a97e5582591fa162e4c4c05db84d63d77166026b4c54c`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 231.4 KB (231390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0282dbd195ef1b9176b8b02809bed658ecca6c1a8adc61249d2b82db65f5fccb`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250c8914cb765807d1d184edc38436bd02e30a85a7d66cb0632c3b4e9ee07cd`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:215445d24c925f2338dec5724d5a3b4eb410440fa72077c01da8f0a9b5a2d060
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

### `spiped:1.6.2` - linux; amd64

```console
$ docker pull spiped@sha256:515eeff0790a66d6f804a47e6066d0dc088ebce04e8b14f9d25c1907ae717db2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8398d3028b7e7e89842d7546b1b809800bb5fdaf11ae1a3eb9ea880c93fc6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:03:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:03:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:03:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:03:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:03:56 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:03:56 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:03:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:03:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec62ed2a44d78c21ab72e8eee1fbc27cb1392fa8cf508574175d315ea02cc2b0`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75e86d7e6035b646443c975a02019d31e645279762165d8a50f2c67f932c079`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2a87693b0022c3ad8f9fab9c55b79e7493e4f5f6bfe661963a18bcf230ad13`  
		Last Modified: Tue, 06 Dec 2022 08:04:15 GMT  
		Size: 6.0 MB (5998429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02692279b0822562e0d73effc9e6e2658002863fa714173db9d3c646773ad1df`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f02843045aeaf0a03708f693de0cd7996b5ad9880831a2bcad1532f6baf19`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:4c7d2251d333f8d0431820c3b578f7ae41917ca1093c5935c2388b147706ae15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aa0014abccf756d84170e4ca178cb8a05c991898f66e6fb02fe20b62f8d0df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:26 GMT
ADD file:3333e32449573e158be62ea6948788daec95a151f49035d65db8d7cb72b42c53 in / 
# Tue, 06 Dec 2022 01:49:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:43:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:44:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:44:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:44:21 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:44:21 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:44:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:44:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98c2ef299f89748b9c6075c728521ba8fe6e236fa46f50c465894cdb0ce69b35`  
		Last Modified: Tue, 06 Dec 2022 01:54:34 GMT  
		Size: 28.9 MB (28914353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ea1113a1be6fc2a9627ef082e720ff371fc45d6716fe7f722ca707538c7b1`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3887c862b2195ae4cc2a426d5f5da6cc1a1eb1aeb3a9cda029ab716e93d0a4c8`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3fd5451d1949d361ab4448641dae3c1482c3b583f689519a217b67e38dc17`  
		Last Modified: Tue, 06 Dec 2022 08:44:44 GMT  
		Size: 5.0 MB (5029310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecf2c8c904629c3af4f6d49c73ef023d6a3578840593d5c4b34d1fb74127e11`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e19dee5dfc587991ed9321301a47c108d9e1bcd7bb2fc6f545c025b18ad05b2`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:40b754b0ea2e65a750e0ca29e975bb772e33487bff62b443d2d3a52383d1f856
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31328552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665b2cb1f145cf0fe91e25c0b3bfc3f426e923bf58b844f0a566c36f00cbdd15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:44:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 09:44:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:44:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 09:45:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 09:45:11 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 09:45:11 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 09:45:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 09:45:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 09:45:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31137077cb0a083a399832c97ab11acd4066178e346b5813f3ad88e22a0565de`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77617815911ed6c386761a2b71808839da34856eb521da23c158122c5dc681c`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8da531098fead18d0722a7917658b99135017faf865e63f16660a7651b2c`  
		Last Modified: Tue, 06 Dec 2022 09:45:50 GMT  
		Size: 4.7 MB (4749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fc380b3e32f8df7a1f5caf7c53ade9e62badfc4b800cde9f8d6cac51d680ea`  
		Last Modified: Tue, 06 Dec 2022 09:45:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40dad1f3cce34a30fa25661aae54c80af7db819079b217cd779e7f27b025fada`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d2c74a0140b5ff5c4ac410868ab4e933c8fd4074b898f4f90f2b7115d320d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35335991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e5c42236284f6ec20094f338bf351249ecc7f86a22321f73b1d77ad606aaab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:35:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 10:35:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:35:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 10:35:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 10:35:25 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 10:35:25 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 10:35:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 10:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:35:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ceaf30e109e8e4905e43890b83c26829fd61fa10f17e13462ee8790b4468b8`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec2a36ae512de467eae80692b0847767fcc2b7aec528063f2b6d41bb85baa4`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ad1673176eebc504a201540453eeaee3186931383a394a3e546a276d55ef41`  
		Last Modified: Tue, 06 Dec 2022 10:35:42 GMT  
		Size: 5.3 MB (5272419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3062f7c67c493a547b2454cf88fa51cab1cc38c8df1f504ecf30d28076ead221`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29a78cb947b3e22331e5dab5bbd5b0a972a02304c8d4a269d4f140e5a2b6ffb`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:21683409c40b45caaa9892eeeb0265739531b0a7f2a5ad90060ce6e64ef3a900
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0f9496a0be91eeaf73c055cac1402e38a9a2d802d459d2f34207377e2bdd5f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:52 GMT
ADD file:3912079114d3e8e334fdf795a4793a492f37989804e1148b98fafbd4eaa00b7e in / 
# Tue, 06 Dec 2022 01:39:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:32:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 12:32:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:32:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 12:33:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 12:33:03 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 12:33:04 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 12:33:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 12:33:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:01cb95e209fce595702ddb2b5ed266e2a01b6687efe67d201d74a5aee9595995`  
		Last Modified: Tue, 06 Dec 2022 01:45:41 GMT  
		Size: 32.4 MB (32393046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc0276e5e23210f0ae119a521bb5a36c9ac6ea1ba05ec37d3890a6070d146b8`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 1.6 KB (1605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9445491c104304bdf9ba228d314dd6158c7df0b9ea50fe7795afede47acfbf`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48657d4f8cc4df23d15e90b2a96432e39cf70c9a31d6ce4b6140f7c586cb1e59`  
		Last Modified: Tue, 06 Dec 2022 12:33:38 GMT  
		Size: 7.9 MB (7890570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109e82677ad67afecdcd5f24b41d2ee08bb69eb7fd7c5f6e4d2c7004079d405e`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9774e02f7ad0b016cf2fdd82b9f5767f3f351d9643f501876bacf0bfbf485918`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:be565c6c7ce72ae179a63cc9e7907b4a895291fa066e73ecf38c64f5be74d964
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74342145bdc223560b3369661df6752c36d1bee5036d309a065bebe9ea22f992`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:55:32 GMT
ADD file:d8937be4ad87f6bed7208bb29e2f735fd2a0b27daa20617862416d53a6b9ff89 in / 
# Tue, 06 Dec 2022 01:55:36 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 16:09:14 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 16:09:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 16:09:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 16:10:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 16:11:00 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 16:11:02 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 16:11:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 16:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 16:11:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6311b5f9f3fe3987fe4883793179a21fe55ebdadf1eed52849d93fba8258d036`  
		Last Modified: Tue, 06 Dec 2022 02:03:40 GMT  
		Size: 29.6 MB (29635557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4997a4feadad1da90481ed1a8a95bcab68b8f84295bfd743a911b29207085c3e`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 1.6 KB (1612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2680706d8fc90022e9f5571d29d5a6df182256d3a36f4ffc798fd10cd86ee208`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3132b0d1095b5180c5072d286a92c426e36bb63ea144738f72305b7b2804f35a`  
		Last Modified: Tue, 06 Dec 2022 16:11:33 GMT  
		Size: 5.7 MB (5706354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced02f3e44e20f9257cdd2eda510a40ad99e1e0d7f4b40c0176be16ea82fd029`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364eb0109486bf6b0094da773dd10bf56bc9e79cfe8232ea20e021eff0cc4ade`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:7dc6c63cf3a5c782ff8771d4fc8cdb70c66a6431370a50f4ed21e8de4e72c62e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1038b04ea2f70d259f739f5db46a604ebc27dce654270a95b8bb1bf072c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:46:38 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:46:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:46:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:47:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:47:23 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:47:24 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:47:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:47:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bcd78f9b26ad833839cd08fb046f430437fd8d32e1bc5ecd748ede40c46f38`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e30172f52bc26550dbd4c93f5279187368a3e481306d39c13b4b2028c85b48`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a63688c8b5e78f3b418ecf36a67c6aa74de5018a1779b4fd3fd591630ad5b5`  
		Last Modified: Tue, 06 Dec 2022 08:48:02 GMT  
		Size: 6.0 MB (5999792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435887ede215333bcadcb79291fdc78590675fb277cfc74a82e59e86bdd7810`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711be9812e0b91d8c132be82304a099526684f5ef3ad39ff68e68e23206a2c6`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:dabf67b68c578220856eae3d1aa6e259e705dccdf5cdf67bf94231a7386985ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07220f39cb55897edd960624e94261bf233db44df4f80922a81668b1a269f18f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:43:03 GMT
ADD file:f9243ad65309c3c458bf646b21aced55c055f7601340b3bda80ec30ff2f62159 in / 
# Tue, 06 Dec 2022 01:43:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:30:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 09:30:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:30:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 09:31:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 09:31:16 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 09:31:17 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 09:31:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 09:31:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 09:31:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:66bc250ceea32b3e395aec7bb63aad4ac079791df67a2732692841e8dfacac94`  
		Last Modified: Tue, 06 Dec 2022 01:48:46 GMT  
		Size: 29.6 MB (29643886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993125537188e3ea3515bbe7e54d76f4ffc24e5c5474ab91a4cff3b9f46e3fef`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c24621fa0a7df7b3d38b83959bca65e9c73c5fda9d37fa4f47d47a3d9689f73`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156a325b8e0aad84615bca1bf738ec6e4b90c59878446cc5e3c396b38b9f294f`  
		Last Modified: Tue, 06 Dec 2022 09:32:01 GMT  
		Size: 5.2 MB (5188064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412db3e471810a565457df0caac8b5a3316d99d9086b660612fea84953773282`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ea7d77964979ec04e96d7b369b49c2e0cbbf2004d37a40bbace3c7e21f1c9b`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:e4d289144fcc0917b7c4c078e905c7eae170e8d4de2841151dabe16cd9fe14b4
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

### `spiped:1.6.2-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:1e0b653e4b6eedfa07996ee1e7d2e3a41cbae23c4c29b6410f1c3c08a843c249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ab2799394268dbce2bd74e3feebd3689100d332af8d83cfe7484a22513fc60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:56:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:56:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:56:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:56:56 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:56:57 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:56:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:56:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e26897aae3e43075b9a0367a71b2f95b6488424bfd4663f3c6c405d7096e763`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7157993d28b1a69d4025ddcdc525d561a93315db9cc66a1b0344a71ebbd264b`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 1.5 MB (1483730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86180b4c4f5e9690553a97e5582591fa162e4c4c05db84d63d77166026b4c54c`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 231.4 KB (231390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0282dbd195ef1b9176b8b02809bed658ecca6c1a8adc61249d2b82db65f5fccb`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250c8914cb765807d1d184edc38436bd02e30a85a7d66cb0632c3b4e9ee07cd`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:e4d289144fcc0917b7c4c078e905c7eae170e8d4de2841151dabe16cd9fe14b4
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
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:1e0b653e4b6eedfa07996ee1e7d2e3a41cbae23c4c29b6410f1c3c08a843c249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ab2799394268dbce2bd74e3feebd3689100d332af8d83cfe7484a22513fc60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:56:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:56:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:56:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:56:56 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:56:57 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:56:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:56:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e26897aae3e43075b9a0367a71b2f95b6488424bfd4663f3c6c405d7096e763`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7157993d28b1a69d4025ddcdc525d561a93315db9cc66a1b0344a71ebbd264b`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 1.5 MB (1483730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86180b4c4f5e9690553a97e5582591fa162e4c4c05db84d63d77166026b4c54c`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 231.4 KB (231390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0282dbd195ef1b9176b8b02809bed658ecca6c1a8adc61249d2b82db65f5fccb`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250c8914cb765807d1d184edc38436bd02e30a85a7d66cb0632c3b4e9ee07cd`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:215445d24c925f2338dec5724d5a3b4eb410440fa72077c01da8f0a9b5a2d060
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
$ docker pull spiped@sha256:515eeff0790a66d6f804a47e6066d0dc088ebce04e8b14f9d25c1907ae717db2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8398d3028b7e7e89842d7546b1b809800bb5fdaf11ae1a3eb9ea880c93fc6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:03:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:03:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:03:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:03:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:03:56 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:03:56 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:03:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:03:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec62ed2a44d78c21ab72e8eee1fbc27cb1392fa8cf508574175d315ea02cc2b0`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75e86d7e6035b646443c975a02019d31e645279762165d8a50f2c67f932c079`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2a87693b0022c3ad8f9fab9c55b79e7493e4f5f6bfe661963a18bcf230ad13`  
		Last Modified: Tue, 06 Dec 2022 08:04:15 GMT  
		Size: 6.0 MB (5998429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02692279b0822562e0d73effc9e6e2658002863fa714173db9d3c646773ad1df`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f02843045aeaf0a03708f693de0cd7996b5ad9880831a2bcad1532f6baf19`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:4c7d2251d333f8d0431820c3b578f7ae41917ca1093c5935c2388b147706ae15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aa0014abccf756d84170e4ca178cb8a05c991898f66e6fb02fe20b62f8d0df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:26 GMT
ADD file:3333e32449573e158be62ea6948788daec95a151f49035d65db8d7cb72b42c53 in / 
# Tue, 06 Dec 2022 01:49:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:43:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:44:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:44:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:44:21 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:44:21 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:44:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:44:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98c2ef299f89748b9c6075c728521ba8fe6e236fa46f50c465894cdb0ce69b35`  
		Last Modified: Tue, 06 Dec 2022 01:54:34 GMT  
		Size: 28.9 MB (28914353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ea1113a1be6fc2a9627ef082e720ff371fc45d6716fe7f722ca707538c7b1`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3887c862b2195ae4cc2a426d5f5da6cc1a1eb1aeb3a9cda029ab716e93d0a4c8`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3fd5451d1949d361ab4448641dae3c1482c3b583f689519a217b67e38dc17`  
		Last Modified: Tue, 06 Dec 2022 08:44:44 GMT  
		Size: 5.0 MB (5029310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecf2c8c904629c3af4f6d49c73ef023d6a3578840593d5c4b34d1fb74127e11`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e19dee5dfc587991ed9321301a47c108d9e1bcd7bb2fc6f545c025b18ad05b2`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:40b754b0ea2e65a750e0ca29e975bb772e33487bff62b443d2d3a52383d1f856
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31328552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665b2cb1f145cf0fe91e25c0b3bfc3f426e923bf58b844f0a566c36f00cbdd15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:44:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 09:44:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:44:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 09:45:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 09:45:11 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 09:45:11 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 09:45:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 09:45:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 09:45:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31137077cb0a083a399832c97ab11acd4066178e346b5813f3ad88e22a0565de`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77617815911ed6c386761a2b71808839da34856eb521da23c158122c5dc681c`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8da531098fead18d0722a7917658b99135017faf865e63f16660a7651b2c`  
		Last Modified: Tue, 06 Dec 2022 09:45:50 GMT  
		Size: 4.7 MB (4749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fc380b3e32f8df7a1f5caf7c53ade9e62badfc4b800cde9f8d6cac51d680ea`  
		Last Modified: Tue, 06 Dec 2022 09:45:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40dad1f3cce34a30fa25661aae54c80af7db819079b217cd779e7f27b025fada`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d2c74a0140b5ff5c4ac410868ab4e933c8fd4074b898f4f90f2b7115d320d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35335991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e5c42236284f6ec20094f338bf351249ecc7f86a22321f73b1d77ad606aaab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:35:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 10:35:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:35:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 10:35:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 10:35:25 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 10:35:25 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 10:35:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 10:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:35:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ceaf30e109e8e4905e43890b83c26829fd61fa10f17e13462ee8790b4468b8`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec2a36ae512de467eae80692b0847767fcc2b7aec528063f2b6d41bb85baa4`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ad1673176eebc504a201540453eeaee3186931383a394a3e546a276d55ef41`  
		Last Modified: Tue, 06 Dec 2022 10:35:42 GMT  
		Size: 5.3 MB (5272419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3062f7c67c493a547b2454cf88fa51cab1cc38c8df1f504ecf30d28076ead221`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29a78cb947b3e22331e5dab5bbd5b0a972a02304c8d4a269d4f140e5a2b6ffb`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:21683409c40b45caaa9892eeeb0265739531b0a7f2a5ad90060ce6e64ef3a900
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0f9496a0be91eeaf73c055cac1402e38a9a2d802d459d2f34207377e2bdd5f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:52 GMT
ADD file:3912079114d3e8e334fdf795a4793a492f37989804e1148b98fafbd4eaa00b7e in / 
# Tue, 06 Dec 2022 01:39:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:32:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 12:32:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:32:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 12:33:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 12:33:03 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 12:33:04 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 12:33:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 12:33:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:01cb95e209fce595702ddb2b5ed266e2a01b6687efe67d201d74a5aee9595995`  
		Last Modified: Tue, 06 Dec 2022 01:45:41 GMT  
		Size: 32.4 MB (32393046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc0276e5e23210f0ae119a521bb5a36c9ac6ea1ba05ec37d3890a6070d146b8`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 1.6 KB (1605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9445491c104304bdf9ba228d314dd6158c7df0b9ea50fe7795afede47acfbf`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48657d4f8cc4df23d15e90b2a96432e39cf70c9a31d6ce4b6140f7c586cb1e59`  
		Last Modified: Tue, 06 Dec 2022 12:33:38 GMT  
		Size: 7.9 MB (7890570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109e82677ad67afecdcd5f24b41d2ee08bb69eb7fd7c5f6e4d2c7004079d405e`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9774e02f7ad0b016cf2fdd82b9f5767f3f351d9643f501876bacf0bfbf485918`  
		Last Modified: Tue, 06 Dec 2022 12:33:36 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:be565c6c7ce72ae179a63cc9e7907b4a895291fa066e73ecf38c64f5be74d964
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74342145bdc223560b3369661df6752c36d1bee5036d309a065bebe9ea22f992`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:55:32 GMT
ADD file:d8937be4ad87f6bed7208bb29e2f735fd2a0b27daa20617862416d53a6b9ff89 in / 
# Tue, 06 Dec 2022 01:55:36 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 16:09:14 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 16:09:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 16:09:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 16:10:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 16:11:00 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 16:11:02 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 16:11:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 16:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 16:11:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6311b5f9f3fe3987fe4883793179a21fe55ebdadf1eed52849d93fba8258d036`  
		Last Modified: Tue, 06 Dec 2022 02:03:40 GMT  
		Size: 29.6 MB (29635557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4997a4feadad1da90481ed1a8a95bcab68b8f84295bfd743a911b29207085c3e`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 1.6 KB (1612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2680706d8fc90022e9f5571d29d5a6df182256d3a36f4ffc798fd10cd86ee208`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3132b0d1095b5180c5072d286a92c426e36bb63ea144738f72305b7b2804f35a`  
		Last Modified: Tue, 06 Dec 2022 16:11:33 GMT  
		Size: 5.7 MB (5706354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced02f3e44e20f9257cdd2eda510a40ad99e1e0d7f4b40c0176be16ea82fd029`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364eb0109486bf6b0094da773dd10bf56bc9e79cfe8232ea20e021eff0cc4ade`  
		Last Modified: Tue, 06 Dec 2022 16:11:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:7dc6c63cf3a5c782ff8771d4fc8cdb70c66a6431370a50f4ed21e8de4e72c62e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1038b04ea2f70d259f739f5db46a604ebc27dce654270a95b8bb1bf072c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:46:38 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:46:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:46:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:47:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:47:23 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:47:24 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:47:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:47:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bcd78f9b26ad833839cd08fb046f430437fd8d32e1bc5ecd748ede40c46f38`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e30172f52bc26550dbd4c93f5279187368a3e481306d39c13b4b2028c85b48`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a63688c8b5e78f3b418ecf36a67c6aa74de5018a1779b4fd3fd591630ad5b5`  
		Last Modified: Tue, 06 Dec 2022 08:48:02 GMT  
		Size: 6.0 MB (5999792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435887ede215333bcadcb79291fdc78590675fb277cfc74a82e59e86bdd7810`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711be9812e0b91d8c132be82304a099526684f5ef3ad39ff68e68e23206a2c6`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:dabf67b68c578220856eae3d1aa6e259e705dccdf5cdf67bf94231a7386985ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07220f39cb55897edd960624e94261bf233db44df4f80922a81668b1a269f18f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:43:03 GMT
ADD file:f9243ad65309c3c458bf646b21aced55c055f7601340b3bda80ec30ff2f62159 in / 
# Tue, 06 Dec 2022 01:43:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:30:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 09:30:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:30:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 09:31:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 09:31:16 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 09:31:17 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 09:31:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 09:31:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 09:31:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:66bc250ceea32b3e395aec7bb63aad4ac079791df67a2732692841e8dfacac94`  
		Last Modified: Tue, 06 Dec 2022 01:48:46 GMT  
		Size: 29.6 MB (29643886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993125537188e3ea3515bbe7e54d76f4ffc24e5c5474ab91a4cff3b9f46e3fef`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c24621fa0a7df7b3d38b83959bca65e9c73c5fda9d37fa4f47d47a3d9689f73`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156a325b8e0aad84615bca1bf738ec6e4b90c59878446cc5e3c396b38b9f294f`  
		Last Modified: Tue, 06 Dec 2022 09:32:01 GMT  
		Size: 5.2 MB (5188064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412db3e471810a565457df0caac8b5a3316d99d9086b660612fea84953773282`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ea7d77964979ec04e96d7b369b49c2e0cbbf2004d37a40bbace3c7e21f1c9b`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
