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
$ docker pull spiped@sha256:3051fd2111d842b48252f722a94c75dbf39dd094a5f3be71676cf84f3a285896
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
$ docker pull spiped@sha256:6e56f898cffedf314d7e78c36169a3c82a3cecb7b3eabcae761df786ffcfa776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37404848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a5c88f0c911b4337a918ef32508daa452d712618d486a0160cd5793cd361ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 12:26:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 12:26:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 12:26:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 12:26:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 12:26:34 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 12:26:34 GMT
WORKDIR /spiped
# Tue, 23 May 2023 12:26:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 12:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 12:26:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ec67773fceb5d595bfdd899df865f6dba186d457790bcbb5651bc6cc99d90d`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843a0deb718885d4a7ec0829e15e29d5bf108522d62cb859c1ea655b40de7c37`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37406cfa1e5f43875100dd643b4ffe1d3d94166b88ca9c89e45c85f9836f4f3f`  
		Last Modified: Tue, 23 May 2023 12:26:50 GMT  
		Size: 6.0 MB (5998006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1da50da921d37b3dd928ff99cbe7041e472193b33f8e7a363565f0918192396`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e68bb6f8c79f1122c9447e56b77fc1f1f33701394359d7da671620d33ea690`  
		Last Modified: Tue, 23 May 2023 12:26:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:49ed0f173e4fcb9fd6bd56651f254b8dfa6b3aed0e1a42f93f166bc8f2226655
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33935055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1db0534cd6253a7850d8a6035c7dca53b22cf72cb2ad369c5cc20375a302343`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:48:41 GMT
ADD file:868f634f5ddb80ed9e9c719ccaf5d564d96fe819f0b000ecc734311baf5da99b in / 
# Tue, 23 May 2023 00:48:42 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:08:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 01:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:08:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 01:09:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:09:25 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 01:09:25 GMT
WORKDIR /spiped
# Tue, 23 May 2023 01:09:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 01:09:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:812967ccba449e7a96044b2d48ffc62816b22eb17641844c4dfffbe3b3ec6f21`  
		Last Modified: Tue, 23 May 2023 00:51:19 GMT  
		Size: 28.9 MB (28903411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce835c01736d996228e733dc5e9ddc64fcaa06d162232eae144c1a997a0e89b3`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354077a571b20fe4e85fcd0dbe7f8ef2f92c66b05eae053b9d9b9a59e99e814`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e5170f406fb5ebb782e8c048c3b0dc057ca5f19b4c4fa9d2fb512b9679350f`  
		Last Modified: Tue, 23 May 2023 01:09:37 GMT  
		Size: 5.0 MB (5028397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca08ae3499842a4a09ebb9ce9ea5344fb0f8a28fa563c97aea66ebc4512d6c7`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8877754d946fb8eef9f97dfae22bbf5f50e90791a8118e6f200475f033e247`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2b9b51f2747566b62f99f3285ba2b22426a10480dcda2197906482f9caa1fc6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31316045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12235c47b83e4e541a5cb08eddccde28158ca3115c91c99a636bbfaad8fda42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:49:41 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 09:49:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 09:49:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 09:50:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 09:50:08 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 09:50:08 GMT
WORKDIR /spiped
# Tue, 23 May 2023 09:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 09:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 09:50:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e366a5a086c832200cf0079c021df977cbf4af1f1bacc5836c38ca9e4fb0801`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26db70e43f87da848b7e77ab58c78d0a9f5df4ea0796fccdf2ff18c5cd8e770`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6b5e5b595b275c3cae346bc7bd81e46d03327fe80e02b279a395a7a94d10f9`  
		Last Modified: Tue, 23 May 2023 09:50:23 GMT  
		Size: 4.7 MB (4748156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c1114f756402ee5152fce302822c514afa5908c89b694fb31c688c1412955`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fde6856633e2275a7b963cf3d0dbe22d60395a4bc9d2c9f197bb10db5f5ff2a`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8a5154f80fcd5049f56d81eaa5fa39c4fd82721f5cc583b6d14bdb7e1b23731f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35326914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7da60844d4229ac6dffb12604f36f1438e8ff4ed0546651f6ba44ab83acc7c28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:20:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 07:20:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:20:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 07:20:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 07:20:57 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 07:20:57 GMT
WORKDIR /spiped
# Tue, 23 May 2023 07:20:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 07:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 07:20:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa8f6bfb1c027bb9f657161080f0ab93d19eebc194113b874d055fdcbfcb460`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47a57eada7dc6536f84b1b4335e54a33593d6eb7ec21e4d1033d6ad1e0a86e7`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e3fff08fa9daa5729dace8c989618277b41785008308f87afcc87e10c5bbb4`  
		Last Modified: Tue, 23 May 2023 07:21:11 GMT  
		Size: 5.3 MB (5270912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c03b1322313f66b8edacbb1f3daf86f76fa0bcf2461f8e9b1c8b0182c569c41`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bce57662b8b31a2ce6d26052524b37aa0e54ae5e585421cd7bd6202e7219607`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:c86f183f59a1da0d47a0ef90433af289f2f2b7c2d833a89316c34d51afe2d0f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40282845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6185bc58ac223183e9461e6107bae7b0e9ca3bbb4338869c1f863ab9c624fa13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:51:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 01:51:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:51:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 01:51:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:51:43 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 01:51:43 GMT
WORKDIR /spiped
# Tue, 23 May 2023 01:51:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 01:51:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 01:51:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9100966936a8c84c9e0e8b57d0811fb36e0e2c2d3e1138a0d3a7a918fe6745c9`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57610b2efa5f7c48f7d1ab161334a38849ff14c70658cb48567036e35e685b91`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1302ffc3a0d553d137a506717f8c2741436b82ff5b23b4353023fc9a35cd98`  
		Last Modified: Tue, 23 May 2023 01:52:01 GMT  
		Size: 7.9 MB (7891426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed28e099af4805a76b58eb4139bf498ac46acfb4d643ec70c9b840eb827750fb`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab03d42d20f08b827cfa1c2ef42e597ffbd8333e2237fa7167ad56119457fbb`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:5048eca6297857f351909c330a9a32c045a8a5656f8a306773cd773ed026ca87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69bb2dc15afa48fd2a905c1b95630d24cb02183dd2e42a0aea1139444f8b2e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 00:10:34 GMT
ADD file:4d5c7737e954f157e3d7ea47cc1814c46ec5c753a3d5d828ad9614969b572253 in / 
# Tue, 13 Jun 2023 00:10:38 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:43:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Jun 2023 01:43:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:43:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Jun 2023 01:45:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:45:14 GMT
VOLUME [/spiped]
# Tue, 13 Jun 2023 01:45:17 GMT
WORKDIR /spiped
# Tue, 13 Jun 2023 01:45:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:45:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 01:45:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:61bd6562a93acd0a3b327321e5465408e1d921b3ce1fb4fe353633330c3ede91`  
		Last Modified: Tue, 13 Jun 2023 00:23:53 GMT  
		Size: 29.6 MB (29634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f0ef0a3861267b4ef08cf448b2f1fc3ade81711b0b5fbd9d6d1581d6d8444f`  
		Last Modified: Tue, 13 Jun 2023 01:45:38 GMT  
		Size: 1.6 KB (1607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46baf526b17f9846cc40a9942d857383066be6d7b9a763ad5fffe1d117d59b3`  
		Last Modified: Tue, 13 Jun 2023 01:45:37 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b277e66890f62e701bf366cadb6b71924c5cb7a1a7286555f99f64fe3b06207`  
		Last Modified: Tue, 13 Jun 2023 01:45:42 GMT  
		Size: 5.7 MB (5705100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fd55e3c4b14927f26b90efaa6ce8242e295488d2b3bba74d8fb002479f80b0`  
		Last Modified: Tue, 13 Jun 2023 01:45:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23161a5a3690af3fa56d7600a2430fad04ac37a3c42eebf022ebd04cc427fb5`  
		Last Modified: Tue, 13 Jun 2023 01:45:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:e26c208c4a4342785c225a1004342e0114c3561ce9b1530544a567b47005086e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41284428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c610878704350416c6e781ffc11dc286e43f4fd60173a4e237e7855a91d0ebb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 10:48:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 10:49:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 10:49:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 10:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 10:49:49 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 10:49:49 GMT
WORKDIR /spiped
# Tue, 23 May 2023 10:49:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 10:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 10:49:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f4a119486e3fcedd3af8f31d52c720861f5cacee89269ad7e0be2c0ab48eed`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b52a815f8a92c8687a8959408e5922807bf95c0905f55a535f52551bf75e6a`  
		Last Modified: Tue, 23 May 2023 10:50:07 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b713f962480fbb84f8dd9a119a34339176e1e324df77251b08080ff5c51f96`  
		Last Modified: Tue, 23 May 2023 10:50:10 GMT  
		Size: 6.0 MB (6000259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d48bbdef4e3e839c97da555fe50a2684844e5f2050859146379821c9e9a67e8`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fd6c48b9797955661de6b1bbdb133281e646ce48bea218e29ecbaa8628958f`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:77c4a743329649cd8376baf45d3d6088c85b35a8ea5721c57edcb0d81618293f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34832955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100593e415fe1cca86ecefedad743a9d40d5d926f202e1640dce617d73db3e0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:54:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 05:54:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:54:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 05:54:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 05:54:36 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 05:54:36 GMT
WORKDIR /spiped
# Tue, 23 May 2023 05:54:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 05:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 05:54:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b30fc529faa1ae767912072bbcccc2766cf1567a698bb67daa62fa10f3f50`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dcb25beaa639b1e91802b771b089588a793ca63c16d6e04aa8ba4ca5a5a5e5`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7464ed886e0c0540af2e338ca3ee908bcc9304c2e6922e098a45971e97ca3d3c`  
		Last Modified: Tue, 23 May 2023 05:54:56 GMT  
		Size: 5.2 MB (5187522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28f63af2e817d0c24b1df2d0f6043a0a3d2dac2d8fb740d174f6edbfd68b30`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6499d915f8b515d612f588a84d618d858617e13525e299f6856f58c80df8eaaf`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:2fad538a1868dc8df307fb3e444f7ad9871c29c4590b61a3ad73eab8c97eb30e
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
$ docker pull spiped@sha256:7b7f7844dc68c4b9728d9185d906025f7565df88ca9612aaaf420ac91523f405
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b60c5b50be16ba58852d923ea4e7d5224aecb355eb4588ab08b2f70c72ad851`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:36:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 02:36:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 02:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 02:37:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 02:37:01 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 02:37:02 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 02:37:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:37:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833c4ea98211ab2b826b6d62f250a61b8c5ae407b5de38776cc5bc31d895d3fa`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870359eb3ab308a11eaf9cfc6782cd2bea0c513f3920492180bd5f5cbbea54eb`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.5 MB (1483362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afeb4ec06ad120774f5e7a75610323bda25b84d5957c8bac3f5c90ea7fdd17`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 221.3 KB (221284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9641a8793752f42f60dcbb12e857125ba41995c02e48630112ef3f6d5747a28`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb90b001556af3810279377523e96a71161f2dc727b628cb3d284764e5e847fd`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:98e69abcdbbbc31f8223857ec6529b855f8e21be02602fe6763b73403a252650
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4560042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4871452a88018819e0282cc73c7c17274cbea4b4fd8f73619664078771460b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:22:48 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:22:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:22:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:22:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:22:58 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:22:58 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:22:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:22:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:22:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f18e2ef9b0aa3ce161a88dbc21a7f6e04c161889cd2e9a48db6753f539a908`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f98080b1dde5f78f59c30b4e0ecd3d8755ce81a51335edb1f928872b6ea2758`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.2 MB (1241151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaabfafc343e9926cb7046e859064ad3777e2fc8cddcb7e477dde08175094e7`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 206.4 KB (206355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41f7588b8c91b544e8c7d054c90e59b7a9bd11c4e88918abb84a283000e0017`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd529e07580d9750fa02477c2004129b10b554d974efb4047239df64df3a24`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6c2a2f1aeafd6139364938089caba1b87ad68bedb26cd1880228677d027a8a71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9eb306d4124eb8e1c6195849bb2b723860dae03a03f9bae43f0cb32e1462fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:08:21 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:08:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:08:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:08:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:08:30 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:08:30 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:08:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:08:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df1c1b7ee69f0ffebff840bb383923a8a217c78132af46a52a21f12e14482c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7fa369f75c521bfa073b091a994479792b5e564a5c37699be2008acad03c72`  
		Last Modified: Sat, 08 Apr 2023 02:48:09 GMT  
		Size: 1.2 MB (1167611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21f3a95209349c9b1a3a521865cce5d3c5b7d5c8ff6ff9da5c62bb698fbf9c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 200.1 KB (200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd163e2f331db36950fd2761a2e3546fb04b46eba66cc2de8d5491d403e4be9`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e4936ce3183df5af3ef7fa3066376cab728047d4e40c1541aad098e3d01fb5`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b21f6104cf4f986ae42d2548c5a3e8edfeac1672739642c0051b1ce2e7ddc5dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306f5b9d541620eedadaec0c057f09c6db34da10d9378cae2f5155b0081420a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:50:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 05:50:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 05:50:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 05:50:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 05:50:40 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 05:50:40 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 05:50:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:50:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a75b9333a53162c1a5789a4c7973a5cc525b738e1a394e58db69d0c32fa089`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a905f71ab7e32bea70c662b413534aa7f764438f72937d84176a7b21115e19e`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8364c9ed77705e5bab6f7d3ebcefe334f2401e4822779b17ceb1bb94d7510ce7`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a0bb75b3c36c6b1f0df28be9d91f3073dfcc4b0701cd2dffcafc2d8834c55`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fdfb5809799657c2cc38eac53edd7e1105371601d7e1c155b00bf07f8f3d0`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:0e5f49d56599b01f5aa0c4d6ebedb8fe9e52f5d2a66e094700b5f7703cc3f26e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5132057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa9e52e3f82d57652b3398c82d896ea0c351c189b78a1daa85740fc04413b4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 01:33:10 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 01:33:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 01:33:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 01:33:22 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 01:33:22 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 01:33:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 01:33:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a513a8526f3d62fd7ec1e80a76b26d4cf8c8c37ea534b10e2c0060eb3cb6f0`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7fa7db70396ccd0f7c43ec98f7831c11a443d8d0f9ae5383bd39a0256cd39d`  
		Last Modified: Thu, 30 Mar 2023 01:33:32 GMT  
		Size: 1.5 MB (1486443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d342e0d74297744901c335be2694a48a287375cc57389ee49fc329b6093f5a`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 231.6 KB (231615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc5bf7a2360503d1b51116e389e689406594d6295129a36524b8e4f7bad02d7`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae5cb4f4de570095d623ebcde4ca7cf3062c366c24ad3595d5108c7111c29af`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8b13ec4b458ac31fb096b22da921ddc5f982ca84907ae2ad42dfc9935e69a793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70983caa08c37ccc9d7968473ced65e5b8ee6cc50feff3049de378aee313e62f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 04:32:26 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 04:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 04:32:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 04:32:42 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 04:32:43 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 04:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:32:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:32:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abd914c752b02f6f79b7ef1571ed87d4130a25ed21a1d3892a23e3c2c1cfbec`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cc8ae50d4833e170ee7dc2db705d37cc39c4e228e121c72a14cd9620b4847c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.4 MB (1413051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac183c495785747e187a666506a1c63aeb182e3c511beaa79f82f4c86278a170`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 220.0 KB (220030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a70723c954d9ac5e16090c8b3aa6668bfab3384b6ce30cab8e10925bd1cd6c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a4bf70a1b07cf55ae9e8498ca917bc7a43613629d823f0e1fa9b6c689b47b7`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:31fd069ea692240b5c5fc9e133487e244e6df34ce932c3470cad5763dffaa4c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 MB (6397813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f11cae2fc86cb997405cc5c3a4996740ff4651abe9f0e4af3b4f7ec8c89d5d31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 03 May 2023 23:12:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 03 May 2023 23:12:13 GMT
RUN apk add --no-cache libssl1.1
# Wed, 03 May 2023 23:12:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 May 2023 23:12:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 03 May 2023 23:12:21 GMT
VOLUME [/spiped]
# Wed, 03 May 2023 23:12:21 GMT
WORKDIR /spiped
# Wed, 03 May 2023 23:12:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 May 2023 23:12:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 23:12:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8767d4ba6ffb04a8f593ae3a55b22eb4d0723a412c55cd55bca0f87af4ae7e71`  
		Last Modified: Wed, 03 May 2023 23:12:48 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0ed4aa030d3cd667bab6930140621e2daf46573e404ec7feaa13530d59cf9`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 1.2 MB (1223437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b0ffcfed6008438606174a08a596b98cdf875367dfaecebb1cb095f0fe00e1`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 2.0 MB (1997449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af890e08dc1da930eb9bac534ec7ad96bd229fa34632688bb5a345a9044009c9`  
		Last Modified: Wed, 03 May 2023 23:12:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09f55129759a34f268901f558c8760261b43509b7900c8e66f5f6a447b2ef25`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:3051fd2111d842b48252f722a94c75dbf39dd094a5f3be71676cf84f3a285896
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
$ docker pull spiped@sha256:6e56f898cffedf314d7e78c36169a3c82a3cecb7b3eabcae761df786ffcfa776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37404848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a5c88f0c911b4337a918ef32508daa452d712618d486a0160cd5793cd361ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 12:26:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 12:26:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 12:26:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 12:26:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 12:26:34 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 12:26:34 GMT
WORKDIR /spiped
# Tue, 23 May 2023 12:26:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 12:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 12:26:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ec67773fceb5d595bfdd899df865f6dba186d457790bcbb5651bc6cc99d90d`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843a0deb718885d4a7ec0829e15e29d5bf108522d62cb859c1ea655b40de7c37`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37406cfa1e5f43875100dd643b4ffe1d3d94166b88ca9c89e45c85f9836f4f3f`  
		Last Modified: Tue, 23 May 2023 12:26:50 GMT  
		Size: 6.0 MB (5998006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1da50da921d37b3dd928ff99cbe7041e472193b33f8e7a363565f0918192396`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e68bb6f8c79f1122c9447e56b77fc1f1f33701394359d7da671620d33ea690`  
		Last Modified: Tue, 23 May 2023 12:26:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:49ed0f173e4fcb9fd6bd56651f254b8dfa6b3aed0e1a42f93f166bc8f2226655
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33935055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1db0534cd6253a7850d8a6035c7dca53b22cf72cb2ad369c5cc20375a302343`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:48:41 GMT
ADD file:868f634f5ddb80ed9e9c719ccaf5d564d96fe819f0b000ecc734311baf5da99b in / 
# Tue, 23 May 2023 00:48:42 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:08:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 01:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:08:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 01:09:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:09:25 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 01:09:25 GMT
WORKDIR /spiped
# Tue, 23 May 2023 01:09:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 01:09:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:812967ccba449e7a96044b2d48ffc62816b22eb17641844c4dfffbe3b3ec6f21`  
		Last Modified: Tue, 23 May 2023 00:51:19 GMT  
		Size: 28.9 MB (28903411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce835c01736d996228e733dc5e9ddc64fcaa06d162232eae144c1a997a0e89b3`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354077a571b20fe4e85fcd0dbe7f8ef2f92c66b05eae053b9d9b9a59e99e814`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e5170f406fb5ebb782e8c048c3b0dc057ca5f19b4c4fa9d2fb512b9679350f`  
		Last Modified: Tue, 23 May 2023 01:09:37 GMT  
		Size: 5.0 MB (5028397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca08ae3499842a4a09ebb9ce9ea5344fb0f8a28fa563c97aea66ebc4512d6c7`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8877754d946fb8eef9f97dfae22bbf5f50e90791a8118e6f200475f033e247`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2b9b51f2747566b62f99f3285ba2b22426a10480dcda2197906482f9caa1fc6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31316045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12235c47b83e4e541a5cb08eddccde28158ca3115c91c99a636bbfaad8fda42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:49:41 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 09:49:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 09:49:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 09:50:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 09:50:08 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 09:50:08 GMT
WORKDIR /spiped
# Tue, 23 May 2023 09:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 09:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 09:50:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e366a5a086c832200cf0079c021df977cbf4af1f1bacc5836c38ca9e4fb0801`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26db70e43f87da848b7e77ab58c78d0a9f5df4ea0796fccdf2ff18c5cd8e770`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6b5e5b595b275c3cae346bc7bd81e46d03327fe80e02b279a395a7a94d10f9`  
		Last Modified: Tue, 23 May 2023 09:50:23 GMT  
		Size: 4.7 MB (4748156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c1114f756402ee5152fce302822c514afa5908c89b694fb31c688c1412955`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fde6856633e2275a7b963cf3d0dbe22d60395a4bc9d2c9f197bb10db5f5ff2a`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8a5154f80fcd5049f56d81eaa5fa39c4fd82721f5cc583b6d14bdb7e1b23731f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35326914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7da60844d4229ac6dffb12604f36f1438e8ff4ed0546651f6ba44ab83acc7c28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:20:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 07:20:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:20:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 07:20:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 07:20:57 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 07:20:57 GMT
WORKDIR /spiped
# Tue, 23 May 2023 07:20:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 07:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 07:20:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa8f6bfb1c027bb9f657161080f0ab93d19eebc194113b874d055fdcbfcb460`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47a57eada7dc6536f84b1b4335e54a33593d6eb7ec21e4d1033d6ad1e0a86e7`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e3fff08fa9daa5729dace8c989618277b41785008308f87afcc87e10c5bbb4`  
		Last Modified: Tue, 23 May 2023 07:21:11 GMT  
		Size: 5.3 MB (5270912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c03b1322313f66b8edacbb1f3daf86f76fa0bcf2461f8e9b1c8b0182c569c41`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bce57662b8b31a2ce6d26052524b37aa0e54ae5e585421cd7bd6202e7219607`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:c86f183f59a1da0d47a0ef90433af289f2f2b7c2d833a89316c34d51afe2d0f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40282845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6185bc58ac223183e9461e6107bae7b0e9ca3bbb4338869c1f863ab9c624fa13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:51:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 01:51:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:51:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 01:51:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:51:43 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 01:51:43 GMT
WORKDIR /spiped
# Tue, 23 May 2023 01:51:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 01:51:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 01:51:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9100966936a8c84c9e0e8b57d0811fb36e0e2c2d3e1138a0d3a7a918fe6745c9`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57610b2efa5f7c48f7d1ab161334a38849ff14c70658cb48567036e35e685b91`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1302ffc3a0d553d137a506717f8c2741436b82ff5b23b4353023fc9a35cd98`  
		Last Modified: Tue, 23 May 2023 01:52:01 GMT  
		Size: 7.9 MB (7891426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed28e099af4805a76b58eb4139bf498ac46acfb4d643ec70c9b840eb827750fb`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab03d42d20f08b827cfa1c2ef42e597ffbd8333e2237fa7167ad56119457fbb`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:5048eca6297857f351909c330a9a32c045a8a5656f8a306773cd773ed026ca87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69bb2dc15afa48fd2a905c1b95630d24cb02183dd2e42a0aea1139444f8b2e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 00:10:34 GMT
ADD file:4d5c7737e954f157e3d7ea47cc1814c46ec5c753a3d5d828ad9614969b572253 in / 
# Tue, 13 Jun 2023 00:10:38 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:43:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Jun 2023 01:43:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:43:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Jun 2023 01:45:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:45:14 GMT
VOLUME [/spiped]
# Tue, 13 Jun 2023 01:45:17 GMT
WORKDIR /spiped
# Tue, 13 Jun 2023 01:45:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:45:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 01:45:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:61bd6562a93acd0a3b327321e5465408e1d921b3ce1fb4fe353633330c3ede91`  
		Last Modified: Tue, 13 Jun 2023 00:23:53 GMT  
		Size: 29.6 MB (29634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f0ef0a3861267b4ef08cf448b2f1fc3ade81711b0b5fbd9d6d1581d6d8444f`  
		Last Modified: Tue, 13 Jun 2023 01:45:38 GMT  
		Size: 1.6 KB (1607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46baf526b17f9846cc40a9942d857383066be6d7b9a763ad5fffe1d117d59b3`  
		Last Modified: Tue, 13 Jun 2023 01:45:37 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b277e66890f62e701bf366cadb6b71924c5cb7a1a7286555f99f64fe3b06207`  
		Last Modified: Tue, 13 Jun 2023 01:45:42 GMT  
		Size: 5.7 MB (5705100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fd55e3c4b14927f26b90efaa6ce8242e295488d2b3bba74d8fb002479f80b0`  
		Last Modified: Tue, 13 Jun 2023 01:45:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23161a5a3690af3fa56d7600a2430fad04ac37a3c42eebf022ebd04cc427fb5`  
		Last Modified: Tue, 13 Jun 2023 01:45:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:e26c208c4a4342785c225a1004342e0114c3561ce9b1530544a567b47005086e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41284428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c610878704350416c6e781ffc11dc286e43f4fd60173a4e237e7855a91d0ebb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 10:48:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 10:49:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 10:49:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 10:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 10:49:49 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 10:49:49 GMT
WORKDIR /spiped
# Tue, 23 May 2023 10:49:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 10:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 10:49:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f4a119486e3fcedd3af8f31d52c720861f5cacee89269ad7e0be2c0ab48eed`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b52a815f8a92c8687a8959408e5922807bf95c0905f55a535f52551bf75e6a`  
		Last Modified: Tue, 23 May 2023 10:50:07 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b713f962480fbb84f8dd9a119a34339176e1e324df77251b08080ff5c51f96`  
		Last Modified: Tue, 23 May 2023 10:50:10 GMT  
		Size: 6.0 MB (6000259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d48bbdef4e3e839c97da555fe50a2684844e5f2050859146379821c9e9a67e8`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fd6c48b9797955661de6b1bbdb133281e646ce48bea218e29ecbaa8628958f`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:77c4a743329649cd8376baf45d3d6088c85b35a8ea5721c57edcb0d81618293f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34832955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100593e415fe1cca86ecefedad743a9d40d5d926f202e1640dce617d73db3e0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:54:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 05:54:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:54:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 05:54:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 05:54:36 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 05:54:36 GMT
WORKDIR /spiped
# Tue, 23 May 2023 05:54:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 05:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 05:54:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b30fc529faa1ae767912072bbcccc2766cf1567a698bb67daa62fa10f3f50`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dcb25beaa639b1e91802b771b089588a793ca63c16d6e04aa8ba4ca5a5a5e5`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7464ed886e0c0540af2e338ca3ee908bcc9304c2e6922e098a45971e97ca3d3c`  
		Last Modified: Tue, 23 May 2023 05:54:56 GMT  
		Size: 5.2 MB (5187522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28f63af2e817d0c24b1df2d0f6043a0a3d2dac2d8fb740d174f6edbfd68b30`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6499d915f8b515d612f588a84d618d858617e13525e299f6856f58c80df8eaaf`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:2fad538a1868dc8df307fb3e444f7ad9871c29c4590b61a3ad73eab8c97eb30e
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
$ docker pull spiped@sha256:7b7f7844dc68c4b9728d9185d906025f7565df88ca9612aaaf420ac91523f405
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b60c5b50be16ba58852d923ea4e7d5224aecb355eb4588ab08b2f70c72ad851`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:36:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 02:36:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 02:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 02:37:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 02:37:01 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 02:37:02 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 02:37:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:37:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833c4ea98211ab2b826b6d62f250a61b8c5ae407b5de38776cc5bc31d895d3fa`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870359eb3ab308a11eaf9cfc6782cd2bea0c513f3920492180bd5f5cbbea54eb`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.5 MB (1483362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afeb4ec06ad120774f5e7a75610323bda25b84d5957c8bac3f5c90ea7fdd17`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 221.3 KB (221284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9641a8793752f42f60dcbb12e857125ba41995c02e48630112ef3f6d5747a28`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb90b001556af3810279377523e96a71161f2dc727b628cb3d284764e5e847fd`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:98e69abcdbbbc31f8223857ec6529b855f8e21be02602fe6763b73403a252650
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4560042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4871452a88018819e0282cc73c7c17274cbea4b4fd8f73619664078771460b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:22:48 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:22:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:22:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:22:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:22:58 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:22:58 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:22:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:22:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:22:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f18e2ef9b0aa3ce161a88dbc21a7f6e04c161889cd2e9a48db6753f539a908`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f98080b1dde5f78f59c30b4e0ecd3d8755ce81a51335edb1f928872b6ea2758`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.2 MB (1241151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaabfafc343e9926cb7046e859064ad3777e2fc8cddcb7e477dde08175094e7`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 206.4 KB (206355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41f7588b8c91b544e8c7d054c90e59b7a9bd11c4e88918abb84a283000e0017`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd529e07580d9750fa02477c2004129b10b554d974efb4047239df64df3a24`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6c2a2f1aeafd6139364938089caba1b87ad68bedb26cd1880228677d027a8a71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9eb306d4124eb8e1c6195849bb2b723860dae03a03f9bae43f0cb32e1462fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:08:21 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:08:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:08:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:08:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:08:30 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:08:30 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:08:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:08:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df1c1b7ee69f0ffebff840bb383923a8a217c78132af46a52a21f12e14482c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7fa369f75c521bfa073b091a994479792b5e564a5c37699be2008acad03c72`  
		Last Modified: Sat, 08 Apr 2023 02:48:09 GMT  
		Size: 1.2 MB (1167611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21f3a95209349c9b1a3a521865cce5d3c5b7d5c8ff6ff9da5c62bb698fbf9c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 200.1 KB (200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd163e2f331db36950fd2761a2e3546fb04b46eba66cc2de8d5491d403e4be9`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e4936ce3183df5af3ef7fa3066376cab728047d4e40c1541aad098e3d01fb5`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b21f6104cf4f986ae42d2548c5a3e8edfeac1672739642c0051b1ce2e7ddc5dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306f5b9d541620eedadaec0c057f09c6db34da10d9378cae2f5155b0081420a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:50:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 05:50:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 05:50:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 05:50:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 05:50:40 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 05:50:40 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 05:50:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:50:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a75b9333a53162c1a5789a4c7973a5cc525b738e1a394e58db69d0c32fa089`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a905f71ab7e32bea70c662b413534aa7f764438f72937d84176a7b21115e19e`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8364c9ed77705e5bab6f7d3ebcefe334f2401e4822779b17ceb1bb94d7510ce7`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a0bb75b3c36c6b1f0df28be9d91f3073dfcc4b0701cd2dffcafc2d8834c55`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fdfb5809799657c2cc38eac53edd7e1105371601d7e1c155b00bf07f8f3d0`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:0e5f49d56599b01f5aa0c4d6ebedb8fe9e52f5d2a66e094700b5f7703cc3f26e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5132057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa9e52e3f82d57652b3398c82d896ea0c351c189b78a1daa85740fc04413b4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 01:33:10 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 01:33:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 01:33:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 01:33:22 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 01:33:22 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 01:33:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 01:33:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a513a8526f3d62fd7ec1e80a76b26d4cf8c8c37ea534b10e2c0060eb3cb6f0`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7fa7db70396ccd0f7c43ec98f7831c11a443d8d0f9ae5383bd39a0256cd39d`  
		Last Modified: Thu, 30 Mar 2023 01:33:32 GMT  
		Size: 1.5 MB (1486443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d342e0d74297744901c335be2694a48a287375cc57389ee49fc329b6093f5a`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 231.6 KB (231615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc5bf7a2360503d1b51116e389e689406594d6295129a36524b8e4f7bad02d7`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae5cb4f4de570095d623ebcde4ca7cf3062c366c24ad3595d5108c7111c29af`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8b13ec4b458ac31fb096b22da921ddc5f982ca84907ae2ad42dfc9935e69a793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70983caa08c37ccc9d7968473ced65e5b8ee6cc50feff3049de378aee313e62f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 04:32:26 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 04:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 04:32:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 04:32:42 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 04:32:43 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 04:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:32:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:32:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abd914c752b02f6f79b7ef1571ed87d4130a25ed21a1d3892a23e3c2c1cfbec`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cc8ae50d4833e170ee7dc2db705d37cc39c4e228e121c72a14cd9620b4847c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.4 MB (1413051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac183c495785747e187a666506a1c63aeb182e3c511beaa79f82f4c86278a170`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 220.0 KB (220030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a70723c954d9ac5e16090c8b3aa6668bfab3384b6ce30cab8e10925bd1cd6c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a4bf70a1b07cf55ae9e8498ca917bc7a43613629d823f0e1fa9b6c689b47b7`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:31fd069ea692240b5c5fc9e133487e244e6df34ce932c3470cad5763dffaa4c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 MB (6397813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f11cae2fc86cb997405cc5c3a4996740ff4651abe9f0e4af3b4f7ec8c89d5d31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 03 May 2023 23:12:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 03 May 2023 23:12:13 GMT
RUN apk add --no-cache libssl1.1
# Wed, 03 May 2023 23:12:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 May 2023 23:12:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 03 May 2023 23:12:21 GMT
VOLUME [/spiped]
# Wed, 03 May 2023 23:12:21 GMT
WORKDIR /spiped
# Wed, 03 May 2023 23:12:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 May 2023 23:12:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 23:12:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8767d4ba6ffb04a8f593ae3a55b22eb4d0723a412c55cd55bca0f87af4ae7e71`  
		Last Modified: Wed, 03 May 2023 23:12:48 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0ed4aa030d3cd667bab6930140621e2daf46573e404ec7feaa13530d59cf9`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 1.2 MB (1223437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b0ffcfed6008438606174a08a596b98cdf875367dfaecebb1cb095f0fe00e1`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 2.0 MB (1997449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af890e08dc1da930eb9bac534ec7ad96bd229fa34632688bb5a345a9044009c9`  
		Last Modified: Wed, 03 May 2023 23:12:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09f55129759a34f268901f558c8760261b43509b7900c8e66f5f6a447b2ef25`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:3051fd2111d842b48252f722a94c75dbf39dd094a5f3be71676cf84f3a285896
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
$ docker pull spiped@sha256:6e56f898cffedf314d7e78c36169a3c82a3cecb7b3eabcae761df786ffcfa776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37404848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a5c88f0c911b4337a918ef32508daa452d712618d486a0160cd5793cd361ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 12:26:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 12:26:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 12:26:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 12:26:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 12:26:34 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 12:26:34 GMT
WORKDIR /spiped
# Tue, 23 May 2023 12:26:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 12:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 12:26:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ec67773fceb5d595bfdd899df865f6dba186d457790bcbb5651bc6cc99d90d`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843a0deb718885d4a7ec0829e15e29d5bf108522d62cb859c1ea655b40de7c37`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37406cfa1e5f43875100dd643b4ffe1d3d94166b88ca9c89e45c85f9836f4f3f`  
		Last Modified: Tue, 23 May 2023 12:26:50 GMT  
		Size: 6.0 MB (5998006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1da50da921d37b3dd928ff99cbe7041e472193b33f8e7a363565f0918192396`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e68bb6f8c79f1122c9447e56b77fc1f1f33701394359d7da671620d33ea690`  
		Last Modified: Tue, 23 May 2023 12:26:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:49ed0f173e4fcb9fd6bd56651f254b8dfa6b3aed0e1a42f93f166bc8f2226655
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33935055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1db0534cd6253a7850d8a6035c7dca53b22cf72cb2ad369c5cc20375a302343`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:48:41 GMT
ADD file:868f634f5ddb80ed9e9c719ccaf5d564d96fe819f0b000ecc734311baf5da99b in / 
# Tue, 23 May 2023 00:48:42 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:08:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 01:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:08:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 01:09:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:09:25 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 01:09:25 GMT
WORKDIR /spiped
# Tue, 23 May 2023 01:09:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 01:09:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:812967ccba449e7a96044b2d48ffc62816b22eb17641844c4dfffbe3b3ec6f21`  
		Last Modified: Tue, 23 May 2023 00:51:19 GMT  
		Size: 28.9 MB (28903411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce835c01736d996228e733dc5e9ddc64fcaa06d162232eae144c1a997a0e89b3`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354077a571b20fe4e85fcd0dbe7f8ef2f92c66b05eae053b9d9b9a59e99e814`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e5170f406fb5ebb782e8c048c3b0dc057ca5f19b4c4fa9d2fb512b9679350f`  
		Last Modified: Tue, 23 May 2023 01:09:37 GMT  
		Size: 5.0 MB (5028397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca08ae3499842a4a09ebb9ce9ea5344fb0f8a28fa563c97aea66ebc4512d6c7`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8877754d946fb8eef9f97dfae22bbf5f50e90791a8118e6f200475f033e247`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2b9b51f2747566b62f99f3285ba2b22426a10480dcda2197906482f9caa1fc6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31316045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12235c47b83e4e541a5cb08eddccde28158ca3115c91c99a636bbfaad8fda42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:49:41 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 09:49:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 09:49:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 09:50:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 09:50:08 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 09:50:08 GMT
WORKDIR /spiped
# Tue, 23 May 2023 09:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 09:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 09:50:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e366a5a086c832200cf0079c021df977cbf4af1f1bacc5836c38ca9e4fb0801`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26db70e43f87da848b7e77ab58c78d0a9f5df4ea0796fccdf2ff18c5cd8e770`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6b5e5b595b275c3cae346bc7bd81e46d03327fe80e02b279a395a7a94d10f9`  
		Last Modified: Tue, 23 May 2023 09:50:23 GMT  
		Size: 4.7 MB (4748156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c1114f756402ee5152fce302822c514afa5908c89b694fb31c688c1412955`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fde6856633e2275a7b963cf3d0dbe22d60395a4bc9d2c9f197bb10db5f5ff2a`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8a5154f80fcd5049f56d81eaa5fa39c4fd82721f5cc583b6d14bdb7e1b23731f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35326914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7da60844d4229ac6dffb12604f36f1438e8ff4ed0546651f6ba44ab83acc7c28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:20:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 07:20:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:20:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 07:20:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 07:20:57 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 07:20:57 GMT
WORKDIR /spiped
# Tue, 23 May 2023 07:20:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 07:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 07:20:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa8f6bfb1c027bb9f657161080f0ab93d19eebc194113b874d055fdcbfcb460`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47a57eada7dc6536f84b1b4335e54a33593d6eb7ec21e4d1033d6ad1e0a86e7`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e3fff08fa9daa5729dace8c989618277b41785008308f87afcc87e10c5bbb4`  
		Last Modified: Tue, 23 May 2023 07:21:11 GMT  
		Size: 5.3 MB (5270912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c03b1322313f66b8edacbb1f3daf86f76fa0bcf2461f8e9b1c8b0182c569c41`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bce57662b8b31a2ce6d26052524b37aa0e54ae5e585421cd7bd6202e7219607`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:c86f183f59a1da0d47a0ef90433af289f2f2b7c2d833a89316c34d51afe2d0f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40282845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6185bc58ac223183e9461e6107bae7b0e9ca3bbb4338869c1f863ab9c624fa13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:51:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 01:51:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:51:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 01:51:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:51:43 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 01:51:43 GMT
WORKDIR /spiped
# Tue, 23 May 2023 01:51:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 01:51:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 01:51:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9100966936a8c84c9e0e8b57d0811fb36e0e2c2d3e1138a0d3a7a918fe6745c9`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57610b2efa5f7c48f7d1ab161334a38849ff14c70658cb48567036e35e685b91`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1302ffc3a0d553d137a506717f8c2741436b82ff5b23b4353023fc9a35cd98`  
		Last Modified: Tue, 23 May 2023 01:52:01 GMT  
		Size: 7.9 MB (7891426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed28e099af4805a76b58eb4139bf498ac46acfb4d643ec70c9b840eb827750fb`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab03d42d20f08b827cfa1c2ef42e597ffbd8333e2237fa7167ad56119457fbb`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:5048eca6297857f351909c330a9a32c045a8a5656f8a306773cd773ed026ca87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69bb2dc15afa48fd2a905c1b95630d24cb02183dd2e42a0aea1139444f8b2e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 00:10:34 GMT
ADD file:4d5c7737e954f157e3d7ea47cc1814c46ec5c753a3d5d828ad9614969b572253 in / 
# Tue, 13 Jun 2023 00:10:38 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:43:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Jun 2023 01:43:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:43:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Jun 2023 01:45:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:45:14 GMT
VOLUME [/spiped]
# Tue, 13 Jun 2023 01:45:17 GMT
WORKDIR /spiped
# Tue, 13 Jun 2023 01:45:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:45:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 01:45:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:61bd6562a93acd0a3b327321e5465408e1d921b3ce1fb4fe353633330c3ede91`  
		Last Modified: Tue, 13 Jun 2023 00:23:53 GMT  
		Size: 29.6 MB (29634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f0ef0a3861267b4ef08cf448b2f1fc3ade81711b0b5fbd9d6d1581d6d8444f`  
		Last Modified: Tue, 13 Jun 2023 01:45:38 GMT  
		Size: 1.6 KB (1607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46baf526b17f9846cc40a9942d857383066be6d7b9a763ad5fffe1d117d59b3`  
		Last Modified: Tue, 13 Jun 2023 01:45:37 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b277e66890f62e701bf366cadb6b71924c5cb7a1a7286555f99f64fe3b06207`  
		Last Modified: Tue, 13 Jun 2023 01:45:42 GMT  
		Size: 5.7 MB (5705100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fd55e3c4b14927f26b90efaa6ce8242e295488d2b3bba74d8fb002479f80b0`  
		Last Modified: Tue, 13 Jun 2023 01:45:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23161a5a3690af3fa56d7600a2430fad04ac37a3c42eebf022ebd04cc427fb5`  
		Last Modified: Tue, 13 Jun 2023 01:45:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:e26c208c4a4342785c225a1004342e0114c3561ce9b1530544a567b47005086e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41284428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c610878704350416c6e781ffc11dc286e43f4fd60173a4e237e7855a91d0ebb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 10:48:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 10:49:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 10:49:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 10:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 10:49:49 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 10:49:49 GMT
WORKDIR /spiped
# Tue, 23 May 2023 10:49:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 10:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 10:49:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f4a119486e3fcedd3af8f31d52c720861f5cacee89269ad7e0be2c0ab48eed`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b52a815f8a92c8687a8959408e5922807bf95c0905f55a535f52551bf75e6a`  
		Last Modified: Tue, 23 May 2023 10:50:07 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b713f962480fbb84f8dd9a119a34339176e1e324df77251b08080ff5c51f96`  
		Last Modified: Tue, 23 May 2023 10:50:10 GMT  
		Size: 6.0 MB (6000259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d48bbdef4e3e839c97da555fe50a2684844e5f2050859146379821c9e9a67e8`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fd6c48b9797955661de6b1bbdb133281e646ce48bea218e29ecbaa8628958f`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:77c4a743329649cd8376baf45d3d6088c85b35a8ea5721c57edcb0d81618293f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34832955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100593e415fe1cca86ecefedad743a9d40d5d926f202e1640dce617d73db3e0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:54:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 05:54:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:54:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 05:54:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 05:54:36 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 05:54:36 GMT
WORKDIR /spiped
# Tue, 23 May 2023 05:54:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 05:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 05:54:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b30fc529faa1ae767912072bbcccc2766cf1567a698bb67daa62fa10f3f50`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dcb25beaa639b1e91802b771b089588a793ca63c16d6e04aa8ba4ca5a5a5e5`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7464ed886e0c0540af2e338ca3ee908bcc9304c2e6922e098a45971e97ca3d3c`  
		Last Modified: Tue, 23 May 2023 05:54:56 GMT  
		Size: 5.2 MB (5187522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28f63af2e817d0c24b1df2d0f6043a0a3d2dac2d8fb740d174f6edbfd68b30`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6499d915f8b515d612f588a84d618d858617e13525e299f6856f58c80df8eaaf`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:2fad538a1868dc8df307fb3e444f7ad9871c29c4590b61a3ad73eab8c97eb30e
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
$ docker pull spiped@sha256:7b7f7844dc68c4b9728d9185d906025f7565df88ca9612aaaf420ac91523f405
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b60c5b50be16ba58852d923ea4e7d5224aecb355eb4588ab08b2f70c72ad851`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:36:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 02:36:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 02:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 02:37:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 02:37:01 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 02:37:02 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 02:37:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:37:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833c4ea98211ab2b826b6d62f250a61b8c5ae407b5de38776cc5bc31d895d3fa`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870359eb3ab308a11eaf9cfc6782cd2bea0c513f3920492180bd5f5cbbea54eb`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.5 MB (1483362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afeb4ec06ad120774f5e7a75610323bda25b84d5957c8bac3f5c90ea7fdd17`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 221.3 KB (221284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9641a8793752f42f60dcbb12e857125ba41995c02e48630112ef3f6d5747a28`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb90b001556af3810279377523e96a71161f2dc727b628cb3d284764e5e847fd`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:98e69abcdbbbc31f8223857ec6529b855f8e21be02602fe6763b73403a252650
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4560042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4871452a88018819e0282cc73c7c17274cbea4b4fd8f73619664078771460b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:22:48 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:22:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:22:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:22:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:22:58 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:22:58 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:22:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:22:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:22:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f18e2ef9b0aa3ce161a88dbc21a7f6e04c161889cd2e9a48db6753f539a908`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f98080b1dde5f78f59c30b4e0ecd3d8755ce81a51335edb1f928872b6ea2758`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.2 MB (1241151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaabfafc343e9926cb7046e859064ad3777e2fc8cddcb7e477dde08175094e7`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 206.4 KB (206355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41f7588b8c91b544e8c7d054c90e59b7a9bd11c4e88918abb84a283000e0017`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd529e07580d9750fa02477c2004129b10b554d974efb4047239df64df3a24`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6c2a2f1aeafd6139364938089caba1b87ad68bedb26cd1880228677d027a8a71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9eb306d4124eb8e1c6195849bb2b723860dae03a03f9bae43f0cb32e1462fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:08:21 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:08:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:08:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:08:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:08:30 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:08:30 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:08:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:08:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df1c1b7ee69f0ffebff840bb383923a8a217c78132af46a52a21f12e14482c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7fa369f75c521bfa073b091a994479792b5e564a5c37699be2008acad03c72`  
		Last Modified: Sat, 08 Apr 2023 02:48:09 GMT  
		Size: 1.2 MB (1167611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21f3a95209349c9b1a3a521865cce5d3c5b7d5c8ff6ff9da5c62bb698fbf9c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 200.1 KB (200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd163e2f331db36950fd2761a2e3546fb04b46eba66cc2de8d5491d403e4be9`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e4936ce3183df5af3ef7fa3066376cab728047d4e40c1541aad098e3d01fb5`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b21f6104cf4f986ae42d2548c5a3e8edfeac1672739642c0051b1ce2e7ddc5dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306f5b9d541620eedadaec0c057f09c6db34da10d9378cae2f5155b0081420a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:50:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 05:50:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 05:50:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 05:50:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 05:50:40 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 05:50:40 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 05:50:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:50:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a75b9333a53162c1a5789a4c7973a5cc525b738e1a394e58db69d0c32fa089`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a905f71ab7e32bea70c662b413534aa7f764438f72937d84176a7b21115e19e`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8364c9ed77705e5bab6f7d3ebcefe334f2401e4822779b17ceb1bb94d7510ce7`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a0bb75b3c36c6b1f0df28be9d91f3073dfcc4b0701cd2dffcafc2d8834c55`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fdfb5809799657c2cc38eac53edd7e1105371601d7e1c155b00bf07f8f3d0`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:0e5f49d56599b01f5aa0c4d6ebedb8fe9e52f5d2a66e094700b5f7703cc3f26e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5132057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa9e52e3f82d57652b3398c82d896ea0c351c189b78a1daa85740fc04413b4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 01:33:10 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 01:33:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 01:33:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 01:33:22 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 01:33:22 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 01:33:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 01:33:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a513a8526f3d62fd7ec1e80a76b26d4cf8c8c37ea534b10e2c0060eb3cb6f0`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7fa7db70396ccd0f7c43ec98f7831c11a443d8d0f9ae5383bd39a0256cd39d`  
		Last Modified: Thu, 30 Mar 2023 01:33:32 GMT  
		Size: 1.5 MB (1486443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d342e0d74297744901c335be2694a48a287375cc57389ee49fc329b6093f5a`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 231.6 KB (231615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc5bf7a2360503d1b51116e389e689406594d6295129a36524b8e4f7bad02d7`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae5cb4f4de570095d623ebcde4ca7cf3062c366c24ad3595d5108c7111c29af`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8b13ec4b458ac31fb096b22da921ddc5f982ca84907ae2ad42dfc9935e69a793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70983caa08c37ccc9d7968473ced65e5b8ee6cc50feff3049de378aee313e62f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 04:32:26 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 04:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 04:32:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 04:32:42 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 04:32:43 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 04:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:32:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:32:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abd914c752b02f6f79b7ef1571ed87d4130a25ed21a1d3892a23e3c2c1cfbec`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cc8ae50d4833e170ee7dc2db705d37cc39c4e228e121c72a14cd9620b4847c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.4 MB (1413051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac183c495785747e187a666506a1c63aeb182e3c511beaa79f82f4c86278a170`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 220.0 KB (220030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a70723c954d9ac5e16090c8b3aa6668bfab3384b6ce30cab8e10925bd1cd6c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a4bf70a1b07cf55ae9e8498ca917bc7a43613629d823f0e1fa9b6c689b47b7`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:31fd069ea692240b5c5fc9e133487e244e6df34ce932c3470cad5763dffaa4c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 MB (6397813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f11cae2fc86cb997405cc5c3a4996740ff4651abe9f0e4af3b4f7ec8c89d5d31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 03 May 2023 23:12:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 03 May 2023 23:12:13 GMT
RUN apk add --no-cache libssl1.1
# Wed, 03 May 2023 23:12:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 May 2023 23:12:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 03 May 2023 23:12:21 GMT
VOLUME [/spiped]
# Wed, 03 May 2023 23:12:21 GMT
WORKDIR /spiped
# Wed, 03 May 2023 23:12:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 May 2023 23:12:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 23:12:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8767d4ba6ffb04a8f593ae3a55b22eb4d0723a412c55cd55bca0f87af4ae7e71`  
		Last Modified: Wed, 03 May 2023 23:12:48 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0ed4aa030d3cd667bab6930140621e2daf46573e404ec7feaa13530d59cf9`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 1.2 MB (1223437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b0ffcfed6008438606174a08a596b98cdf875367dfaecebb1cb095f0fe00e1`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 2.0 MB (1997449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af890e08dc1da930eb9bac534ec7ad96bd229fa34632688bb5a345a9044009c9`  
		Last Modified: Wed, 03 May 2023 23:12:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09f55129759a34f268901f558c8760261b43509b7900c8e66f5f6a447b2ef25`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:2fad538a1868dc8df307fb3e444f7ad9871c29c4590b61a3ad73eab8c97eb30e
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
$ docker pull spiped@sha256:7b7f7844dc68c4b9728d9185d906025f7565df88ca9612aaaf420ac91523f405
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b60c5b50be16ba58852d923ea4e7d5224aecb355eb4588ab08b2f70c72ad851`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:36:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 02:36:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 02:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 02:37:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 02:37:01 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 02:37:02 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 02:37:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:37:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833c4ea98211ab2b826b6d62f250a61b8c5ae407b5de38776cc5bc31d895d3fa`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870359eb3ab308a11eaf9cfc6782cd2bea0c513f3920492180bd5f5cbbea54eb`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.5 MB (1483362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afeb4ec06ad120774f5e7a75610323bda25b84d5957c8bac3f5c90ea7fdd17`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 221.3 KB (221284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9641a8793752f42f60dcbb12e857125ba41995c02e48630112ef3f6d5747a28`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb90b001556af3810279377523e96a71161f2dc727b628cb3d284764e5e847fd`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:98e69abcdbbbc31f8223857ec6529b855f8e21be02602fe6763b73403a252650
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4560042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4871452a88018819e0282cc73c7c17274cbea4b4fd8f73619664078771460b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:22:48 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:22:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:22:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:22:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:22:58 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:22:58 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:22:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:22:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:22:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f18e2ef9b0aa3ce161a88dbc21a7f6e04c161889cd2e9a48db6753f539a908`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f98080b1dde5f78f59c30b4e0ecd3d8755ce81a51335edb1f928872b6ea2758`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.2 MB (1241151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaabfafc343e9926cb7046e859064ad3777e2fc8cddcb7e477dde08175094e7`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 206.4 KB (206355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41f7588b8c91b544e8c7d054c90e59b7a9bd11c4e88918abb84a283000e0017`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd529e07580d9750fa02477c2004129b10b554d974efb4047239df64df3a24`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6c2a2f1aeafd6139364938089caba1b87ad68bedb26cd1880228677d027a8a71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9eb306d4124eb8e1c6195849bb2b723860dae03a03f9bae43f0cb32e1462fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:08:21 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:08:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:08:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:08:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:08:30 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:08:30 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:08:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:08:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df1c1b7ee69f0ffebff840bb383923a8a217c78132af46a52a21f12e14482c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7fa369f75c521bfa073b091a994479792b5e564a5c37699be2008acad03c72`  
		Last Modified: Sat, 08 Apr 2023 02:48:09 GMT  
		Size: 1.2 MB (1167611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21f3a95209349c9b1a3a521865cce5d3c5b7d5c8ff6ff9da5c62bb698fbf9c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 200.1 KB (200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd163e2f331db36950fd2761a2e3546fb04b46eba66cc2de8d5491d403e4be9`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e4936ce3183df5af3ef7fa3066376cab728047d4e40c1541aad098e3d01fb5`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b21f6104cf4f986ae42d2548c5a3e8edfeac1672739642c0051b1ce2e7ddc5dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306f5b9d541620eedadaec0c057f09c6db34da10d9378cae2f5155b0081420a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:50:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 05:50:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 05:50:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 05:50:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 05:50:40 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 05:50:40 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 05:50:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:50:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a75b9333a53162c1a5789a4c7973a5cc525b738e1a394e58db69d0c32fa089`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a905f71ab7e32bea70c662b413534aa7f764438f72937d84176a7b21115e19e`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8364c9ed77705e5bab6f7d3ebcefe334f2401e4822779b17ceb1bb94d7510ce7`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a0bb75b3c36c6b1f0df28be9d91f3073dfcc4b0701cd2dffcafc2d8834c55`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fdfb5809799657c2cc38eac53edd7e1105371601d7e1c155b00bf07f8f3d0`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:0e5f49d56599b01f5aa0c4d6ebedb8fe9e52f5d2a66e094700b5f7703cc3f26e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5132057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa9e52e3f82d57652b3398c82d896ea0c351c189b78a1daa85740fc04413b4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 01:33:10 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 01:33:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 01:33:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 01:33:22 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 01:33:22 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 01:33:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 01:33:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a513a8526f3d62fd7ec1e80a76b26d4cf8c8c37ea534b10e2c0060eb3cb6f0`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7fa7db70396ccd0f7c43ec98f7831c11a443d8d0f9ae5383bd39a0256cd39d`  
		Last Modified: Thu, 30 Mar 2023 01:33:32 GMT  
		Size: 1.5 MB (1486443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d342e0d74297744901c335be2694a48a287375cc57389ee49fc329b6093f5a`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 231.6 KB (231615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc5bf7a2360503d1b51116e389e689406594d6295129a36524b8e4f7bad02d7`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae5cb4f4de570095d623ebcde4ca7cf3062c366c24ad3595d5108c7111c29af`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8b13ec4b458ac31fb096b22da921ddc5f982ca84907ae2ad42dfc9935e69a793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70983caa08c37ccc9d7968473ced65e5b8ee6cc50feff3049de378aee313e62f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 04:32:26 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 04:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 04:32:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 04:32:42 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 04:32:43 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 04:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:32:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:32:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abd914c752b02f6f79b7ef1571ed87d4130a25ed21a1d3892a23e3c2c1cfbec`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cc8ae50d4833e170ee7dc2db705d37cc39c4e228e121c72a14cd9620b4847c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.4 MB (1413051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac183c495785747e187a666506a1c63aeb182e3c511beaa79f82f4c86278a170`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 220.0 KB (220030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a70723c954d9ac5e16090c8b3aa6668bfab3384b6ce30cab8e10925bd1cd6c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a4bf70a1b07cf55ae9e8498ca917bc7a43613629d823f0e1fa9b6c689b47b7`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:31fd069ea692240b5c5fc9e133487e244e6df34ce932c3470cad5763dffaa4c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 MB (6397813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f11cae2fc86cb997405cc5c3a4996740ff4651abe9f0e4af3b4f7ec8c89d5d31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 03 May 2023 23:12:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 03 May 2023 23:12:13 GMT
RUN apk add --no-cache libssl1.1
# Wed, 03 May 2023 23:12:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 May 2023 23:12:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 03 May 2023 23:12:21 GMT
VOLUME [/spiped]
# Wed, 03 May 2023 23:12:21 GMT
WORKDIR /spiped
# Wed, 03 May 2023 23:12:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 May 2023 23:12:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 23:12:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8767d4ba6ffb04a8f593ae3a55b22eb4d0723a412c55cd55bca0f87af4ae7e71`  
		Last Modified: Wed, 03 May 2023 23:12:48 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0ed4aa030d3cd667bab6930140621e2daf46573e404ec7feaa13530d59cf9`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 1.2 MB (1223437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b0ffcfed6008438606174a08a596b98cdf875367dfaecebb1cb095f0fe00e1`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 2.0 MB (1997449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af890e08dc1da930eb9bac534ec7ad96bd229fa34632688bb5a345a9044009c9`  
		Last Modified: Wed, 03 May 2023 23:12:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09f55129759a34f268901f558c8760261b43509b7900c8e66f5f6a447b2ef25`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:3051fd2111d842b48252f722a94c75dbf39dd094a5f3be71676cf84f3a285896
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
$ docker pull spiped@sha256:6e56f898cffedf314d7e78c36169a3c82a3cecb7b3eabcae761df786ffcfa776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37404848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a5c88f0c911b4337a918ef32508daa452d712618d486a0160cd5793cd361ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 12:26:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 12:26:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 12:26:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 12:26:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 12:26:34 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 12:26:34 GMT
WORKDIR /spiped
# Tue, 23 May 2023 12:26:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 12:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 12:26:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ec67773fceb5d595bfdd899df865f6dba186d457790bcbb5651bc6cc99d90d`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843a0deb718885d4a7ec0829e15e29d5bf108522d62cb859c1ea655b40de7c37`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37406cfa1e5f43875100dd643b4ffe1d3d94166b88ca9c89e45c85f9836f4f3f`  
		Last Modified: Tue, 23 May 2023 12:26:50 GMT  
		Size: 6.0 MB (5998006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1da50da921d37b3dd928ff99cbe7041e472193b33f8e7a363565f0918192396`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e68bb6f8c79f1122c9447e56b77fc1f1f33701394359d7da671620d33ea690`  
		Last Modified: Tue, 23 May 2023 12:26:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:49ed0f173e4fcb9fd6bd56651f254b8dfa6b3aed0e1a42f93f166bc8f2226655
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33935055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1db0534cd6253a7850d8a6035c7dca53b22cf72cb2ad369c5cc20375a302343`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:48:41 GMT
ADD file:868f634f5ddb80ed9e9c719ccaf5d564d96fe819f0b000ecc734311baf5da99b in / 
# Tue, 23 May 2023 00:48:42 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:08:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 01:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:08:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 01:09:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:09:25 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 01:09:25 GMT
WORKDIR /spiped
# Tue, 23 May 2023 01:09:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 01:09:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:812967ccba449e7a96044b2d48ffc62816b22eb17641844c4dfffbe3b3ec6f21`  
		Last Modified: Tue, 23 May 2023 00:51:19 GMT  
		Size: 28.9 MB (28903411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce835c01736d996228e733dc5e9ddc64fcaa06d162232eae144c1a997a0e89b3`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354077a571b20fe4e85fcd0dbe7f8ef2f92c66b05eae053b9d9b9a59e99e814`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e5170f406fb5ebb782e8c048c3b0dc057ca5f19b4c4fa9d2fb512b9679350f`  
		Last Modified: Tue, 23 May 2023 01:09:37 GMT  
		Size: 5.0 MB (5028397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca08ae3499842a4a09ebb9ce9ea5344fb0f8a28fa563c97aea66ebc4512d6c7`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8877754d946fb8eef9f97dfae22bbf5f50e90791a8118e6f200475f033e247`  
		Last Modified: Tue, 23 May 2023 01:09:36 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2b9b51f2747566b62f99f3285ba2b22426a10480dcda2197906482f9caa1fc6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31316045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12235c47b83e4e541a5cb08eddccde28158ca3115c91c99a636bbfaad8fda42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:49:41 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 09:49:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 09:49:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 09:50:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 09:50:08 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 09:50:08 GMT
WORKDIR /spiped
# Tue, 23 May 2023 09:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 09:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 09:50:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e366a5a086c832200cf0079c021df977cbf4af1f1bacc5836c38ca9e4fb0801`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26db70e43f87da848b7e77ab58c78d0a9f5df4ea0796fccdf2ff18c5cd8e770`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6b5e5b595b275c3cae346bc7bd81e46d03327fe80e02b279a395a7a94d10f9`  
		Last Modified: Tue, 23 May 2023 09:50:23 GMT  
		Size: 4.7 MB (4748156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c1114f756402ee5152fce302822c514afa5908c89b694fb31c688c1412955`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fde6856633e2275a7b963cf3d0dbe22d60395a4bc9d2c9f197bb10db5f5ff2a`  
		Last Modified: Tue, 23 May 2023 09:50:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8a5154f80fcd5049f56d81eaa5fa39c4fd82721f5cc583b6d14bdb7e1b23731f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35326914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7da60844d4229ac6dffb12604f36f1438e8ff4ed0546651f6ba44ab83acc7c28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:20:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 07:20:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:20:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 07:20:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 07:20:57 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 07:20:57 GMT
WORKDIR /spiped
# Tue, 23 May 2023 07:20:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 07:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 07:20:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa8f6bfb1c027bb9f657161080f0ab93d19eebc194113b874d055fdcbfcb460`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47a57eada7dc6536f84b1b4335e54a33593d6eb7ec21e4d1033d6ad1e0a86e7`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e3fff08fa9daa5729dace8c989618277b41785008308f87afcc87e10c5bbb4`  
		Last Modified: Tue, 23 May 2023 07:21:11 GMT  
		Size: 5.3 MB (5270912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c03b1322313f66b8edacbb1f3daf86f76fa0bcf2461f8e9b1c8b0182c569c41`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bce57662b8b31a2ce6d26052524b37aa0e54ae5e585421cd7bd6202e7219607`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:c86f183f59a1da0d47a0ef90433af289f2f2b7c2d833a89316c34d51afe2d0f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40282845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6185bc58ac223183e9461e6107bae7b0e9ca3bbb4338869c1f863ab9c624fa13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:51:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 01:51:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:51:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 01:51:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:51:43 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 01:51:43 GMT
WORKDIR /spiped
# Tue, 23 May 2023 01:51:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 01:51:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 01:51:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9100966936a8c84c9e0e8b57d0811fb36e0e2c2d3e1138a0d3a7a918fe6745c9`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57610b2efa5f7c48f7d1ab161334a38849ff14c70658cb48567036e35e685b91`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1302ffc3a0d553d137a506717f8c2741436b82ff5b23b4353023fc9a35cd98`  
		Last Modified: Tue, 23 May 2023 01:52:01 GMT  
		Size: 7.9 MB (7891426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed28e099af4805a76b58eb4139bf498ac46acfb4d643ec70c9b840eb827750fb`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab03d42d20f08b827cfa1c2ef42e597ffbd8333e2237fa7167ad56119457fbb`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:5048eca6297857f351909c330a9a32c045a8a5656f8a306773cd773ed026ca87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69bb2dc15afa48fd2a905c1b95630d24cb02183dd2e42a0aea1139444f8b2e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 00:10:34 GMT
ADD file:4d5c7737e954f157e3d7ea47cc1814c46ec5c753a3d5d828ad9614969b572253 in / 
# Tue, 13 Jun 2023 00:10:38 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:43:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Jun 2023 01:43:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:43:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Jun 2023 01:45:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:45:14 GMT
VOLUME [/spiped]
# Tue, 13 Jun 2023 01:45:17 GMT
WORKDIR /spiped
# Tue, 13 Jun 2023 01:45:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:45:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 01:45:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:61bd6562a93acd0a3b327321e5465408e1d921b3ce1fb4fe353633330c3ede91`  
		Last Modified: Tue, 13 Jun 2023 00:23:53 GMT  
		Size: 29.6 MB (29634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f0ef0a3861267b4ef08cf448b2f1fc3ade81711b0b5fbd9d6d1581d6d8444f`  
		Last Modified: Tue, 13 Jun 2023 01:45:38 GMT  
		Size: 1.6 KB (1607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46baf526b17f9846cc40a9942d857383066be6d7b9a763ad5fffe1d117d59b3`  
		Last Modified: Tue, 13 Jun 2023 01:45:37 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b277e66890f62e701bf366cadb6b71924c5cb7a1a7286555f99f64fe3b06207`  
		Last Modified: Tue, 13 Jun 2023 01:45:42 GMT  
		Size: 5.7 MB (5705100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fd55e3c4b14927f26b90efaa6ce8242e295488d2b3bba74d8fb002479f80b0`  
		Last Modified: Tue, 13 Jun 2023 01:45:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23161a5a3690af3fa56d7600a2430fad04ac37a3c42eebf022ebd04cc427fb5`  
		Last Modified: Tue, 13 Jun 2023 01:45:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:e26c208c4a4342785c225a1004342e0114c3561ce9b1530544a567b47005086e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41284428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c610878704350416c6e781ffc11dc286e43f4fd60173a4e237e7855a91d0ebb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 10:48:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 10:49:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 10:49:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 10:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 10:49:49 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 10:49:49 GMT
WORKDIR /spiped
# Tue, 23 May 2023 10:49:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 10:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 10:49:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f4a119486e3fcedd3af8f31d52c720861f5cacee89269ad7e0be2c0ab48eed`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b52a815f8a92c8687a8959408e5922807bf95c0905f55a535f52551bf75e6a`  
		Last Modified: Tue, 23 May 2023 10:50:07 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b713f962480fbb84f8dd9a119a34339176e1e324df77251b08080ff5c51f96`  
		Last Modified: Tue, 23 May 2023 10:50:10 GMT  
		Size: 6.0 MB (6000259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d48bbdef4e3e839c97da555fe50a2684844e5f2050859146379821c9e9a67e8`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fd6c48b9797955661de6b1bbdb133281e646ce48bea218e29ecbaa8628958f`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:77c4a743329649cd8376baf45d3d6088c85b35a8ea5721c57edcb0d81618293f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34832955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100593e415fe1cca86ecefedad743a9d40d5d926f202e1640dce617d73db3e0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:54:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 05:54:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:54:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 05:54:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 05:54:36 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 05:54:36 GMT
WORKDIR /spiped
# Tue, 23 May 2023 05:54:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 05:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 05:54:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b30fc529faa1ae767912072bbcccc2766cf1567a698bb67daa62fa10f3f50`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dcb25beaa639b1e91802b771b089588a793ca63c16d6e04aa8ba4ca5a5a5e5`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7464ed886e0c0540af2e338ca3ee908bcc9304c2e6922e098a45971e97ca3d3c`  
		Last Modified: Tue, 23 May 2023 05:54:56 GMT  
		Size: 5.2 MB (5187522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28f63af2e817d0c24b1df2d0f6043a0a3d2dac2d8fb740d174f6edbfd68b30`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6499d915f8b515d612f588a84d618d858617e13525e299f6856f58c80df8eaaf`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
