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
$ docker pull spiped@sha256:ab6427d6903f8c26ed3da5c6bea858043a2043a6454daee528194faf1daa952b
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
$ docker pull spiped@sha256:8cd0d350e2a175da5f685212ca720cd31451daaa5c1c3ce22268a6c098628210
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0db056ae424f84934906f39c45bedff6339474a256240442fac553e048ab43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:25:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 14:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:25:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 14:26:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:26:06 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 14:26:06 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 14:26:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 14:26:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 14:26:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f05cfc98bdaab076eb82751252e3e75f04ba7cfe8574948694f75664ca08bd`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fbdb1be8384f98617d85b0a558459f05f31aec8a6f50df7182b1d0fbb9e01f`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17020edad6b1b0115116b35db60695f0f7ec88d5131069843c36bfc054d5863b`  
		Last Modified: Tue, 15 Nov 2022 14:26:24 GMT  
		Size: 6.0 MB (5998420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a563f1a79ce4f6624f04ac38760550529ab712ee4d46a3511ab645c054e6bbb`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a3a38d3e6c729c4b6d04992a60df1c5e4fd52f25f06a8708668e0568ebe22b`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:ec9790e3310ab830942f954fecd18dcd4a7fc78930eb5e9865b493c09d8de342
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f25e72bc7a8fea9ed51c48382332e6ad92a68e3821d104133619fe2a4ed8f376`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:18 GMT
ADD file:1949af7e583a1b54055a421129c32315fc101e53e2cda05da3171ed461bde0a6 in / 
# Tue, 15 Nov 2022 01:49:19 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:12:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 10:12:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:12:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 10:12:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 10:12:52 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 10:12:52 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 10:12:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 10:12:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:12:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b56836d864a6d857be3d12242b65962f2a2cf0d77c48cfb85bbbdf9d56a7e93d`  
		Last Modified: Tue, 15 Nov 2022 01:54:26 GMT  
		Size: 28.9 MB (28914126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52010eba05268403bb9ce16397f34a8d809c7d45381ed17d54727ec5312f8e64`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7f68ad0da9f44bae685b91c83e3125017b5e1fa894e902eb8af4059ec64232`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d61522f3adb083ae0c3a1100dd755cae1c3068f4615122d0d4d9fb9dcbd553b`  
		Last Modified: Tue, 15 Nov 2022 10:13:15 GMT  
		Size: 5.0 MB (5029291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382a079faf68aa665a39ca7ccb83043aa797d1c5ee7951f318b9c2bece18802b`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a4b4fabe7c1bacd9b9e252066f171608f18bc9125cae758db235ade53e961c`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bfff3efcf03753ba51d784c4deaee4cb8e634cede50272f622be6701a39e2c2e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31331482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed2d92b57a070235e7c98b6ba242d1cbd18b6492b75f763388eff3d53dc4d2e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 04:08:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Oct 2022 04:08:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 04:08:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Oct 2022 04:09:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Oct 2022 04:09:01 GMT
VOLUME [/spiped]
# Wed, 26 Oct 2022 04:09:01 GMT
WORKDIR /spiped
# Wed, 26 Oct 2022 04:09:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Oct 2022 04:09:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 04:09:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adf378b5b9701669a758188b83d55e929eb48bd4c543f9b8f8a431570a6711d`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c6587474e215654a49ffdca22b9d48921c15b50cf53a07d57670bb4caaf2cd`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b726e98a4dbc4add399728b2912edba24f9efb947fd81fd7e885e02c4ba50a`  
		Last Modified: Wed, 26 Oct 2022 04:09:54 GMT  
		Size: 4.7 MB (4749002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f830752e5f1c0df89505c43f8ee698e7b59e1a17aa5a93d366d0d83dc1d2d5d6`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce0b6a93edcda9a62223fb9e4977ef54baffc64715df9cfbbce9b2d943e9950`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:15446b678eff03a766ba070afd86b1b4b2b512383e7e86ae05bdbe35761d32cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960d815e93ee6a3ba5b7e52ef354ad4259e2ad94c8cdaee91366cdac33ce10d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:25:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:25:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:25:35 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:25:35 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:25:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f263b1855bd471c83539756f8b70a58c84c9dc0ff2dbcb682afdf46fa84af`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f63490a49f76c19d7c7411339c219429156afda6ef909fcb6e4aa90b7bcbc`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc90b9cb2517275e1ea4f6fa67c968e862002478d6945dd0a455d324aa9e9ef8`  
		Last Modified: Tue, 15 Nov 2022 13:25:56 GMT  
		Size: 5.3 MB (5272459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b17c3ba478f87caafa84a5a1a090060c3e18cf2ef8b7000dd0294fd8c425286`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bfbc8db5dc7db117e54b445680eb62aced5bdafa9c38b141250fc7aa7d5a8a`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:bc3034ea433bc46dd8c0b1f375517e13ebce3786f7ecbfffdb7edc99af6185f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe71f396ab173d0e7a95d9be87cd921b46ab02f959c0cbf70a4d5b39250f548e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 17:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 17:51:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 17:51:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 17:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 17:51:59 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 17:52:00 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 17:52:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 17:52:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 17:52:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fbdc019d80d6a30ab90868896498a28c5e819659f22bb2894d5fc2e7d6bb3f`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d64fbdfcaf79efbaf8da0d679f65709cf4066699e35b9fbb0029f30317bbf9`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1159f60b8a31090685214f0ae08d84535c724e5e92a2f79c4684a8af8435bdb`  
		Last Modified: Tue, 15 Nov 2022 17:52:34 GMT  
		Size: 7.9 MB (7890569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48a2b4bd1d2bd7ea1b36aea4ae7e36171af6be414a64513fdab695cf409fd0`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abba44a7b8700f9ac9dd0dba12b7983ecdc4c918ba4f8129e912828bd9b529`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:aac80a4c64529fa60afc110d64d0c85b6a568df1b7cb5a5a9ca9d5ac966ca456
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dad9d417652d7dc5fa4f1473c6a4076a1d44506ae13e748b502ed478db269`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 00:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 00:04:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:04:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 00:06:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 00:06:10 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 00:06:13 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 00:06:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 00:06:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 00:06:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423cc689eb0f49221096b6d78f2f88cde0b37b5c1b49367ebff22a6e1ee33ba`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff778c8a78825f7845b585d8dae3024757f98b009043b391253b9555d1bd3ee2`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9787dc2ceb548759ff582e8606939f449df9a0dd7ce05dc5d1722c52cb9feb0c`  
		Last Modified: Wed, 16 Nov 2022 00:06:51 GMT  
		Size: 5.7 MB (5706376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e18e00bc8e5f5bd8ded0d5c9a2d7e7ef1eddc72b6c9594971ecc6a5cd62c3d`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867e28a7d951478254c55c58be169d8812eaa99008aa6b11248a5c9046ae2f3`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:a4e046168feb1ad487131c35168c1565ab29cadfb409be2835dff56c857c96dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0760132dad5ee85c440e6c65bfb91e366f095c47c565a5c69bfc2730a81b81e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 05:18:45 GMT
ADD file:520926164fdc762143905745329e568c67289232bec450e48645d82a4613dccf in / 
# Tue, 15 Nov 2022 05:18:47 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 18:33:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 18:33:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 18:33:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 18:34:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 18:34:09 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 18:34:09 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 18:34:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 18:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 18:34:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c57913b7d0318ef1a47f0348ce54d9865316776aa1ffb2c7871b1473b3d29407`  
		Last Modified: Tue, 15 Nov 2022 05:24:22 GMT  
		Size: 35.3 MB (35285140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a5d9c14025c15f34163961f4eafc162696a33cc493eaa86dc0b54fa025e646`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddacb9148d8a6e8ce0f8dc4a7074198eea102ea0da570ce71824001314ec581`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a5572d4fe22794ba76d4bf209b17ff799559f885284884850d02580328ea93`  
		Last Modified: Tue, 15 Nov 2022 18:34:47 GMT  
		Size: 6.0 MB (5999748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42de0ee16e98c0a72bc01c622a96fa73c429fee856e55b597c7248a40335d900`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d7db34ebd9272908023a6993d28bbd615a3897bbba7d518beed99fbee7b30a`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:c473e05e698144dc8315ef89467944d3111b39a88bbad9963db8ab7843059b73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa617c4a5699ed04e207e266e667d59db1d726bba445409e8a648f5a6e4c18af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:14:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:14:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:14:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:15:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:15:44 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:15:45 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:15:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:15:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:15:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d0559b9988e98911430249fdef7b998e0b4c32305f0ccd4bcb8905987488be`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2b9a5754a77e47074f8f2ac4a0d9905ce7bd388dcb1f07ad8748af5ffc3e23`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7788cf8d0aadbaa693ab2c8e52e54631507aaac0f3a376941ec75476a67778a`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 5.2 MB (5188015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a9f1f79d29017e6e16df8a84cd6ca4120daaabd71eecb98fce0747916d094d`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d84d4f34ee0b4bc57bc91e1c4d2b9825b124f70fe19c92c828d01c7d9325a`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:82dced4a656b2d513450d2342ecddc3f9244f04c9c07a8565d1e90dd24b83259
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
$ docker pull spiped@sha256:88600bfd34359fe38ba773717d293fc4d6095338551ab0b9c98ced2944029635
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef58a68bf7b0e4e343f1c174cd34a75b21f0714a3fe9e5e50df70c1cb3313a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:31:09 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:31:10 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:31:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:31:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:31:21 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:31:21 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:31:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:31:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:31:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba143d89ef43493de610789b011ec6f78fd98311801bd1b895263425d2b80f9`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3bf49195ff499a5b7913c2890b39e1ca85bd2ba2fc46bdf7967974cdaa578`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 7.8 KB (7762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6bcd4c1d546b37c09f8d577cb9065b685c82b401a5f2271774cdf3a57f325e`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 221.2 KB (221203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e9846fbf23dbba2f28e731ca1a2b68957835ecbfe09de8fcecd43f01ce7312`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1bbea7f748e9071525f54078c4c1afed13fcad17509d2a56a430c21b8b56d5`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:4a97e4614d77053ba39fa5c745d6105a7715cb2a1339a25d4fa13a27d0d5b071
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef16808dbefc833d0994260a2717a0477aecef28d949a2bd4c8da571b5627b51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:28:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:28:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:28:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:28:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:28:26 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:28:26 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:28:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:28:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:28:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ad9b8c9f0b2df322f6b1cabda5e7ca816a4a3d899eb140b118c2827fddfe2`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2057d8252d211e7c1c7a5a22ff586d7ad6fb222a67ddc10c861346d2f5de70d7`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 7.8 KB (7761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7036cdcac704f3ec530ed23d018a37fa64b0d4e1ec8c26bd0388a1a2d99220d7`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 205.9 KB (205882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d603c20f7582181b49742ecc7a817667c6067b1e3ee6ec3e64ecbe1bf10206d0`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2d6b98135a7de547f76953f15d873bc47703d65c6f2c87b0a719561fb1066f`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:da26d167b81e6942d2bf840b15ff59a945c83bcb6c34968a2cb76d61b48368d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2627783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335ebf8c2444c91778b85ac23284d5a8bb8a0564755cb6ea06160705fc72ebfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:09:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:10:00 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:10:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:10:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:10:09 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:10:09 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:10:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:10:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:10:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adeca438422069f0b2d529c93aa015b2d66ff14e7f811a2db7155b3780f3f17`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a307f22f7b61faf288c16b2e278af2069d3f0f1d7ccb5de2669081f800b82595`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 7.8 KB (7766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ada82ce81437697e7bbaef8a8df96fe30079d2b62708af97071da84c0be91f`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 199.6 KB (199550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650ecac6d83dd8ac1473ff90545abe2e47ad63985de2031e7fb65a25c99847b2`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304511b2e0cd4c9408aace74412dcce1dcbb72f7cc52fa88e57892bfe2beae31`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cc37e731d1198e448359b790e73b2016b757e9d1a05425fa0a2df9fc6fe0cc9b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe1152848438c5b85156eb4f564f5a436e27d69210842e300de2be7c0bdf598`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 09:52:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 09:52:51 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 09:52:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 09:52:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 09:52:59 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 09:52:59 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 09:52:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 09:52:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 09:52:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a33d40b7aea60d797950562e12532c05e2bec1dfb8dc5431f8c871028f801d`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046893368895bc36323127bb34d70394b9e08715b8cd3609c1396fd7dcc7baad`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d84e6ac65d4649eecb08b3cb834f0b6205a88df39adc3099e196a2e03d066`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 214.6 KB (214567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7ee94c43226ce1cbb59b1a15b651a023be893f860642d7af91e0dbf49b0bdf`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053b7b3dc658bda7a53962394fac910f8408b95bc4066c9342ad508eb98fb56e`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:843ee0a06fce410e9185f279bedec495552d30a9b235351c9e52bd669095b6a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3049117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c9c942ec6bc7f10412698170c354b1c1e3784c5293bb45763683f9fae4ff45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:29:06 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 07:29:08 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 07:29:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 07:29:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 07:29:21 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 07:29:22 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 07:29:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 07:29:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 07:29:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d809fb6be6b6c5126ea93c77f723eabd38a79da96195f2112d4ba37475d11cec`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed4111161b7b7d291c73883105977d83b95161ff3092cb8c51baa969a0f4f40`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefd93dcc118fc9b6c2575a0e2e6442cf1941ad36cd7c23a11ff37f954d72696`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 231.4 KB (231353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12465fe04c57bef25da7dd19448585a8f389a2be5002904390928db02803c463`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19ff97a8609ea6c7b399819d80dd69016ccd3db9c032fb36c9caaec3462cde`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9a5fa9635e3b3150a7fb86be203bd9ac800242a8715366e1ebf80137524c1d49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3422852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aac8ab48bba973ccd96958d6b1a6ead1c79dc7016524a07dc87240ccf918e9f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 13:39:51 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 13:39:53 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 13:39:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 13:40:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 13:40:08 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 13:40:09 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 13:40:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 13:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 13:40:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0194afa072d947a442ef104e10d9216659dfc8a0d66a1aa9d83dc2daa6d3cb60`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3636e065dbfa3ffe9e220f75a2656046c6e68daa308f669c824c33129da33d8e`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 7.8 KB (7776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6a06d391f6599e576cc221ab33e97777c1a2d34912c03b26bb42f42ba72ca`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 611.8 KB (611788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0000fde7d027d5e5be6d184daac6a936d889c009e92180fc9992b2e1b4385cc`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385151a4c23844070ef5830264bf1ee9abeb01f86bbb0c5dba45868ea8324f3c`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:47e6ca3b66046e043d8efb1996b3f02334b21d52d0378b9e70a9eee14bc8ba05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2809081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bb44b07872890902f462d8051264598233b2791b8d17ac8d1e9650682147605`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:49:57 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:49:59 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:49:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:50:06 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:50:06 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:50:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:50:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:50:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c21b0fe0ff4f5675555696be2fdd46dbd120c67b2a2a82d2f9358d673a2fddc`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faafadd95cb1b92a7217a5e1a180e88ffd0de612088f75c144bbf3d501585ff`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157d141feb67cd00e910527177fb9131596a73032d3f627e9160255a17512dc6`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 208.4 KB (208447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5180ea5424d8443b199fbe5a892596a2c6d2f9fff62a8e41bcc2a68035514`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda12945c53bd011c9f75619e916738acd26381a21194ab28a173176009878b0`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:ab6427d6903f8c26ed3da5c6bea858043a2043a6454daee528194faf1daa952b
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
$ docker pull spiped@sha256:8cd0d350e2a175da5f685212ca720cd31451daaa5c1c3ce22268a6c098628210
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0db056ae424f84934906f39c45bedff6339474a256240442fac553e048ab43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:25:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 14:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:25:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 14:26:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:26:06 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 14:26:06 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 14:26:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 14:26:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 14:26:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f05cfc98bdaab076eb82751252e3e75f04ba7cfe8574948694f75664ca08bd`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fbdb1be8384f98617d85b0a558459f05f31aec8a6f50df7182b1d0fbb9e01f`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17020edad6b1b0115116b35db60695f0f7ec88d5131069843c36bfc054d5863b`  
		Last Modified: Tue, 15 Nov 2022 14:26:24 GMT  
		Size: 6.0 MB (5998420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a563f1a79ce4f6624f04ac38760550529ab712ee4d46a3511ab645c054e6bbb`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a3a38d3e6c729c4b6d04992a60df1c5e4fd52f25f06a8708668e0568ebe22b`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:ec9790e3310ab830942f954fecd18dcd4a7fc78930eb5e9865b493c09d8de342
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f25e72bc7a8fea9ed51c48382332e6ad92a68e3821d104133619fe2a4ed8f376`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:18 GMT
ADD file:1949af7e583a1b54055a421129c32315fc101e53e2cda05da3171ed461bde0a6 in / 
# Tue, 15 Nov 2022 01:49:19 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:12:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 10:12:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:12:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 10:12:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 10:12:52 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 10:12:52 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 10:12:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 10:12:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:12:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b56836d864a6d857be3d12242b65962f2a2cf0d77c48cfb85bbbdf9d56a7e93d`  
		Last Modified: Tue, 15 Nov 2022 01:54:26 GMT  
		Size: 28.9 MB (28914126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52010eba05268403bb9ce16397f34a8d809c7d45381ed17d54727ec5312f8e64`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7f68ad0da9f44bae685b91c83e3125017b5e1fa894e902eb8af4059ec64232`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d61522f3adb083ae0c3a1100dd755cae1c3068f4615122d0d4d9fb9dcbd553b`  
		Last Modified: Tue, 15 Nov 2022 10:13:15 GMT  
		Size: 5.0 MB (5029291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382a079faf68aa665a39ca7ccb83043aa797d1c5ee7951f318b9c2bece18802b`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a4b4fabe7c1bacd9b9e252066f171608f18bc9125cae758db235ade53e961c`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bfff3efcf03753ba51d784c4deaee4cb8e634cede50272f622be6701a39e2c2e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31331482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed2d92b57a070235e7c98b6ba242d1cbd18b6492b75f763388eff3d53dc4d2e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 04:08:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Oct 2022 04:08:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 04:08:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Oct 2022 04:09:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Oct 2022 04:09:01 GMT
VOLUME [/spiped]
# Wed, 26 Oct 2022 04:09:01 GMT
WORKDIR /spiped
# Wed, 26 Oct 2022 04:09:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Oct 2022 04:09:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 04:09:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adf378b5b9701669a758188b83d55e929eb48bd4c543f9b8f8a431570a6711d`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c6587474e215654a49ffdca22b9d48921c15b50cf53a07d57670bb4caaf2cd`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b726e98a4dbc4add399728b2912edba24f9efb947fd81fd7e885e02c4ba50a`  
		Last Modified: Wed, 26 Oct 2022 04:09:54 GMT  
		Size: 4.7 MB (4749002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f830752e5f1c0df89505c43f8ee698e7b59e1a17aa5a93d366d0d83dc1d2d5d6`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce0b6a93edcda9a62223fb9e4977ef54baffc64715df9cfbbce9b2d943e9950`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:15446b678eff03a766ba070afd86b1b4b2b512383e7e86ae05bdbe35761d32cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960d815e93ee6a3ba5b7e52ef354ad4259e2ad94c8cdaee91366cdac33ce10d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:25:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:25:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:25:35 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:25:35 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:25:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f263b1855bd471c83539756f8b70a58c84c9dc0ff2dbcb682afdf46fa84af`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f63490a49f76c19d7c7411339c219429156afda6ef909fcb6e4aa90b7bcbc`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc90b9cb2517275e1ea4f6fa67c968e862002478d6945dd0a455d324aa9e9ef8`  
		Last Modified: Tue, 15 Nov 2022 13:25:56 GMT  
		Size: 5.3 MB (5272459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b17c3ba478f87caafa84a5a1a090060c3e18cf2ef8b7000dd0294fd8c425286`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bfbc8db5dc7db117e54b445680eb62aced5bdafa9c38b141250fc7aa7d5a8a`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:bc3034ea433bc46dd8c0b1f375517e13ebce3786f7ecbfffdb7edc99af6185f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe71f396ab173d0e7a95d9be87cd921b46ab02f959c0cbf70a4d5b39250f548e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 17:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 17:51:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 17:51:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 17:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 17:51:59 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 17:52:00 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 17:52:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 17:52:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 17:52:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fbdc019d80d6a30ab90868896498a28c5e819659f22bb2894d5fc2e7d6bb3f`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d64fbdfcaf79efbaf8da0d679f65709cf4066699e35b9fbb0029f30317bbf9`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1159f60b8a31090685214f0ae08d84535c724e5e92a2f79c4684a8af8435bdb`  
		Last Modified: Tue, 15 Nov 2022 17:52:34 GMT  
		Size: 7.9 MB (7890569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48a2b4bd1d2bd7ea1b36aea4ae7e36171af6be414a64513fdab695cf409fd0`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abba44a7b8700f9ac9dd0dba12b7983ecdc4c918ba4f8129e912828bd9b529`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:aac80a4c64529fa60afc110d64d0c85b6a568df1b7cb5a5a9ca9d5ac966ca456
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dad9d417652d7dc5fa4f1473c6a4076a1d44506ae13e748b502ed478db269`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 00:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 00:04:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:04:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 00:06:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 00:06:10 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 00:06:13 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 00:06:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 00:06:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 00:06:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423cc689eb0f49221096b6d78f2f88cde0b37b5c1b49367ebff22a6e1ee33ba`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff778c8a78825f7845b585d8dae3024757f98b009043b391253b9555d1bd3ee2`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9787dc2ceb548759ff582e8606939f449df9a0dd7ce05dc5d1722c52cb9feb0c`  
		Last Modified: Wed, 16 Nov 2022 00:06:51 GMT  
		Size: 5.7 MB (5706376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e18e00bc8e5f5bd8ded0d5c9a2d7e7ef1eddc72b6c9594971ecc6a5cd62c3d`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867e28a7d951478254c55c58be169d8812eaa99008aa6b11248a5c9046ae2f3`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:a4e046168feb1ad487131c35168c1565ab29cadfb409be2835dff56c857c96dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0760132dad5ee85c440e6c65bfb91e366f095c47c565a5c69bfc2730a81b81e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 05:18:45 GMT
ADD file:520926164fdc762143905745329e568c67289232bec450e48645d82a4613dccf in / 
# Tue, 15 Nov 2022 05:18:47 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 18:33:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 18:33:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 18:33:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 18:34:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 18:34:09 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 18:34:09 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 18:34:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 18:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 18:34:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c57913b7d0318ef1a47f0348ce54d9865316776aa1ffb2c7871b1473b3d29407`  
		Last Modified: Tue, 15 Nov 2022 05:24:22 GMT  
		Size: 35.3 MB (35285140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a5d9c14025c15f34163961f4eafc162696a33cc493eaa86dc0b54fa025e646`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddacb9148d8a6e8ce0f8dc4a7074198eea102ea0da570ce71824001314ec581`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a5572d4fe22794ba76d4bf209b17ff799559f885284884850d02580328ea93`  
		Last Modified: Tue, 15 Nov 2022 18:34:47 GMT  
		Size: 6.0 MB (5999748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42de0ee16e98c0a72bc01c622a96fa73c429fee856e55b597c7248a40335d900`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d7db34ebd9272908023a6993d28bbd615a3897bbba7d518beed99fbee7b30a`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:c473e05e698144dc8315ef89467944d3111b39a88bbad9963db8ab7843059b73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa617c4a5699ed04e207e266e667d59db1d726bba445409e8a648f5a6e4c18af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:14:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:14:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:14:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:15:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:15:44 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:15:45 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:15:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:15:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:15:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d0559b9988e98911430249fdef7b998e0b4c32305f0ccd4bcb8905987488be`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2b9a5754a77e47074f8f2ac4a0d9905ce7bd388dcb1f07ad8748af5ffc3e23`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7788cf8d0aadbaa693ab2c8e52e54631507aaac0f3a376941ec75476a67778a`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 5.2 MB (5188015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a9f1f79d29017e6e16df8a84cd6ca4120daaabd71eecb98fce0747916d094d`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d84d4f34ee0b4bc57bc91e1c4d2b9825b124f70fe19c92c828d01c7d9325a`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:82dced4a656b2d513450d2342ecddc3f9244f04c9c07a8565d1e90dd24b83259
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
$ docker pull spiped@sha256:88600bfd34359fe38ba773717d293fc4d6095338551ab0b9c98ced2944029635
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef58a68bf7b0e4e343f1c174cd34a75b21f0714a3fe9e5e50df70c1cb3313a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:31:09 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:31:10 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:31:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:31:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:31:21 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:31:21 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:31:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:31:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:31:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba143d89ef43493de610789b011ec6f78fd98311801bd1b895263425d2b80f9`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3bf49195ff499a5b7913c2890b39e1ca85bd2ba2fc46bdf7967974cdaa578`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 7.8 KB (7762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6bcd4c1d546b37c09f8d577cb9065b685c82b401a5f2271774cdf3a57f325e`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 221.2 KB (221203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e9846fbf23dbba2f28e731ca1a2b68957835ecbfe09de8fcecd43f01ce7312`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1bbea7f748e9071525f54078c4c1afed13fcad17509d2a56a430c21b8b56d5`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:4a97e4614d77053ba39fa5c745d6105a7715cb2a1339a25d4fa13a27d0d5b071
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef16808dbefc833d0994260a2717a0477aecef28d949a2bd4c8da571b5627b51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:28:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:28:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:28:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:28:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:28:26 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:28:26 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:28:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:28:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:28:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ad9b8c9f0b2df322f6b1cabda5e7ca816a4a3d899eb140b118c2827fddfe2`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2057d8252d211e7c1c7a5a22ff586d7ad6fb222a67ddc10c861346d2f5de70d7`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 7.8 KB (7761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7036cdcac704f3ec530ed23d018a37fa64b0d4e1ec8c26bd0388a1a2d99220d7`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 205.9 KB (205882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d603c20f7582181b49742ecc7a817667c6067b1e3ee6ec3e64ecbe1bf10206d0`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2d6b98135a7de547f76953f15d873bc47703d65c6f2c87b0a719561fb1066f`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:da26d167b81e6942d2bf840b15ff59a945c83bcb6c34968a2cb76d61b48368d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2627783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335ebf8c2444c91778b85ac23284d5a8bb8a0564755cb6ea06160705fc72ebfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:09:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:10:00 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:10:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:10:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:10:09 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:10:09 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:10:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:10:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:10:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adeca438422069f0b2d529c93aa015b2d66ff14e7f811a2db7155b3780f3f17`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a307f22f7b61faf288c16b2e278af2069d3f0f1d7ccb5de2669081f800b82595`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 7.8 KB (7766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ada82ce81437697e7bbaef8a8df96fe30079d2b62708af97071da84c0be91f`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 199.6 KB (199550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650ecac6d83dd8ac1473ff90545abe2e47ad63985de2031e7fb65a25c99847b2`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304511b2e0cd4c9408aace74412dcce1dcbb72f7cc52fa88e57892bfe2beae31`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cc37e731d1198e448359b790e73b2016b757e9d1a05425fa0a2df9fc6fe0cc9b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe1152848438c5b85156eb4f564f5a436e27d69210842e300de2be7c0bdf598`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 09:52:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 09:52:51 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 09:52:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 09:52:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 09:52:59 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 09:52:59 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 09:52:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 09:52:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 09:52:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a33d40b7aea60d797950562e12532c05e2bec1dfb8dc5431f8c871028f801d`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046893368895bc36323127bb34d70394b9e08715b8cd3609c1396fd7dcc7baad`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d84e6ac65d4649eecb08b3cb834f0b6205a88df39adc3099e196a2e03d066`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 214.6 KB (214567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7ee94c43226ce1cbb59b1a15b651a023be893f860642d7af91e0dbf49b0bdf`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053b7b3dc658bda7a53962394fac910f8408b95bc4066c9342ad508eb98fb56e`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:843ee0a06fce410e9185f279bedec495552d30a9b235351c9e52bd669095b6a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3049117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c9c942ec6bc7f10412698170c354b1c1e3784c5293bb45763683f9fae4ff45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:29:06 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 07:29:08 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 07:29:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 07:29:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 07:29:21 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 07:29:22 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 07:29:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 07:29:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 07:29:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d809fb6be6b6c5126ea93c77f723eabd38a79da96195f2112d4ba37475d11cec`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed4111161b7b7d291c73883105977d83b95161ff3092cb8c51baa969a0f4f40`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefd93dcc118fc9b6c2575a0e2e6442cf1941ad36cd7c23a11ff37f954d72696`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 231.4 KB (231353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12465fe04c57bef25da7dd19448585a8f389a2be5002904390928db02803c463`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19ff97a8609ea6c7b399819d80dd69016ccd3db9c032fb36c9caaec3462cde`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9a5fa9635e3b3150a7fb86be203bd9ac800242a8715366e1ebf80137524c1d49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3422852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aac8ab48bba973ccd96958d6b1a6ead1c79dc7016524a07dc87240ccf918e9f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 13:39:51 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 13:39:53 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 13:39:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 13:40:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 13:40:08 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 13:40:09 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 13:40:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 13:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 13:40:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0194afa072d947a442ef104e10d9216659dfc8a0d66a1aa9d83dc2daa6d3cb60`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3636e065dbfa3ffe9e220f75a2656046c6e68daa308f669c824c33129da33d8e`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 7.8 KB (7776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6a06d391f6599e576cc221ab33e97777c1a2d34912c03b26bb42f42ba72ca`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 611.8 KB (611788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0000fde7d027d5e5be6d184daac6a936d889c009e92180fc9992b2e1b4385cc`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385151a4c23844070ef5830264bf1ee9abeb01f86bbb0c5dba45868ea8324f3c`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:47e6ca3b66046e043d8efb1996b3f02334b21d52d0378b9e70a9eee14bc8ba05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2809081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bb44b07872890902f462d8051264598233b2791b8d17ac8d1e9650682147605`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:49:57 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:49:59 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:49:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:50:06 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:50:06 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:50:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:50:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:50:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c21b0fe0ff4f5675555696be2fdd46dbd120c67b2a2a82d2f9358d673a2fddc`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faafadd95cb1b92a7217a5e1a180e88ffd0de612088f75c144bbf3d501585ff`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157d141feb67cd00e910527177fb9131596a73032d3f627e9160255a17512dc6`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 208.4 KB (208447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5180ea5424d8443b199fbe5a892596a2c6d2f9fff62a8e41bcc2a68035514`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda12945c53bd011c9f75619e916738acd26381a21194ab28a173176009878b0`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:ab6427d6903f8c26ed3da5c6bea858043a2043a6454daee528194faf1daa952b
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
$ docker pull spiped@sha256:8cd0d350e2a175da5f685212ca720cd31451daaa5c1c3ce22268a6c098628210
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0db056ae424f84934906f39c45bedff6339474a256240442fac553e048ab43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:25:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 14:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:25:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 14:26:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:26:06 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 14:26:06 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 14:26:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 14:26:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 14:26:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f05cfc98bdaab076eb82751252e3e75f04ba7cfe8574948694f75664ca08bd`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fbdb1be8384f98617d85b0a558459f05f31aec8a6f50df7182b1d0fbb9e01f`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17020edad6b1b0115116b35db60695f0f7ec88d5131069843c36bfc054d5863b`  
		Last Modified: Tue, 15 Nov 2022 14:26:24 GMT  
		Size: 6.0 MB (5998420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a563f1a79ce4f6624f04ac38760550529ab712ee4d46a3511ab645c054e6bbb`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a3a38d3e6c729c4b6d04992a60df1c5e4fd52f25f06a8708668e0568ebe22b`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:ec9790e3310ab830942f954fecd18dcd4a7fc78930eb5e9865b493c09d8de342
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f25e72bc7a8fea9ed51c48382332e6ad92a68e3821d104133619fe2a4ed8f376`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:18 GMT
ADD file:1949af7e583a1b54055a421129c32315fc101e53e2cda05da3171ed461bde0a6 in / 
# Tue, 15 Nov 2022 01:49:19 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:12:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 10:12:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:12:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 10:12:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 10:12:52 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 10:12:52 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 10:12:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 10:12:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:12:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b56836d864a6d857be3d12242b65962f2a2cf0d77c48cfb85bbbdf9d56a7e93d`  
		Last Modified: Tue, 15 Nov 2022 01:54:26 GMT  
		Size: 28.9 MB (28914126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52010eba05268403bb9ce16397f34a8d809c7d45381ed17d54727ec5312f8e64`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7f68ad0da9f44bae685b91c83e3125017b5e1fa894e902eb8af4059ec64232`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d61522f3adb083ae0c3a1100dd755cae1c3068f4615122d0d4d9fb9dcbd553b`  
		Last Modified: Tue, 15 Nov 2022 10:13:15 GMT  
		Size: 5.0 MB (5029291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382a079faf68aa665a39ca7ccb83043aa797d1c5ee7951f318b9c2bece18802b`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a4b4fabe7c1bacd9b9e252066f171608f18bc9125cae758db235ade53e961c`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bfff3efcf03753ba51d784c4deaee4cb8e634cede50272f622be6701a39e2c2e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31331482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed2d92b57a070235e7c98b6ba242d1cbd18b6492b75f763388eff3d53dc4d2e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 04:08:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Oct 2022 04:08:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 04:08:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Oct 2022 04:09:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Oct 2022 04:09:01 GMT
VOLUME [/spiped]
# Wed, 26 Oct 2022 04:09:01 GMT
WORKDIR /spiped
# Wed, 26 Oct 2022 04:09:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Oct 2022 04:09:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 04:09:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adf378b5b9701669a758188b83d55e929eb48bd4c543f9b8f8a431570a6711d`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c6587474e215654a49ffdca22b9d48921c15b50cf53a07d57670bb4caaf2cd`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b726e98a4dbc4add399728b2912edba24f9efb947fd81fd7e885e02c4ba50a`  
		Last Modified: Wed, 26 Oct 2022 04:09:54 GMT  
		Size: 4.7 MB (4749002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f830752e5f1c0df89505c43f8ee698e7b59e1a17aa5a93d366d0d83dc1d2d5d6`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce0b6a93edcda9a62223fb9e4977ef54baffc64715df9cfbbce9b2d943e9950`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:15446b678eff03a766ba070afd86b1b4b2b512383e7e86ae05bdbe35761d32cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960d815e93ee6a3ba5b7e52ef354ad4259e2ad94c8cdaee91366cdac33ce10d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:25:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:25:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:25:35 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:25:35 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:25:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f263b1855bd471c83539756f8b70a58c84c9dc0ff2dbcb682afdf46fa84af`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f63490a49f76c19d7c7411339c219429156afda6ef909fcb6e4aa90b7bcbc`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc90b9cb2517275e1ea4f6fa67c968e862002478d6945dd0a455d324aa9e9ef8`  
		Last Modified: Tue, 15 Nov 2022 13:25:56 GMT  
		Size: 5.3 MB (5272459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b17c3ba478f87caafa84a5a1a090060c3e18cf2ef8b7000dd0294fd8c425286`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bfbc8db5dc7db117e54b445680eb62aced5bdafa9c38b141250fc7aa7d5a8a`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:bc3034ea433bc46dd8c0b1f375517e13ebce3786f7ecbfffdb7edc99af6185f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe71f396ab173d0e7a95d9be87cd921b46ab02f959c0cbf70a4d5b39250f548e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 17:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 17:51:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 17:51:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 17:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 17:51:59 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 17:52:00 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 17:52:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 17:52:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 17:52:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fbdc019d80d6a30ab90868896498a28c5e819659f22bb2894d5fc2e7d6bb3f`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d64fbdfcaf79efbaf8da0d679f65709cf4066699e35b9fbb0029f30317bbf9`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1159f60b8a31090685214f0ae08d84535c724e5e92a2f79c4684a8af8435bdb`  
		Last Modified: Tue, 15 Nov 2022 17:52:34 GMT  
		Size: 7.9 MB (7890569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48a2b4bd1d2bd7ea1b36aea4ae7e36171af6be414a64513fdab695cf409fd0`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abba44a7b8700f9ac9dd0dba12b7983ecdc4c918ba4f8129e912828bd9b529`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:aac80a4c64529fa60afc110d64d0c85b6a568df1b7cb5a5a9ca9d5ac966ca456
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dad9d417652d7dc5fa4f1473c6a4076a1d44506ae13e748b502ed478db269`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 00:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 00:04:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:04:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 00:06:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 00:06:10 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 00:06:13 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 00:06:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 00:06:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 00:06:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423cc689eb0f49221096b6d78f2f88cde0b37b5c1b49367ebff22a6e1ee33ba`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff778c8a78825f7845b585d8dae3024757f98b009043b391253b9555d1bd3ee2`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9787dc2ceb548759ff582e8606939f449df9a0dd7ce05dc5d1722c52cb9feb0c`  
		Last Modified: Wed, 16 Nov 2022 00:06:51 GMT  
		Size: 5.7 MB (5706376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e18e00bc8e5f5bd8ded0d5c9a2d7e7ef1eddc72b6c9594971ecc6a5cd62c3d`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867e28a7d951478254c55c58be169d8812eaa99008aa6b11248a5c9046ae2f3`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:a4e046168feb1ad487131c35168c1565ab29cadfb409be2835dff56c857c96dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0760132dad5ee85c440e6c65bfb91e366f095c47c565a5c69bfc2730a81b81e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 05:18:45 GMT
ADD file:520926164fdc762143905745329e568c67289232bec450e48645d82a4613dccf in / 
# Tue, 15 Nov 2022 05:18:47 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 18:33:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 18:33:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 18:33:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 18:34:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 18:34:09 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 18:34:09 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 18:34:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 18:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 18:34:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c57913b7d0318ef1a47f0348ce54d9865316776aa1ffb2c7871b1473b3d29407`  
		Last Modified: Tue, 15 Nov 2022 05:24:22 GMT  
		Size: 35.3 MB (35285140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a5d9c14025c15f34163961f4eafc162696a33cc493eaa86dc0b54fa025e646`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddacb9148d8a6e8ce0f8dc4a7074198eea102ea0da570ce71824001314ec581`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a5572d4fe22794ba76d4bf209b17ff799559f885284884850d02580328ea93`  
		Last Modified: Tue, 15 Nov 2022 18:34:47 GMT  
		Size: 6.0 MB (5999748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42de0ee16e98c0a72bc01c622a96fa73c429fee856e55b597c7248a40335d900`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d7db34ebd9272908023a6993d28bbd615a3897bbba7d518beed99fbee7b30a`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:c473e05e698144dc8315ef89467944d3111b39a88bbad9963db8ab7843059b73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa617c4a5699ed04e207e266e667d59db1d726bba445409e8a648f5a6e4c18af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:14:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:14:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:14:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:15:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:15:44 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:15:45 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:15:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:15:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:15:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d0559b9988e98911430249fdef7b998e0b4c32305f0ccd4bcb8905987488be`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2b9a5754a77e47074f8f2ac4a0d9905ce7bd388dcb1f07ad8748af5ffc3e23`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7788cf8d0aadbaa693ab2c8e52e54631507aaac0f3a376941ec75476a67778a`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 5.2 MB (5188015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a9f1f79d29017e6e16df8a84cd6ca4120daaabd71eecb98fce0747916d094d`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d84d4f34ee0b4bc57bc91e1c4d2b9825b124f70fe19c92c828d01c7d9325a`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:82dced4a656b2d513450d2342ecddc3f9244f04c9c07a8565d1e90dd24b83259
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
$ docker pull spiped@sha256:88600bfd34359fe38ba773717d293fc4d6095338551ab0b9c98ced2944029635
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef58a68bf7b0e4e343f1c174cd34a75b21f0714a3fe9e5e50df70c1cb3313a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:31:09 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:31:10 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:31:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:31:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:31:21 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:31:21 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:31:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:31:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:31:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba143d89ef43493de610789b011ec6f78fd98311801bd1b895263425d2b80f9`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3bf49195ff499a5b7913c2890b39e1ca85bd2ba2fc46bdf7967974cdaa578`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 7.8 KB (7762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6bcd4c1d546b37c09f8d577cb9065b685c82b401a5f2271774cdf3a57f325e`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 221.2 KB (221203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e9846fbf23dbba2f28e731ca1a2b68957835ecbfe09de8fcecd43f01ce7312`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1bbea7f748e9071525f54078c4c1afed13fcad17509d2a56a430c21b8b56d5`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:4a97e4614d77053ba39fa5c745d6105a7715cb2a1339a25d4fa13a27d0d5b071
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef16808dbefc833d0994260a2717a0477aecef28d949a2bd4c8da571b5627b51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:28:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:28:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:28:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:28:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:28:26 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:28:26 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:28:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:28:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:28:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ad9b8c9f0b2df322f6b1cabda5e7ca816a4a3d899eb140b118c2827fddfe2`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2057d8252d211e7c1c7a5a22ff586d7ad6fb222a67ddc10c861346d2f5de70d7`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 7.8 KB (7761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7036cdcac704f3ec530ed23d018a37fa64b0d4e1ec8c26bd0388a1a2d99220d7`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 205.9 KB (205882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d603c20f7582181b49742ecc7a817667c6067b1e3ee6ec3e64ecbe1bf10206d0`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2d6b98135a7de547f76953f15d873bc47703d65c6f2c87b0a719561fb1066f`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:da26d167b81e6942d2bf840b15ff59a945c83bcb6c34968a2cb76d61b48368d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2627783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335ebf8c2444c91778b85ac23284d5a8bb8a0564755cb6ea06160705fc72ebfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:09:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:10:00 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:10:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:10:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:10:09 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:10:09 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:10:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:10:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:10:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adeca438422069f0b2d529c93aa015b2d66ff14e7f811a2db7155b3780f3f17`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a307f22f7b61faf288c16b2e278af2069d3f0f1d7ccb5de2669081f800b82595`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 7.8 KB (7766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ada82ce81437697e7bbaef8a8df96fe30079d2b62708af97071da84c0be91f`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 199.6 KB (199550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650ecac6d83dd8ac1473ff90545abe2e47ad63985de2031e7fb65a25c99847b2`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304511b2e0cd4c9408aace74412dcce1dcbb72f7cc52fa88e57892bfe2beae31`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cc37e731d1198e448359b790e73b2016b757e9d1a05425fa0a2df9fc6fe0cc9b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe1152848438c5b85156eb4f564f5a436e27d69210842e300de2be7c0bdf598`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 09:52:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 09:52:51 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 09:52:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 09:52:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 09:52:59 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 09:52:59 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 09:52:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 09:52:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 09:52:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a33d40b7aea60d797950562e12532c05e2bec1dfb8dc5431f8c871028f801d`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046893368895bc36323127bb34d70394b9e08715b8cd3609c1396fd7dcc7baad`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d84e6ac65d4649eecb08b3cb834f0b6205a88df39adc3099e196a2e03d066`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 214.6 KB (214567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7ee94c43226ce1cbb59b1a15b651a023be893f860642d7af91e0dbf49b0bdf`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053b7b3dc658bda7a53962394fac910f8408b95bc4066c9342ad508eb98fb56e`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:843ee0a06fce410e9185f279bedec495552d30a9b235351c9e52bd669095b6a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3049117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c9c942ec6bc7f10412698170c354b1c1e3784c5293bb45763683f9fae4ff45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:29:06 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 07:29:08 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 07:29:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 07:29:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 07:29:21 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 07:29:22 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 07:29:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 07:29:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 07:29:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d809fb6be6b6c5126ea93c77f723eabd38a79da96195f2112d4ba37475d11cec`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed4111161b7b7d291c73883105977d83b95161ff3092cb8c51baa969a0f4f40`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefd93dcc118fc9b6c2575a0e2e6442cf1941ad36cd7c23a11ff37f954d72696`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 231.4 KB (231353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12465fe04c57bef25da7dd19448585a8f389a2be5002904390928db02803c463`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19ff97a8609ea6c7b399819d80dd69016ccd3db9c032fb36c9caaec3462cde`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9a5fa9635e3b3150a7fb86be203bd9ac800242a8715366e1ebf80137524c1d49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3422852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aac8ab48bba973ccd96958d6b1a6ead1c79dc7016524a07dc87240ccf918e9f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 13:39:51 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 13:39:53 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 13:39:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 13:40:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 13:40:08 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 13:40:09 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 13:40:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 13:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 13:40:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0194afa072d947a442ef104e10d9216659dfc8a0d66a1aa9d83dc2daa6d3cb60`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3636e065dbfa3ffe9e220f75a2656046c6e68daa308f669c824c33129da33d8e`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 7.8 KB (7776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6a06d391f6599e576cc221ab33e97777c1a2d34912c03b26bb42f42ba72ca`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 611.8 KB (611788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0000fde7d027d5e5be6d184daac6a936d889c009e92180fc9992b2e1b4385cc`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385151a4c23844070ef5830264bf1ee9abeb01f86bbb0c5dba45868ea8324f3c`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:47e6ca3b66046e043d8efb1996b3f02334b21d52d0378b9e70a9eee14bc8ba05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2809081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bb44b07872890902f462d8051264598233b2791b8d17ac8d1e9650682147605`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:49:57 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:49:59 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:49:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:50:06 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:50:06 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:50:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:50:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:50:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c21b0fe0ff4f5675555696be2fdd46dbd120c67b2a2a82d2f9358d673a2fddc`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faafadd95cb1b92a7217a5e1a180e88ffd0de612088f75c144bbf3d501585ff`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157d141feb67cd00e910527177fb9131596a73032d3f627e9160255a17512dc6`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 208.4 KB (208447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5180ea5424d8443b199fbe5a892596a2c6d2f9fff62a8e41bcc2a68035514`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda12945c53bd011c9f75619e916738acd26381a21194ab28a173176009878b0`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:82dced4a656b2d513450d2342ecddc3f9244f04c9c07a8565d1e90dd24b83259
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
$ docker pull spiped@sha256:88600bfd34359fe38ba773717d293fc4d6095338551ab0b9c98ced2944029635
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef58a68bf7b0e4e343f1c174cd34a75b21f0714a3fe9e5e50df70c1cb3313a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:31:09 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:31:10 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:31:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:31:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:31:21 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:31:21 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:31:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:31:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:31:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba143d89ef43493de610789b011ec6f78fd98311801bd1b895263425d2b80f9`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3bf49195ff499a5b7913c2890b39e1ca85bd2ba2fc46bdf7967974cdaa578`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 7.8 KB (7762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6bcd4c1d546b37c09f8d577cb9065b685c82b401a5f2271774cdf3a57f325e`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 221.2 KB (221203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e9846fbf23dbba2f28e731ca1a2b68957835ecbfe09de8fcecd43f01ce7312`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1bbea7f748e9071525f54078c4c1afed13fcad17509d2a56a430c21b8b56d5`  
		Last Modified: Sat, 12 Nov 2022 08:31:36 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:4a97e4614d77053ba39fa5c745d6105a7715cb2a1339a25d4fa13a27d0d5b071
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef16808dbefc833d0994260a2717a0477aecef28d949a2bd4c8da571b5627b51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:28:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:28:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:28:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:28:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:28:26 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:28:26 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:28:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:28:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:28:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ad9b8c9f0b2df322f6b1cabda5e7ca816a4a3d899eb140b118c2827fddfe2`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2057d8252d211e7c1c7a5a22ff586d7ad6fb222a67ddc10c861346d2f5de70d7`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 7.8 KB (7761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7036cdcac704f3ec530ed23d018a37fa64b0d4e1ec8c26bd0388a1a2d99220d7`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 205.9 KB (205882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d603c20f7582181b49742ecc7a817667c6067b1e3ee6ec3e64ecbe1bf10206d0`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2d6b98135a7de547f76953f15d873bc47703d65c6f2c87b0a719561fb1066f`  
		Last Modified: Sat, 12 Nov 2022 08:28:46 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:da26d167b81e6942d2bf840b15ff59a945c83bcb6c34968a2cb76d61b48368d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2627783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335ebf8c2444c91778b85ac23284d5a8bb8a0564755cb6ea06160705fc72ebfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:09:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:10:00 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:10:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:10:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:10:09 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:10:09 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:10:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:10:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:10:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adeca438422069f0b2d529c93aa015b2d66ff14e7f811a2db7155b3780f3f17`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a307f22f7b61faf288c16b2e278af2069d3f0f1d7ccb5de2669081f800b82595`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 7.8 KB (7766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ada82ce81437697e7bbaef8a8df96fe30079d2b62708af97071da84c0be91f`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 199.6 KB (199550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650ecac6d83dd8ac1473ff90545abe2e47ad63985de2031e7fb65a25c99847b2`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304511b2e0cd4c9408aace74412dcce1dcbb72f7cc52fa88e57892bfe2beae31`  
		Last Modified: Sat, 12 Nov 2022 08:10:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cc37e731d1198e448359b790e73b2016b757e9d1a05425fa0a2df9fc6fe0cc9b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe1152848438c5b85156eb4f564f5a436e27d69210842e300de2be7c0bdf598`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 09:52:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 09:52:51 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 09:52:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 09:52:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 09:52:59 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 09:52:59 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 09:52:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 09:52:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 09:52:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a33d40b7aea60d797950562e12532c05e2bec1dfb8dc5431f8c871028f801d`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046893368895bc36323127bb34d70394b9e08715b8cd3609c1396fd7dcc7baad`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d84e6ac65d4649eecb08b3cb834f0b6205a88df39adc3099e196a2e03d066`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 214.6 KB (214567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7ee94c43226ce1cbb59b1a15b651a023be893f860642d7af91e0dbf49b0bdf`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053b7b3dc658bda7a53962394fac910f8408b95bc4066c9342ad508eb98fb56e`  
		Last Modified: Sat, 12 Nov 2022 09:53:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:843ee0a06fce410e9185f279bedec495552d30a9b235351c9e52bd669095b6a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3049117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c9c942ec6bc7f10412698170c354b1c1e3784c5293bb45763683f9fae4ff45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:29:06 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 07:29:08 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 07:29:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 07:29:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 07:29:21 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 07:29:22 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 07:29:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 07:29:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 07:29:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d809fb6be6b6c5126ea93c77f723eabd38a79da96195f2112d4ba37475d11cec`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed4111161b7b7d291c73883105977d83b95161ff3092cb8c51baa969a0f4f40`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefd93dcc118fc9b6c2575a0e2e6442cf1941ad36cd7c23a11ff37f954d72696`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 231.4 KB (231353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12465fe04c57bef25da7dd19448585a8f389a2be5002904390928db02803c463`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19ff97a8609ea6c7b399819d80dd69016ccd3db9c032fb36c9caaec3462cde`  
		Last Modified: Sat, 12 Nov 2022 07:29:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9a5fa9635e3b3150a7fb86be203bd9ac800242a8715366e1ebf80137524c1d49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3422852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aac8ab48bba973ccd96958d6b1a6ead1c79dc7016524a07dc87240ccf918e9f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 13:39:51 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 13:39:53 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 13:39:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 13:40:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 13:40:08 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 13:40:09 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 13:40:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 13:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 13:40:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0194afa072d947a442ef104e10d9216659dfc8a0d66a1aa9d83dc2daa6d3cb60`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3636e065dbfa3ffe9e220f75a2656046c6e68daa308f669c824c33129da33d8e`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 7.8 KB (7776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6a06d391f6599e576cc221ab33e97777c1a2d34912c03b26bb42f42ba72ca`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 611.8 KB (611788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0000fde7d027d5e5be6d184daac6a936d889c009e92180fc9992b2e1b4385cc`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385151a4c23844070ef5830264bf1ee9abeb01f86bbb0c5dba45868ea8324f3c`  
		Last Modified: Sat, 12 Nov 2022 13:40:42 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:47e6ca3b66046e043d8efb1996b3f02334b21d52d0378b9e70a9eee14bc8ba05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2809081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bb44b07872890902f462d8051264598233b2791b8d17ac8d1e9650682147605`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:49:57 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 12 Nov 2022 08:49:59 GMT
RUN apk add --no-cache libssl1.1
# Sat, 12 Nov 2022 08:49:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 12 Nov 2022 08:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:50:06 GMT
VOLUME [/spiped]
# Sat, 12 Nov 2022 08:50:06 GMT
WORKDIR /spiped
# Sat, 12 Nov 2022 08:50:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:50:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:50:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c21b0fe0ff4f5675555696be2fdd46dbd120c67b2a2a82d2f9358d673a2fddc`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faafadd95cb1b92a7217a5e1a180e88ffd0de612088f75c144bbf3d501585ff`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157d141feb67cd00e910527177fb9131596a73032d3f627e9160255a17512dc6`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 208.4 KB (208447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5180ea5424d8443b199fbe5a892596a2c6d2f9fff62a8e41bcc2a68035514`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda12945c53bd011c9f75619e916738acd26381a21194ab28a173176009878b0`  
		Last Modified: Sat, 12 Nov 2022 08:50:37 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:ab6427d6903f8c26ed3da5c6bea858043a2043a6454daee528194faf1daa952b
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
$ docker pull spiped@sha256:8cd0d350e2a175da5f685212ca720cd31451daaa5c1c3ce22268a6c098628210
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0db056ae424f84934906f39c45bedff6339474a256240442fac553e048ab43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:25:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 14:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:25:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 14:26:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:26:06 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 14:26:06 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 14:26:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 14:26:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 14:26:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f05cfc98bdaab076eb82751252e3e75f04ba7cfe8574948694f75664ca08bd`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fbdb1be8384f98617d85b0a558459f05f31aec8a6f50df7182b1d0fbb9e01f`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17020edad6b1b0115116b35db60695f0f7ec88d5131069843c36bfc054d5863b`  
		Last Modified: Tue, 15 Nov 2022 14:26:24 GMT  
		Size: 6.0 MB (5998420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a563f1a79ce4f6624f04ac38760550529ab712ee4d46a3511ab645c054e6bbb`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a3a38d3e6c729c4b6d04992a60df1c5e4fd52f25f06a8708668e0568ebe22b`  
		Last Modified: Tue, 15 Nov 2022 14:26:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:ec9790e3310ab830942f954fecd18dcd4a7fc78930eb5e9865b493c09d8de342
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f25e72bc7a8fea9ed51c48382332e6ad92a68e3821d104133619fe2a4ed8f376`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:18 GMT
ADD file:1949af7e583a1b54055a421129c32315fc101e53e2cda05da3171ed461bde0a6 in / 
# Tue, 15 Nov 2022 01:49:19 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:12:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 10:12:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:12:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 10:12:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 10:12:52 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 10:12:52 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 10:12:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 10:12:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:12:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b56836d864a6d857be3d12242b65962f2a2cf0d77c48cfb85bbbdf9d56a7e93d`  
		Last Modified: Tue, 15 Nov 2022 01:54:26 GMT  
		Size: 28.9 MB (28914126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52010eba05268403bb9ce16397f34a8d809c7d45381ed17d54727ec5312f8e64`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7f68ad0da9f44bae685b91c83e3125017b5e1fa894e902eb8af4059ec64232`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d61522f3adb083ae0c3a1100dd755cae1c3068f4615122d0d4d9fb9dcbd553b`  
		Last Modified: Tue, 15 Nov 2022 10:13:15 GMT  
		Size: 5.0 MB (5029291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382a079faf68aa665a39ca7ccb83043aa797d1c5ee7951f318b9c2bece18802b`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a4b4fabe7c1bacd9b9e252066f171608f18bc9125cae758db235ade53e961c`  
		Last Modified: Tue, 15 Nov 2022 10:13:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bfff3efcf03753ba51d784c4deaee4cb8e634cede50272f622be6701a39e2c2e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31331482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed2d92b57a070235e7c98b6ba242d1cbd18b6492b75f763388eff3d53dc4d2e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 04:08:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Oct 2022 04:08:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 04:08:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Oct 2022 04:09:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Oct 2022 04:09:01 GMT
VOLUME [/spiped]
# Wed, 26 Oct 2022 04:09:01 GMT
WORKDIR /spiped
# Wed, 26 Oct 2022 04:09:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Oct 2022 04:09:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 04:09:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adf378b5b9701669a758188b83d55e929eb48bd4c543f9b8f8a431570a6711d`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c6587474e215654a49ffdca22b9d48921c15b50cf53a07d57670bb4caaf2cd`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b726e98a4dbc4add399728b2912edba24f9efb947fd81fd7e885e02c4ba50a`  
		Last Modified: Wed, 26 Oct 2022 04:09:54 GMT  
		Size: 4.7 MB (4749002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f830752e5f1c0df89505c43f8ee698e7b59e1a17aa5a93d366d0d83dc1d2d5d6`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce0b6a93edcda9a62223fb9e4977ef54baffc64715df9cfbbce9b2d943e9950`  
		Last Modified: Wed, 26 Oct 2022 04:09:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:15446b678eff03a766ba070afd86b1b4b2b512383e7e86ae05bdbe35761d32cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960d815e93ee6a3ba5b7e52ef354ad4259e2ad94c8cdaee91366cdac33ce10d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:25:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:25:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:25:35 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:25:35 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:25:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f263b1855bd471c83539756f8b70a58c84c9dc0ff2dbcb682afdf46fa84af`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f63490a49f76c19d7c7411339c219429156afda6ef909fcb6e4aa90b7bcbc`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc90b9cb2517275e1ea4f6fa67c968e862002478d6945dd0a455d324aa9e9ef8`  
		Last Modified: Tue, 15 Nov 2022 13:25:56 GMT  
		Size: 5.3 MB (5272459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b17c3ba478f87caafa84a5a1a090060c3e18cf2ef8b7000dd0294fd8c425286`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bfbc8db5dc7db117e54b445680eb62aced5bdafa9c38b141250fc7aa7d5a8a`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:bc3034ea433bc46dd8c0b1f375517e13ebce3786f7ecbfffdb7edc99af6185f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe71f396ab173d0e7a95d9be87cd921b46ab02f959c0cbf70a4d5b39250f548e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 17:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 17:51:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 17:51:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 17:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 17:51:59 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 17:52:00 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 17:52:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 17:52:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 17:52:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fbdc019d80d6a30ab90868896498a28c5e819659f22bb2894d5fc2e7d6bb3f`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d64fbdfcaf79efbaf8da0d679f65709cf4066699e35b9fbb0029f30317bbf9`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1159f60b8a31090685214f0ae08d84535c724e5e92a2f79c4684a8af8435bdb`  
		Last Modified: Tue, 15 Nov 2022 17:52:34 GMT  
		Size: 7.9 MB (7890569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48a2b4bd1d2bd7ea1b36aea4ae7e36171af6be414a64513fdab695cf409fd0`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abba44a7b8700f9ac9dd0dba12b7983ecdc4c918ba4f8129e912828bd9b529`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:aac80a4c64529fa60afc110d64d0c85b6a568df1b7cb5a5a9ca9d5ac966ca456
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dad9d417652d7dc5fa4f1473c6a4076a1d44506ae13e748b502ed478db269`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 00:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 00:04:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:04:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 00:06:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 00:06:10 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 00:06:13 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 00:06:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 00:06:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 00:06:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423cc689eb0f49221096b6d78f2f88cde0b37b5c1b49367ebff22a6e1ee33ba`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff778c8a78825f7845b585d8dae3024757f98b009043b391253b9555d1bd3ee2`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9787dc2ceb548759ff582e8606939f449df9a0dd7ce05dc5d1722c52cb9feb0c`  
		Last Modified: Wed, 16 Nov 2022 00:06:51 GMT  
		Size: 5.7 MB (5706376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e18e00bc8e5f5bd8ded0d5c9a2d7e7ef1eddc72b6c9594971ecc6a5cd62c3d`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867e28a7d951478254c55c58be169d8812eaa99008aa6b11248a5c9046ae2f3`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:a4e046168feb1ad487131c35168c1565ab29cadfb409be2835dff56c857c96dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0760132dad5ee85c440e6c65bfb91e366f095c47c565a5c69bfc2730a81b81e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 05:18:45 GMT
ADD file:520926164fdc762143905745329e568c67289232bec450e48645d82a4613dccf in / 
# Tue, 15 Nov 2022 05:18:47 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 18:33:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 18:33:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 18:33:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 18:34:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 18:34:09 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 18:34:09 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 18:34:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 18:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 18:34:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c57913b7d0318ef1a47f0348ce54d9865316776aa1ffb2c7871b1473b3d29407`  
		Last Modified: Tue, 15 Nov 2022 05:24:22 GMT  
		Size: 35.3 MB (35285140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a5d9c14025c15f34163961f4eafc162696a33cc493eaa86dc0b54fa025e646`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddacb9148d8a6e8ce0f8dc4a7074198eea102ea0da570ce71824001314ec581`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a5572d4fe22794ba76d4bf209b17ff799559f885284884850d02580328ea93`  
		Last Modified: Tue, 15 Nov 2022 18:34:47 GMT  
		Size: 6.0 MB (5999748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42de0ee16e98c0a72bc01c622a96fa73c429fee856e55b597c7248a40335d900`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d7db34ebd9272908023a6993d28bbd615a3897bbba7d518beed99fbee7b30a`  
		Last Modified: Tue, 15 Nov 2022 18:34:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:c473e05e698144dc8315ef89467944d3111b39a88bbad9963db8ab7843059b73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa617c4a5699ed04e207e266e667d59db1d726bba445409e8a648f5a6e4c18af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:14:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:14:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:14:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:15:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:15:44 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:15:45 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:15:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:15:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:15:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d0559b9988e98911430249fdef7b998e0b4c32305f0ccd4bcb8905987488be`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2b9a5754a77e47074f8f2ac4a0d9905ce7bd388dcb1f07ad8748af5ffc3e23`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7788cf8d0aadbaa693ab2c8e52e54631507aaac0f3a376941ec75476a67778a`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 5.2 MB (5188015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a9f1f79d29017e6e16df8a84cd6ca4120daaabd71eecb98fce0747916d094d`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d84d4f34ee0b4bc57bc91e1c4d2b9825b124f70fe19c92c828d01c7d9325a`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
