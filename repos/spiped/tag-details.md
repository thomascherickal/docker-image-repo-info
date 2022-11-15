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
$ docker pull spiped@sha256:f9ebe35a78b626a6cdeb4e138bed50918bbaafca6b5d09ff2d37ab4fc1959af9
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
$ docker pull spiped@sha256:907ddd7d8a3f64e3b9587d8bd37803871c7e0301273fd134fff16a4601b764b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37421712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aebdf10111eb9350e84131fa07f10b1e016fae20fb35a2ef3054aac040d9ad51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:37:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 08:37:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:37:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 08:37:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:37:30 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 08:37:30 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 08:37:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 08:37:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 08:37:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee0ea61d941875664cd9c05776da1213111ea724a574da76b9b28c4b8f4528c`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d4fedc70099c8ce233b3659781b1aed74d64581846c692bb49290d355171b7`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16e54acaf0e36c17b7f590939d1cb4ad9b02cb94f13fb00f9f7b86745abe48b`  
		Last Modified: Tue, 25 Oct 2022 08:37:48 GMT  
		Size: 6.0 MB (5998416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56db037880c16bf262262d7370497379e30b11b3fd0281edee6eb60a36552277`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6a4030f16578da977873b98ae987b7321fb1952c6375b4fce536030b6e5836`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:6b101ec27a5ae8f320604e0cf0e9546c392ad8d8065545353a1fba58298c7ed0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40289909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75dd3c8b180ee6f7e59a56438dfed96642932fd382c54a203437c206d8caff1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 11:34:51 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 11:34:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 11:34:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 11:35:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 11:35:16 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 11:35:17 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 11:35:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 11:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 11:35:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ed83e739e0a2df94abb07b64af6442cadc8604341a6c92d12553b1d016f22a`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e27fa8cbddf583608745d18bb43feaabff04c2588b9e1c1f94bb325a4c7ec4b`  
		Last Modified: Tue, 25 Oct 2022 11:35:51 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cf74edda461ba871a76c19f77e0ef97044be562ccb1c8d61a75b94e13d1ae6`  
		Last Modified: Tue, 25 Oct 2022 11:35:52 GMT  
		Size: 7.9 MB (7890559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acddd776b18a97632e23e0bf36ae521a40f00274c77cbf7c76b00f91e5f6f553`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3c0fbbbfa9f279ecb2c1951b886b9105fce2f77f710b00db682fa3f411cead`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:00fc981d65507228c242aa4bdb4e1fc6139afcebba2683c34743dc496e8077dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35350067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:155db8255c6ac9a079e7228c64edb0119d3255a4b23a67a8f19dba64c69677e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 04:39:25 GMT
ADD file:222c5611b805658925ba615b0e69d40aa3dfa37223bc06f150909f7e944e426b in / 
# Tue, 25 Oct 2022 04:39:29 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:57:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Oct 2022 05:57:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:57:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Oct 2022 05:58:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Oct 2022 05:58:56 GMT
VOLUME [/spiped]
# Wed, 26 Oct 2022 05:58:59 GMT
WORKDIR /spiped
# Wed, 26 Oct 2022 05:59:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Oct 2022 05:59:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 05:59:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:85f344f7fa0587aa4dbdc8d09d838d444853a1789047586a0927fa09fa89bb8f`  
		Last Modified: Tue, 25 Oct 2022 04:47:25 GMT  
		Size: 29.6 MB (29640590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690b2de19d8b758195a521ea98837b08f3b18bdeaf8e13fc48ad6981b3cb258c`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81aa4e5e1cfa28f7d8b4b77fadcb3b868b50c1dfb9509742f11a31583e80ae8b`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4cab88bca13a73ee16be74d5b6954fd7cc493932eae28211d1d38c59ff45bb`  
		Last Modified: Wed, 26 Oct 2022 05:59:23 GMT  
		Size: 5.7 MB (5706496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7037feb4132dd15404ae3b7a88c848f4902ea7eeea1adac94169bcc3beaf513e`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a68cac1944e8fd353746991422bc9603c5623d12f599ec437cb5d1d4d2524aa`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:4f8c40985efdc328896edd611d5078c2fc2702512fb7dbf8313b4cae3921a64e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddf972f162417a391365ea02bd55cac90c31e91cea94cde3b1785dc4e07b862c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:56:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 08:56:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:56:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 08:57:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:57:30 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 08:57:30 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 08:57:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 08:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 08:57:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72bcd36564076a1be5059203c37728b7870c126ac7fe06f996ccf16f91855f`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fe46109a02177cec27f93ac157701520a7bb241f376b25305d5d3066a0e344`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c94efcdf110ae18400e5415ff3d6b9e3922164053912c50c55ba08357401ef6`  
		Last Modified: Tue, 25 Oct 2022 08:58:02 GMT  
		Size: 6.0 MB (5999635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf8c734f5fda4c57a8d654d651fd56402b97e7bb5e2ebb9765410fc9b4ebbf`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93111314cb3af703e6ce8c0a09396a4c6e0294ef4a359f1946bbaf70c6ab0b50`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:f9ebe35a78b626a6cdeb4e138bed50918bbaafca6b5d09ff2d37ab4fc1959af9
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
$ docker pull spiped@sha256:907ddd7d8a3f64e3b9587d8bd37803871c7e0301273fd134fff16a4601b764b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37421712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aebdf10111eb9350e84131fa07f10b1e016fae20fb35a2ef3054aac040d9ad51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:37:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 08:37:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:37:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 08:37:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:37:30 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 08:37:30 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 08:37:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 08:37:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 08:37:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee0ea61d941875664cd9c05776da1213111ea724a574da76b9b28c4b8f4528c`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d4fedc70099c8ce233b3659781b1aed74d64581846c692bb49290d355171b7`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16e54acaf0e36c17b7f590939d1cb4ad9b02cb94f13fb00f9f7b86745abe48b`  
		Last Modified: Tue, 25 Oct 2022 08:37:48 GMT  
		Size: 6.0 MB (5998416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56db037880c16bf262262d7370497379e30b11b3fd0281edee6eb60a36552277`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6a4030f16578da977873b98ae987b7321fb1952c6375b4fce536030b6e5836`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:6b101ec27a5ae8f320604e0cf0e9546c392ad8d8065545353a1fba58298c7ed0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40289909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75dd3c8b180ee6f7e59a56438dfed96642932fd382c54a203437c206d8caff1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 11:34:51 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 11:34:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 11:34:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 11:35:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 11:35:16 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 11:35:17 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 11:35:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 11:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 11:35:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ed83e739e0a2df94abb07b64af6442cadc8604341a6c92d12553b1d016f22a`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e27fa8cbddf583608745d18bb43feaabff04c2588b9e1c1f94bb325a4c7ec4b`  
		Last Modified: Tue, 25 Oct 2022 11:35:51 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cf74edda461ba871a76c19f77e0ef97044be562ccb1c8d61a75b94e13d1ae6`  
		Last Modified: Tue, 25 Oct 2022 11:35:52 GMT  
		Size: 7.9 MB (7890559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acddd776b18a97632e23e0bf36ae521a40f00274c77cbf7c76b00f91e5f6f553`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3c0fbbbfa9f279ecb2c1951b886b9105fce2f77f710b00db682fa3f411cead`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:00fc981d65507228c242aa4bdb4e1fc6139afcebba2683c34743dc496e8077dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35350067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:155db8255c6ac9a079e7228c64edb0119d3255a4b23a67a8f19dba64c69677e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 04:39:25 GMT
ADD file:222c5611b805658925ba615b0e69d40aa3dfa37223bc06f150909f7e944e426b in / 
# Tue, 25 Oct 2022 04:39:29 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:57:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Oct 2022 05:57:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:57:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Oct 2022 05:58:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Oct 2022 05:58:56 GMT
VOLUME [/spiped]
# Wed, 26 Oct 2022 05:58:59 GMT
WORKDIR /spiped
# Wed, 26 Oct 2022 05:59:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Oct 2022 05:59:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 05:59:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:85f344f7fa0587aa4dbdc8d09d838d444853a1789047586a0927fa09fa89bb8f`  
		Last Modified: Tue, 25 Oct 2022 04:47:25 GMT  
		Size: 29.6 MB (29640590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690b2de19d8b758195a521ea98837b08f3b18bdeaf8e13fc48ad6981b3cb258c`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81aa4e5e1cfa28f7d8b4b77fadcb3b868b50c1dfb9509742f11a31583e80ae8b`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4cab88bca13a73ee16be74d5b6954fd7cc493932eae28211d1d38c59ff45bb`  
		Last Modified: Wed, 26 Oct 2022 05:59:23 GMT  
		Size: 5.7 MB (5706496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7037feb4132dd15404ae3b7a88c848f4902ea7eeea1adac94169bcc3beaf513e`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a68cac1944e8fd353746991422bc9603c5623d12f599ec437cb5d1d4d2524aa`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:4f8c40985efdc328896edd611d5078c2fc2702512fb7dbf8313b4cae3921a64e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddf972f162417a391365ea02bd55cac90c31e91cea94cde3b1785dc4e07b862c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:56:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 08:56:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:56:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 08:57:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:57:30 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 08:57:30 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 08:57:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 08:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 08:57:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72bcd36564076a1be5059203c37728b7870c126ac7fe06f996ccf16f91855f`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fe46109a02177cec27f93ac157701520a7bb241f376b25305d5d3066a0e344`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c94efcdf110ae18400e5415ff3d6b9e3922164053912c50c55ba08357401ef6`  
		Last Modified: Tue, 25 Oct 2022 08:58:02 GMT  
		Size: 6.0 MB (5999635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf8c734f5fda4c57a8d654d651fd56402b97e7bb5e2ebb9765410fc9b4ebbf`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93111314cb3af703e6ce8c0a09396a4c6e0294ef4a359f1946bbaf70c6ab0b50`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:f9ebe35a78b626a6cdeb4e138bed50918bbaafca6b5d09ff2d37ab4fc1959af9
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
$ docker pull spiped@sha256:907ddd7d8a3f64e3b9587d8bd37803871c7e0301273fd134fff16a4601b764b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37421712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aebdf10111eb9350e84131fa07f10b1e016fae20fb35a2ef3054aac040d9ad51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:37:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 08:37:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:37:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 08:37:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:37:30 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 08:37:30 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 08:37:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 08:37:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 08:37:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee0ea61d941875664cd9c05776da1213111ea724a574da76b9b28c4b8f4528c`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d4fedc70099c8ce233b3659781b1aed74d64581846c692bb49290d355171b7`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16e54acaf0e36c17b7f590939d1cb4ad9b02cb94f13fb00f9f7b86745abe48b`  
		Last Modified: Tue, 25 Oct 2022 08:37:48 GMT  
		Size: 6.0 MB (5998416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56db037880c16bf262262d7370497379e30b11b3fd0281edee6eb60a36552277`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6a4030f16578da977873b98ae987b7321fb1952c6375b4fce536030b6e5836`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:6b101ec27a5ae8f320604e0cf0e9546c392ad8d8065545353a1fba58298c7ed0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40289909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75dd3c8b180ee6f7e59a56438dfed96642932fd382c54a203437c206d8caff1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 11:34:51 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 11:34:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 11:34:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 11:35:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 11:35:16 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 11:35:17 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 11:35:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 11:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 11:35:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ed83e739e0a2df94abb07b64af6442cadc8604341a6c92d12553b1d016f22a`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e27fa8cbddf583608745d18bb43feaabff04c2588b9e1c1f94bb325a4c7ec4b`  
		Last Modified: Tue, 25 Oct 2022 11:35:51 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cf74edda461ba871a76c19f77e0ef97044be562ccb1c8d61a75b94e13d1ae6`  
		Last Modified: Tue, 25 Oct 2022 11:35:52 GMT  
		Size: 7.9 MB (7890559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acddd776b18a97632e23e0bf36ae521a40f00274c77cbf7c76b00f91e5f6f553`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3c0fbbbfa9f279ecb2c1951b886b9105fce2f77f710b00db682fa3f411cead`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:00fc981d65507228c242aa4bdb4e1fc6139afcebba2683c34743dc496e8077dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35350067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:155db8255c6ac9a079e7228c64edb0119d3255a4b23a67a8f19dba64c69677e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 04:39:25 GMT
ADD file:222c5611b805658925ba615b0e69d40aa3dfa37223bc06f150909f7e944e426b in / 
# Tue, 25 Oct 2022 04:39:29 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:57:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Oct 2022 05:57:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:57:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Oct 2022 05:58:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Oct 2022 05:58:56 GMT
VOLUME [/spiped]
# Wed, 26 Oct 2022 05:58:59 GMT
WORKDIR /spiped
# Wed, 26 Oct 2022 05:59:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Oct 2022 05:59:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 05:59:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:85f344f7fa0587aa4dbdc8d09d838d444853a1789047586a0927fa09fa89bb8f`  
		Last Modified: Tue, 25 Oct 2022 04:47:25 GMT  
		Size: 29.6 MB (29640590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690b2de19d8b758195a521ea98837b08f3b18bdeaf8e13fc48ad6981b3cb258c`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81aa4e5e1cfa28f7d8b4b77fadcb3b868b50c1dfb9509742f11a31583e80ae8b`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4cab88bca13a73ee16be74d5b6954fd7cc493932eae28211d1d38c59ff45bb`  
		Last Modified: Wed, 26 Oct 2022 05:59:23 GMT  
		Size: 5.7 MB (5706496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7037feb4132dd15404ae3b7a88c848f4902ea7eeea1adac94169bcc3beaf513e`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a68cac1944e8fd353746991422bc9603c5623d12f599ec437cb5d1d4d2524aa`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:4f8c40985efdc328896edd611d5078c2fc2702512fb7dbf8313b4cae3921a64e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddf972f162417a391365ea02bd55cac90c31e91cea94cde3b1785dc4e07b862c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:56:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 08:56:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:56:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 08:57:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:57:30 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 08:57:30 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 08:57:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 08:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 08:57:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72bcd36564076a1be5059203c37728b7870c126ac7fe06f996ccf16f91855f`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fe46109a02177cec27f93ac157701520a7bb241f376b25305d5d3066a0e344`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c94efcdf110ae18400e5415ff3d6b9e3922164053912c50c55ba08357401ef6`  
		Last Modified: Tue, 25 Oct 2022 08:58:02 GMT  
		Size: 6.0 MB (5999635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf8c734f5fda4c57a8d654d651fd56402b97e7bb5e2ebb9765410fc9b4ebbf`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93111314cb3af703e6ce8c0a09396a4c6e0294ef4a359f1946bbaf70c6ab0b50`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:f9ebe35a78b626a6cdeb4e138bed50918bbaafca6b5d09ff2d37ab4fc1959af9
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
$ docker pull spiped@sha256:907ddd7d8a3f64e3b9587d8bd37803871c7e0301273fd134fff16a4601b764b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37421712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aebdf10111eb9350e84131fa07f10b1e016fae20fb35a2ef3054aac040d9ad51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:37:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 08:37:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:37:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 08:37:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:37:30 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 08:37:30 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 08:37:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 08:37:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 08:37:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee0ea61d941875664cd9c05776da1213111ea724a574da76b9b28c4b8f4528c`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d4fedc70099c8ce233b3659781b1aed74d64581846c692bb49290d355171b7`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16e54acaf0e36c17b7f590939d1cb4ad9b02cb94f13fb00f9f7b86745abe48b`  
		Last Modified: Tue, 25 Oct 2022 08:37:48 GMT  
		Size: 6.0 MB (5998416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56db037880c16bf262262d7370497379e30b11b3fd0281edee6eb60a36552277`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6a4030f16578da977873b98ae987b7321fb1952c6375b4fce536030b6e5836`  
		Last Modified: Tue, 25 Oct 2022 08:37:47 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:6b101ec27a5ae8f320604e0cf0e9546c392ad8d8065545353a1fba58298c7ed0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40289909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75dd3c8b180ee6f7e59a56438dfed96642932fd382c54a203437c206d8caff1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 11:34:51 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 11:34:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 11:34:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 11:35:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 11:35:16 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 11:35:17 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 11:35:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 11:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 11:35:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ed83e739e0a2df94abb07b64af6442cadc8604341a6c92d12553b1d016f22a`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e27fa8cbddf583608745d18bb43feaabff04c2588b9e1c1f94bb325a4c7ec4b`  
		Last Modified: Tue, 25 Oct 2022 11:35:51 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cf74edda461ba871a76c19f77e0ef97044be562ccb1c8d61a75b94e13d1ae6`  
		Last Modified: Tue, 25 Oct 2022 11:35:52 GMT  
		Size: 7.9 MB (7890559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acddd776b18a97632e23e0bf36ae521a40f00274c77cbf7c76b00f91e5f6f553`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3c0fbbbfa9f279ecb2c1951b886b9105fce2f77f710b00db682fa3f411cead`  
		Last Modified: Tue, 25 Oct 2022 11:35:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:00fc981d65507228c242aa4bdb4e1fc6139afcebba2683c34743dc496e8077dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35350067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:155db8255c6ac9a079e7228c64edb0119d3255a4b23a67a8f19dba64c69677e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 04:39:25 GMT
ADD file:222c5611b805658925ba615b0e69d40aa3dfa37223bc06f150909f7e944e426b in / 
# Tue, 25 Oct 2022 04:39:29 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:57:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Oct 2022 05:57:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:57:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Oct 2022 05:58:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Oct 2022 05:58:56 GMT
VOLUME [/spiped]
# Wed, 26 Oct 2022 05:58:59 GMT
WORKDIR /spiped
# Wed, 26 Oct 2022 05:59:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Oct 2022 05:59:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 05:59:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:85f344f7fa0587aa4dbdc8d09d838d444853a1789047586a0927fa09fa89bb8f`  
		Last Modified: Tue, 25 Oct 2022 04:47:25 GMT  
		Size: 29.6 MB (29640590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690b2de19d8b758195a521ea98837b08f3b18bdeaf8e13fc48ad6981b3cb258c`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81aa4e5e1cfa28f7d8b4b77fadcb3b868b50c1dfb9509742f11a31583e80ae8b`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4cab88bca13a73ee16be74d5b6954fd7cc493932eae28211d1d38c59ff45bb`  
		Last Modified: Wed, 26 Oct 2022 05:59:23 GMT  
		Size: 5.7 MB (5706496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7037feb4132dd15404ae3b7a88c848f4902ea7eeea1adac94169bcc3beaf513e`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a68cac1944e8fd353746991422bc9603c5623d12f599ec437cb5d1d4d2524aa`  
		Last Modified: Wed, 26 Oct 2022 05:59:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:4f8c40985efdc328896edd611d5078c2fc2702512fb7dbf8313b4cae3921a64e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddf972f162417a391365ea02bd55cac90c31e91cea94cde3b1785dc4e07b862c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:56:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 25 Oct 2022 08:56:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:56:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 25 Oct 2022 08:57:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 25 Oct 2022 08:57:30 GMT
VOLUME [/spiped]
# Tue, 25 Oct 2022 08:57:30 GMT
WORKDIR /spiped
# Tue, 25 Oct 2022 08:57:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 25 Oct 2022 08:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 08:57:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72bcd36564076a1be5059203c37728b7870c126ac7fe06f996ccf16f91855f`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fe46109a02177cec27f93ac157701520a7bb241f376b25305d5d3066a0e344`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c94efcdf110ae18400e5415ff3d6b9e3922164053912c50c55ba08357401ef6`  
		Last Modified: Tue, 25 Oct 2022 08:58:02 GMT  
		Size: 6.0 MB (5999635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf8c734f5fda4c57a8d654d651fd56402b97e7bb5e2ebb9765410fc9b4ebbf`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93111314cb3af703e6ce8c0a09396a4c6e0294ef4a359f1946bbaf70c6ab0b50`  
		Last Modified: Tue, 25 Oct 2022 08:58:00 GMT  
		Size: 339.0 B  
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
