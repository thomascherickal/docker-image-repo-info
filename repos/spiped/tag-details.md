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
$ docker pull spiped@sha256:23daec2ad9d865e8d83dce3b3853efa6d665082b70f54b7e3a163b6f6d224069
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
$ docker pull spiped@sha256:099048569b329879479b0b1ae1d9f8192e4268013efe8de12c90b8f2278c6c3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38217263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d04e78fe52f9fb4ae91b1ccce84e9b109608505db0d56fbff3ec70f3f803610f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:49 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 01 Nov 2023 00:20:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 15:58:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 15:58:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 15:58:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 15:58:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 15:58:28 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 15:58:28 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 15:58:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 15:58:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 15:58:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee77a37e1a0fae49537f1c45d174eb2156a9f73bdb4c17cdc4848a5d79450314`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a0ee31fece3b5baa9cfb4e7b7f8aea69c34d8c742b1d77ca99b4dd37f5a31f`  
		Last Modified: Wed, 01 Nov 2023 15:58:45 GMT  
		Size: 2.6 MB (2591903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf356231cfb90da4eb4d73b452416f07680c063365c51f4c50aaea003ce539`  
		Last Modified: Wed, 01 Nov 2023 15:58:45 GMT  
		Size: 6.5 MB (6473928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a667b5364abbbc9bb0a0bf62cd773c47ec6aafdea30ae8e31de144b73429c07`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447ca94f057c4abc2edebebf17fdf11a77bbbf3793415ce61c5db3c10304761c`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a22fc52e1353a81c0b5e864f000d5b7c6f511f31d25d33161d7fff1fa66a128f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34250716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:805e4bd68f268c5a14b0391f350041c251fc5129caa5978c1f2bd4a998995836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:48:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:48:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:48:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:48:30 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:48:31 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:48:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c4d22227960e496eb464146dc866dad412f31aa91c728607dde4278de637ee`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53633f32e999cc192394918d73de2f3ad375e658d9e7dd207468ea6b664eb6d4`  
		Last Modified: Tue, 21 Nov 2023 05:48:39 GMT  
		Size: 2.2 MB (2186814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82ff098495f0ea42040c5184eb059c29c59d5d6e660aa0b1fbc7fff91b2ad4b`  
		Last Modified: Tue, 21 Nov 2023 05:48:40 GMT  
		Size: 5.1 MB (5140150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f734161b12b1fc00f0c981ce9f8176dacc5ca02b74484b806d289850efaa8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f8f249901f701b78f48d77ef49a7fe721309da08eae74507aec894e5a49af8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d49e38f255892c26d1cde15165c35c32cf857b3446c025ecbd69a009b6d59a12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31677806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97542227ddc0fffbebd6a1fa7da3015089ed0e15aa7d37d4d6c22aa77e4748e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 11:53:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 11:53:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 11:53:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 11:54:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 11:54:13 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 11:54:13 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 11:54:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 11:54:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac591a8672b5dba3bfcbe0fe6c21f8387ab9a4f56d6ea32f9eebf5e37feca3`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0fa0448ca0214cd73bf754ce7fd1d9686bd3de6b1bf5840a2c8bd3587f1109`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 2.0 MB (2046224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efda8a5518d4c16d427ac57f16268ce4060b4a3d1760ff2cd9b1743185072436`  
		Last Modified: Tue, 21 Nov 2023 11:54:28 GMT  
		Size: 4.9 MB (4881057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37767eb2f6144694ce685d9751a24751196daeb9c3b4a24cda3aa648169b599c`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac67ec8ea82fe47e96246ff7b13f0fbfe7d1fd1f42e5e299ada512bc129fb30`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:76090c55442b5a1a339e0225dbddf64ab112e7715560fa713020b6c391e56550
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37098158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c0a726f8e2e33221721363cb51bbadab29a3564c14f368b1fef9531e6e79f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:33:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 01:33:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:33:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 01:34:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:34:05 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 01:34:05 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 01:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:34:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:34:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9840676639201752d1c30641d8743f17724e8d0c4b718283519d30530b0e2ecc`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2d77be46e1eef3b22cb1d7dfa3dfa8994f40631525df55882881e81583f257`  
		Last Modified: Wed, 01 Nov 2023 01:34:21 GMT  
		Size: 2.4 MB (2434856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e264ffdd76ef3f847308508250d9ab77731cb866ad248402bf0c8fb7cff0f6`  
		Last Modified: Wed, 01 Nov 2023 01:34:21 GMT  
		Size: 5.5 MB (5482582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc3153f116074fd7762f1a27d3d9f26eb5250026557330b8bfb387d82267d4f`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d267862e7e1f6a7e6dad305f2478d4280f6c437aee2829f7cb20f0da8d7215`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:7e372aa52f1b6408dc0e2b086c878acef1c58cd04298b97ab4330722880a4cdf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38697581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14bd1e31d1ffd0aa863dc962f3eaf69bdee6fab1ba6551761353f1825b115986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:56 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Wed, 01 Nov 2023 00:38:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 14:05:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 14:05:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 14:05:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 14:05:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 14:05:47 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 14:05:48 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 14:05:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 14:05:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 14:05:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc51c75c31012b0fbe4656a6d608c47ed9dec06211b4197c7b5552d2444f51f2`  
		Last Modified: Wed, 01 Nov 2023 14:06:06 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a97bb8a3c4f684d59f1d85582646374d7102cdb7512829201a3523bf18651`  
		Last Modified: Wed, 01 Nov 2023 14:06:07 GMT  
		Size: 2.6 MB (2588117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1054b2cdb0ae435d87e3e0639b8193017b5398ee5b0eaea47fdc006106c251`  
		Last Modified: Wed, 01 Nov 2023 14:06:07 GMT  
		Size: 5.9 MB (5943824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9f1f2cd64f6ffb6a8ee7e93593a1c42d359cee8002dd892784b78a80d12227`  
		Last Modified: Wed, 01 Nov 2023 14:06:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0cc5f74c2c351a1b0b71798cc8fc19583ec35bce479af57058e5857e676b72`  
		Last Modified: Wed, 01 Nov 2023 14:06:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:0d61d0a1ea5ac2651b170d9096365703860743a0df774ddcdc327b0915c4544f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36783306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287250c56678b233b997a1c6059e730e147815a68e1df4f12eda08a5eed1ebe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:42:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 16:42:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 16:44:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 16:44:19 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 16:44:22 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 16:44:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 16:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ff2608f3497720032e30b79ae5d65cfa2c8dd359565c1c8dd638f5b3a6f0d`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab7308e1ec6dfefbe63dcd0ffdd71389fcdc64536e65a12a0d4e0b039458285`  
		Last Modified: Tue, 21 Nov 2023 16:44:46 GMT  
		Size: 1.8 MB (1834326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bede55fcddef2dca32fd1854933f48d44eb852b04607b5ca0ee5f0ceede864c`  
		Last Modified: Tue, 21 Nov 2023 16:44:49 GMT  
		Size: 5.8 MB (5805479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8ac4180d595ed6276f96e62a762ce81e1cbc8d5adb99021d674d703250377a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6377814988f39cd05c902f86328248c9751a1903ed8401e8827bf7540cc4a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:99a36d31339087c56743fcd7b09255be818296337c1ee9b0b9e5caa4d6d2a629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42336939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbf18f5d582e136651ca47bbf5c8553330ac36b69e4beb1e957d147dbc321fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:49:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 12:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:49:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 12:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:49:48 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 12:49:48 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 12:49:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 12:49:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e3e9a6e83461086d799b3c35e7086e930106125c74069a1510c25bdb6afb6d`  
		Last Modified: Tue, 21 Nov 2023 12:50:01 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956ee3303181032f855a7b2887c1bdca6910e0cb1ec3c92b65d6509c2f907abb`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 2.8 MB (2770520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ddbd7552dcc1e8096f1f690fb7a8f6d94f6b14b70ac7c130e5224ccc99ae5`  
		Last Modified: Tue, 21 Nov 2023 12:50:03 GMT  
		Size: 6.4 MB (6423216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acdb31d4ba61d5a1503eb5bf6cd716ec162f811fe2c79c2ff5c2e727033efc0`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da63bf7cb4ff2b34de84cd9caefa0d255c9965665b50f421172e3d96c2ee315a`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:e55796d4c561e3f8eec223e5e69fb5d024ac8574c4aace38477a60420ff5414c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35164381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ea59dc57dc93fac49f303c8c58d6d153d1c8a8ffab3500ff5649eb63c8b568`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:54:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:54:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:54:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:54:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:54:34 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:54:34 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:54:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:54:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a1488c1c72f51fc67f2f92a4266ad144068e6265f09a6854a0edda69d1e634`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850f941b1cd09719d174b6a90cb013528879a956734598472118c9ba95f4f146`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 2.3 MB (2262458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647d17c59a394362c94984e56f3babc4addd9e026c843bede6b3b295b4b9439c`  
		Last Modified: Tue, 21 Nov 2023 05:54:55 GMT  
		Size: 5.4 MB (5387438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5763b7fbe5d4e9c3ba3f58020db82f8a9bba3e6a9a702f785249dd13161a253b`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d519c5ded3c9d38ab8b28f40d83037fc367671ed767a048f773b935af62381f`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:b16b2ca29175a26ad03e13d64b6651b78c9aa9261830f6cc430a7cc1eec48288
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
$ docker pull spiped@sha256:cc24224bd99278e1876c04bb6e4e86ff481f441119c8bb146fcde9e97c1651ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5453362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c46e70d917fdea2bc5e8a78881181f8dc6bf82b0674e0c5ea9c251dc3230b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:40:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:40:14 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:40:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:40:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:40:24 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:40:24 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:40:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:40:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:40:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29114bf1da8c1b11e9fcf86119c5269d5142fe62d78585681a33083719709699`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d218d8f221cdfa4ebebec11e4ea188b1aff58040bf996fc7f57d072554aa8f`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 1.4 MB (1433006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d18ea945514bf50934d00103879af4f457d93a676a4a35277ca195812581acd`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 616.6 KB (616650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fa3bcf042b898d0e4caf16fe882669892864bc993826acc6bfdf349acb40ea`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9311940b5d69ae121eba7f48594543d7cbd0f043e01006ed0b8675a5e48cd244`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9df8a0a34577ec497d4f3f9c496c80e25780fb1f7f65b7b4dca4ebeac8ae1519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4991026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1406a1e174e65b701e8309b0f54ca9baedca4ad65edc6f10a353bb3d572a13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:06:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:06:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:06:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:06:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:06:12 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:06:12 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:06:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:06:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d862c0d3de0fac486d6fadbba838d9e7f39d8a7dfc4bf9b581acadbda1fa5b`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3191ed9fa9a76370d05de08851632bb6705a7774f50f7665aa9d4e8116ccb0`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.2 MB (1236779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88370d736f5a7966cfdc651335576668afabbcc66a8194b21ff91e010f4c55b8`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 607.2 KB (607212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c59b5e58ec67619e90903390555d8eb0bdb23cc0abd3d1bf00650a37e7d9b7`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195a434068a95af750df05a3f069cad835530de205cfea200155c2bbb3d17bbc`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7e217a6b1042b741dc317dbc9f5aa1d0a6e846ffb75181e5b4f5a30ecfdf527f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4638967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17d535585fee20a92f1ac79b6c94a3b1217e954e28e5a8f8078c998df038557`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:32:35 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:32:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:32:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:32:45 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:32:45 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:32:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:32:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0685d1c97bb4ab51c253c5c084c6e78be0db7a3c5791be1c9d4602fce3953b79`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980deddc51628db59e13ee670457530ea101bc22548d04eb2eb5ddb82abe598`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 1.2 MB (1163903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882273c520366a5009c0c5ffff4ce6d70e9a8172dbc529636efffede2a77696a`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 573.4 KB (573421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336e75adcb6641cba93182ecfadbbc458f58873a923a6a73ccb7c2660db3b32d`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34003432a0d18065614a57c50acd83bd03210ffdc601a0c5f14c8eca3cdd072`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b3e6d8b6dba4bb203308f2890a66da1d82b1118bfd06f4388d7bb74947459a42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5318202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2979e47c65cc5da347c11efd63887a9a5d3c9a725fdb77d77881c953a600d7af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:04:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:04:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:04:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:04:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:04:32 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:04:33 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:04:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:04:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83a0f29ff084b101d2bedb67bd954464c8ea2c833f6d9e463637ce1e3b85570`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cf75f2a3111f44f8592427f7aa844af1ebf62fa9f9866aa379e5f18d39808f`  
		Last Modified: Sat, 21 Oct 2023 03:04:45 GMT  
		Size: 1.4 MB (1362691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33a4554df0c7945678d4b7f22a6c2516b8138ea1b7e2c83c2a1f18701c9546`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 621.9 KB (621941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0902852a7093c6199857d5a4667571b9d5e3760d5aadc7e95add0b0057fc489c`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5d88ecfb88d6b48191b0de36de2710a9103aef771473701ea711287a3afe1a`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:4a64fa7debbe2222651433cc328105fe1aa8b355b63ae4bba61400f4040ea000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5226880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac627aa6486fd0f2e81ceb74df0a13d52ae058d3f0f360e08a6675b84c84e9c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:04:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 02:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 02:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 02:04:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 02:04:44 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 02:04:44 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 02:04:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 02:04:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33b43d22e223fc31335df903a86b4f1171d08db94ddae5efe5d08e9698f98c1`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04497d2dbca17493cffd45065a4e72ff59533fc06618373387f34e38f0bb1cc0`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 1.4 MB (1353884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e332fd0c16912f90a54e5b24c4dafc83d5784af7379b6be3d69a819fffe3241f`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 635.5 KB (635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc81899e8c005908b85605328231e95708866ba7922deec256bd6437ad48e73`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73737104e3f919559d15046753e769e225f3b531266273778a4ae009548336f9`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f69c272bb3ae2e9b8a177329b2b5e54dc8802654de744089994cb7228ede3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5329375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b87c1a119db9fdddaaeb16754aa4b07f637b42436a69111204d05c75c186608`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:13:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:13:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:13:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:13:41 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:13:42 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:13:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d410f45a90c70f879443ba3946c24240dbe040601a76f35dcb5a380fdc82b60`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a364f51b947cc7eba299e40137deb29c1254d4515d6ef730313422214dbeb7c7`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.4 MB (1361736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7659f4cc5c2bdbf6a67f465a448677fa9c15a6ab68580bec70ffbd57aba9a3f3`  
		Last Modified: Sat, 21 Oct 2023 01:13:59 GMT  
		Size: 619.4 KB (619386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783eb3619067a542b443f39b00f570a8ab027ee35bf4b494c7f658d9ebd6f73`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c72af5246df895d51bbbcaa58fba103965d608a0e9e4bf6b18b08f614317a5`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:98284a17fa0c80767981bd99393cd484fe002e68450233bfaea1b5a88b9b22d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5053046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb467c3a7dc5ff285adfe703953cf1ab92bf7b5d99ff8fd56c7a06b24c551713`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:08:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:08:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:08:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:08:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:08:22 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:08:22 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:08:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:08:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:08:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892540ac0e1d481800201bd26b19bff2b8fb7676da32f32627f7608c581964e`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c30da304e376763e7fb5589b18a8fe13f6efb87563b6578db8f5c52527aae34`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.2 MB (1221479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dff0df9199f69591bd6f28e91cee32ed9da4b645d33d9b7e3f0b618122f4cda`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 614.7 KB (614722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58582257555f94a55275ed46f9a805fef4b3b420a10ba1e5df6382a465b42b6d`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0658640d198e3dd6b2e5b71a78c003d7578a7ab2d3d51b3aa6620b727ebcc370`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:23daec2ad9d865e8d83dce3b3853efa6d665082b70f54b7e3a163b6f6d224069
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
$ docker pull spiped@sha256:099048569b329879479b0b1ae1d9f8192e4268013efe8de12c90b8f2278c6c3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38217263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d04e78fe52f9fb4ae91b1ccce84e9b109608505db0d56fbff3ec70f3f803610f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:49 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 01 Nov 2023 00:20:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 15:58:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 15:58:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 15:58:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 15:58:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 15:58:28 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 15:58:28 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 15:58:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 15:58:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 15:58:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee77a37e1a0fae49537f1c45d174eb2156a9f73bdb4c17cdc4848a5d79450314`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a0ee31fece3b5baa9cfb4e7b7f8aea69c34d8c742b1d77ca99b4dd37f5a31f`  
		Last Modified: Wed, 01 Nov 2023 15:58:45 GMT  
		Size: 2.6 MB (2591903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf356231cfb90da4eb4d73b452416f07680c063365c51f4c50aaea003ce539`  
		Last Modified: Wed, 01 Nov 2023 15:58:45 GMT  
		Size: 6.5 MB (6473928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a667b5364abbbc9bb0a0bf62cd773c47ec6aafdea30ae8e31de144b73429c07`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447ca94f057c4abc2edebebf17fdf11a77bbbf3793415ce61c5db3c10304761c`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a22fc52e1353a81c0b5e864f000d5b7c6f511f31d25d33161d7fff1fa66a128f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34250716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:805e4bd68f268c5a14b0391f350041c251fc5129caa5978c1f2bd4a998995836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:48:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:48:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:48:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:48:30 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:48:31 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:48:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c4d22227960e496eb464146dc866dad412f31aa91c728607dde4278de637ee`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53633f32e999cc192394918d73de2f3ad375e658d9e7dd207468ea6b664eb6d4`  
		Last Modified: Tue, 21 Nov 2023 05:48:39 GMT  
		Size: 2.2 MB (2186814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82ff098495f0ea42040c5184eb059c29c59d5d6e660aa0b1fbc7fff91b2ad4b`  
		Last Modified: Tue, 21 Nov 2023 05:48:40 GMT  
		Size: 5.1 MB (5140150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f734161b12b1fc00f0c981ce9f8176dacc5ca02b74484b806d289850efaa8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f8f249901f701b78f48d77ef49a7fe721309da08eae74507aec894e5a49af8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d49e38f255892c26d1cde15165c35c32cf857b3446c025ecbd69a009b6d59a12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31677806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97542227ddc0fffbebd6a1fa7da3015089ed0e15aa7d37d4d6c22aa77e4748e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 11:53:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 11:53:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 11:53:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 11:54:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 11:54:13 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 11:54:13 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 11:54:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 11:54:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac591a8672b5dba3bfcbe0fe6c21f8387ab9a4f56d6ea32f9eebf5e37feca3`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0fa0448ca0214cd73bf754ce7fd1d9686bd3de6b1bf5840a2c8bd3587f1109`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 2.0 MB (2046224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efda8a5518d4c16d427ac57f16268ce4060b4a3d1760ff2cd9b1743185072436`  
		Last Modified: Tue, 21 Nov 2023 11:54:28 GMT  
		Size: 4.9 MB (4881057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37767eb2f6144694ce685d9751a24751196daeb9c3b4a24cda3aa648169b599c`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac67ec8ea82fe47e96246ff7b13f0fbfe7d1fd1f42e5e299ada512bc129fb30`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:76090c55442b5a1a339e0225dbddf64ab112e7715560fa713020b6c391e56550
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37098158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c0a726f8e2e33221721363cb51bbadab29a3564c14f368b1fef9531e6e79f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:33:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 01:33:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:33:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 01:34:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:34:05 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 01:34:05 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 01:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:34:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:34:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9840676639201752d1c30641d8743f17724e8d0c4b718283519d30530b0e2ecc`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2d77be46e1eef3b22cb1d7dfa3dfa8994f40631525df55882881e81583f257`  
		Last Modified: Wed, 01 Nov 2023 01:34:21 GMT  
		Size: 2.4 MB (2434856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e264ffdd76ef3f847308508250d9ab77731cb866ad248402bf0c8fb7cff0f6`  
		Last Modified: Wed, 01 Nov 2023 01:34:21 GMT  
		Size: 5.5 MB (5482582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc3153f116074fd7762f1a27d3d9f26eb5250026557330b8bfb387d82267d4f`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d267862e7e1f6a7e6dad305f2478d4280f6c437aee2829f7cb20f0da8d7215`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:7e372aa52f1b6408dc0e2b086c878acef1c58cd04298b97ab4330722880a4cdf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38697581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14bd1e31d1ffd0aa863dc962f3eaf69bdee6fab1ba6551761353f1825b115986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:56 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Wed, 01 Nov 2023 00:38:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 14:05:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 14:05:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 14:05:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 14:05:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 14:05:47 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 14:05:48 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 14:05:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 14:05:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 14:05:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc51c75c31012b0fbe4656a6d608c47ed9dec06211b4197c7b5552d2444f51f2`  
		Last Modified: Wed, 01 Nov 2023 14:06:06 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a97bb8a3c4f684d59f1d85582646374d7102cdb7512829201a3523bf18651`  
		Last Modified: Wed, 01 Nov 2023 14:06:07 GMT  
		Size: 2.6 MB (2588117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1054b2cdb0ae435d87e3e0639b8193017b5398ee5b0eaea47fdc006106c251`  
		Last Modified: Wed, 01 Nov 2023 14:06:07 GMT  
		Size: 5.9 MB (5943824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9f1f2cd64f6ffb6a8ee7e93593a1c42d359cee8002dd892784b78a80d12227`  
		Last Modified: Wed, 01 Nov 2023 14:06:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0cc5f74c2c351a1b0b71798cc8fc19583ec35bce479af57058e5857e676b72`  
		Last Modified: Wed, 01 Nov 2023 14:06:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:0d61d0a1ea5ac2651b170d9096365703860743a0df774ddcdc327b0915c4544f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36783306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287250c56678b233b997a1c6059e730e147815a68e1df4f12eda08a5eed1ebe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:42:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 16:42:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 16:44:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 16:44:19 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 16:44:22 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 16:44:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 16:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ff2608f3497720032e30b79ae5d65cfa2c8dd359565c1c8dd638f5b3a6f0d`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab7308e1ec6dfefbe63dcd0ffdd71389fcdc64536e65a12a0d4e0b039458285`  
		Last Modified: Tue, 21 Nov 2023 16:44:46 GMT  
		Size: 1.8 MB (1834326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bede55fcddef2dca32fd1854933f48d44eb852b04607b5ca0ee5f0ceede864c`  
		Last Modified: Tue, 21 Nov 2023 16:44:49 GMT  
		Size: 5.8 MB (5805479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8ac4180d595ed6276f96e62a762ce81e1cbc8d5adb99021d674d703250377a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6377814988f39cd05c902f86328248c9751a1903ed8401e8827bf7540cc4a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:99a36d31339087c56743fcd7b09255be818296337c1ee9b0b9e5caa4d6d2a629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42336939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbf18f5d582e136651ca47bbf5c8553330ac36b69e4beb1e957d147dbc321fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:49:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 12:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:49:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 12:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:49:48 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 12:49:48 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 12:49:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 12:49:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e3e9a6e83461086d799b3c35e7086e930106125c74069a1510c25bdb6afb6d`  
		Last Modified: Tue, 21 Nov 2023 12:50:01 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956ee3303181032f855a7b2887c1bdca6910e0cb1ec3c92b65d6509c2f907abb`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 2.8 MB (2770520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ddbd7552dcc1e8096f1f690fb7a8f6d94f6b14b70ac7c130e5224ccc99ae5`  
		Last Modified: Tue, 21 Nov 2023 12:50:03 GMT  
		Size: 6.4 MB (6423216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acdb31d4ba61d5a1503eb5bf6cd716ec162f811fe2c79c2ff5c2e727033efc0`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da63bf7cb4ff2b34de84cd9caefa0d255c9965665b50f421172e3d96c2ee315a`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:e55796d4c561e3f8eec223e5e69fb5d024ac8574c4aace38477a60420ff5414c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35164381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ea59dc57dc93fac49f303c8c58d6d153d1c8a8ffab3500ff5649eb63c8b568`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:54:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:54:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:54:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:54:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:54:34 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:54:34 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:54:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:54:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a1488c1c72f51fc67f2f92a4266ad144068e6265f09a6854a0edda69d1e634`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850f941b1cd09719d174b6a90cb013528879a956734598472118c9ba95f4f146`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 2.3 MB (2262458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647d17c59a394362c94984e56f3babc4addd9e026c843bede6b3b295b4b9439c`  
		Last Modified: Tue, 21 Nov 2023 05:54:55 GMT  
		Size: 5.4 MB (5387438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5763b7fbe5d4e9c3ba3f58020db82f8a9bba3e6a9a702f785249dd13161a253b`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d519c5ded3c9d38ab8b28f40d83037fc367671ed767a048f773b935af62381f`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:b16b2ca29175a26ad03e13d64b6651b78c9aa9261830f6cc430a7cc1eec48288
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
$ docker pull spiped@sha256:cc24224bd99278e1876c04bb6e4e86ff481f441119c8bb146fcde9e97c1651ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5453362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c46e70d917fdea2bc5e8a78881181f8dc6bf82b0674e0c5ea9c251dc3230b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:40:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:40:14 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:40:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:40:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:40:24 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:40:24 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:40:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:40:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:40:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29114bf1da8c1b11e9fcf86119c5269d5142fe62d78585681a33083719709699`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d218d8f221cdfa4ebebec11e4ea188b1aff58040bf996fc7f57d072554aa8f`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 1.4 MB (1433006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d18ea945514bf50934d00103879af4f457d93a676a4a35277ca195812581acd`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 616.6 KB (616650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fa3bcf042b898d0e4caf16fe882669892864bc993826acc6bfdf349acb40ea`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9311940b5d69ae121eba7f48594543d7cbd0f043e01006ed0b8675a5e48cd244`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9df8a0a34577ec497d4f3f9c496c80e25780fb1f7f65b7b4dca4ebeac8ae1519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4991026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1406a1e174e65b701e8309b0f54ca9baedca4ad65edc6f10a353bb3d572a13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:06:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:06:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:06:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:06:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:06:12 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:06:12 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:06:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:06:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d862c0d3de0fac486d6fadbba838d9e7f39d8a7dfc4bf9b581acadbda1fa5b`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3191ed9fa9a76370d05de08851632bb6705a7774f50f7665aa9d4e8116ccb0`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.2 MB (1236779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88370d736f5a7966cfdc651335576668afabbcc66a8194b21ff91e010f4c55b8`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 607.2 KB (607212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c59b5e58ec67619e90903390555d8eb0bdb23cc0abd3d1bf00650a37e7d9b7`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195a434068a95af750df05a3f069cad835530de205cfea200155c2bbb3d17bbc`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7e217a6b1042b741dc317dbc9f5aa1d0a6e846ffb75181e5b4f5a30ecfdf527f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4638967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17d535585fee20a92f1ac79b6c94a3b1217e954e28e5a8f8078c998df038557`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:32:35 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:32:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:32:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:32:45 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:32:45 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:32:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:32:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0685d1c97bb4ab51c253c5c084c6e78be0db7a3c5791be1c9d4602fce3953b79`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980deddc51628db59e13ee670457530ea101bc22548d04eb2eb5ddb82abe598`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 1.2 MB (1163903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882273c520366a5009c0c5ffff4ce6d70e9a8172dbc529636efffede2a77696a`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 573.4 KB (573421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336e75adcb6641cba93182ecfadbbc458f58873a923a6a73ccb7c2660db3b32d`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34003432a0d18065614a57c50acd83bd03210ffdc601a0c5f14c8eca3cdd072`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b3e6d8b6dba4bb203308f2890a66da1d82b1118bfd06f4388d7bb74947459a42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5318202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2979e47c65cc5da347c11efd63887a9a5d3c9a725fdb77d77881c953a600d7af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:04:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:04:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:04:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:04:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:04:32 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:04:33 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:04:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:04:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83a0f29ff084b101d2bedb67bd954464c8ea2c833f6d9e463637ce1e3b85570`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cf75f2a3111f44f8592427f7aa844af1ebf62fa9f9866aa379e5f18d39808f`  
		Last Modified: Sat, 21 Oct 2023 03:04:45 GMT  
		Size: 1.4 MB (1362691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33a4554df0c7945678d4b7f22a6c2516b8138ea1b7e2c83c2a1f18701c9546`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 621.9 KB (621941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0902852a7093c6199857d5a4667571b9d5e3760d5aadc7e95add0b0057fc489c`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5d88ecfb88d6b48191b0de36de2710a9103aef771473701ea711287a3afe1a`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:4a64fa7debbe2222651433cc328105fe1aa8b355b63ae4bba61400f4040ea000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5226880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac627aa6486fd0f2e81ceb74df0a13d52ae058d3f0f360e08a6675b84c84e9c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:04:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 02:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 02:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 02:04:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 02:04:44 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 02:04:44 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 02:04:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 02:04:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33b43d22e223fc31335df903a86b4f1171d08db94ddae5efe5d08e9698f98c1`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04497d2dbca17493cffd45065a4e72ff59533fc06618373387f34e38f0bb1cc0`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 1.4 MB (1353884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e332fd0c16912f90a54e5b24c4dafc83d5784af7379b6be3d69a819fffe3241f`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 635.5 KB (635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc81899e8c005908b85605328231e95708866ba7922deec256bd6437ad48e73`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73737104e3f919559d15046753e769e225f3b531266273778a4ae009548336f9`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f69c272bb3ae2e9b8a177329b2b5e54dc8802654de744089994cb7228ede3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5329375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b87c1a119db9fdddaaeb16754aa4b07f637b42436a69111204d05c75c186608`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:13:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:13:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:13:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:13:41 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:13:42 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:13:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d410f45a90c70f879443ba3946c24240dbe040601a76f35dcb5a380fdc82b60`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a364f51b947cc7eba299e40137deb29c1254d4515d6ef730313422214dbeb7c7`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.4 MB (1361736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7659f4cc5c2bdbf6a67f465a448677fa9c15a6ab68580bec70ffbd57aba9a3f3`  
		Last Modified: Sat, 21 Oct 2023 01:13:59 GMT  
		Size: 619.4 KB (619386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783eb3619067a542b443f39b00f570a8ab027ee35bf4b494c7f658d9ebd6f73`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c72af5246df895d51bbbcaa58fba103965d608a0e9e4bf6b18b08f614317a5`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:98284a17fa0c80767981bd99393cd484fe002e68450233bfaea1b5a88b9b22d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5053046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb467c3a7dc5ff285adfe703953cf1ab92bf7b5d99ff8fd56c7a06b24c551713`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:08:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:08:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:08:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:08:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:08:22 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:08:22 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:08:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:08:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:08:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892540ac0e1d481800201bd26b19bff2b8fb7676da32f32627f7608c581964e`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c30da304e376763e7fb5589b18a8fe13f6efb87563b6578db8f5c52527aae34`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.2 MB (1221479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dff0df9199f69591bd6f28e91cee32ed9da4b645d33d9b7e3f0b618122f4cda`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 614.7 KB (614722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58582257555f94a55275ed46f9a805fef4b3b420a10ba1e5df6382a465b42b6d`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0658640d198e3dd6b2e5b71a78c003d7578a7ab2d3d51b3aa6620b727ebcc370`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:23daec2ad9d865e8d83dce3b3853efa6d665082b70f54b7e3a163b6f6d224069
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
$ docker pull spiped@sha256:099048569b329879479b0b1ae1d9f8192e4268013efe8de12c90b8f2278c6c3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38217263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d04e78fe52f9fb4ae91b1ccce84e9b109608505db0d56fbff3ec70f3f803610f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:49 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 01 Nov 2023 00:20:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 15:58:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 15:58:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 15:58:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 15:58:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 15:58:28 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 15:58:28 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 15:58:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 15:58:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 15:58:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee77a37e1a0fae49537f1c45d174eb2156a9f73bdb4c17cdc4848a5d79450314`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a0ee31fece3b5baa9cfb4e7b7f8aea69c34d8c742b1d77ca99b4dd37f5a31f`  
		Last Modified: Wed, 01 Nov 2023 15:58:45 GMT  
		Size: 2.6 MB (2591903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf356231cfb90da4eb4d73b452416f07680c063365c51f4c50aaea003ce539`  
		Last Modified: Wed, 01 Nov 2023 15:58:45 GMT  
		Size: 6.5 MB (6473928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a667b5364abbbc9bb0a0bf62cd773c47ec6aafdea30ae8e31de144b73429c07`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447ca94f057c4abc2edebebf17fdf11a77bbbf3793415ce61c5db3c10304761c`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a22fc52e1353a81c0b5e864f000d5b7c6f511f31d25d33161d7fff1fa66a128f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34250716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:805e4bd68f268c5a14b0391f350041c251fc5129caa5978c1f2bd4a998995836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:48:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:48:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:48:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:48:30 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:48:31 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:48:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c4d22227960e496eb464146dc866dad412f31aa91c728607dde4278de637ee`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53633f32e999cc192394918d73de2f3ad375e658d9e7dd207468ea6b664eb6d4`  
		Last Modified: Tue, 21 Nov 2023 05:48:39 GMT  
		Size: 2.2 MB (2186814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82ff098495f0ea42040c5184eb059c29c59d5d6e660aa0b1fbc7fff91b2ad4b`  
		Last Modified: Tue, 21 Nov 2023 05:48:40 GMT  
		Size: 5.1 MB (5140150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f734161b12b1fc00f0c981ce9f8176dacc5ca02b74484b806d289850efaa8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f8f249901f701b78f48d77ef49a7fe721309da08eae74507aec894e5a49af8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d49e38f255892c26d1cde15165c35c32cf857b3446c025ecbd69a009b6d59a12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31677806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97542227ddc0fffbebd6a1fa7da3015089ed0e15aa7d37d4d6c22aa77e4748e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 11:53:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 11:53:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 11:53:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 11:54:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 11:54:13 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 11:54:13 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 11:54:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 11:54:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac591a8672b5dba3bfcbe0fe6c21f8387ab9a4f56d6ea32f9eebf5e37feca3`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0fa0448ca0214cd73bf754ce7fd1d9686bd3de6b1bf5840a2c8bd3587f1109`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 2.0 MB (2046224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efda8a5518d4c16d427ac57f16268ce4060b4a3d1760ff2cd9b1743185072436`  
		Last Modified: Tue, 21 Nov 2023 11:54:28 GMT  
		Size: 4.9 MB (4881057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37767eb2f6144694ce685d9751a24751196daeb9c3b4a24cda3aa648169b599c`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac67ec8ea82fe47e96246ff7b13f0fbfe7d1fd1f42e5e299ada512bc129fb30`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:76090c55442b5a1a339e0225dbddf64ab112e7715560fa713020b6c391e56550
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37098158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c0a726f8e2e33221721363cb51bbadab29a3564c14f368b1fef9531e6e79f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:33:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 01:33:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:33:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 01:34:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:34:05 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 01:34:05 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 01:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:34:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:34:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9840676639201752d1c30641d8743f17724e8d0c4b718283519d30530b0e2ecc`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2d77be46e1eef3b22cb1d7dfa3dfa8994f40631525df55882881e81583f257`  
		Last Modified: Wed, 01 Nov 2023 01:34:21 GMT  
		Size: 2.4 MB (2434856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e264ffdd76ef3f847308508250d9ab77731cb866ad248402bf0c8fb7cff0f6`  
		Last Modified: Wed, 01 Nov 2023 01:34:21 GMT  
		Size: 5.5 MB (5482582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc3153f116074fd7762f1a27d3d9f26eb5250026557330b8bfb387d82267d4f`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d267862e7e1f6a7e6dad305f2478d4280f6c437aee2829f7cb20f0da8d7215`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:7e372aa52f1b6408dc0e2b086c878acef1c58cd04298b97ab4330722880a4cdf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38697581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14bd1e31d1ffd0aa863dc962f3eaf69bdee6fab1ba6551761353f1825b115986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:56 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Wed, 01 Nov 2023 00:38:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 14:05:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 14:05:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 14:05:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 14:05:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 14:05:47 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 14:05:48 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 14:05:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 14:05:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 14:05:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc51c75c31012b0fbe4656a6d608c47ed9dec06211b4197c7b5552d2444f51f2`  
		Last Modified: Wed, 01 Nov 2023 14:06:06 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a97bb8a3c4f684d59f1d85582646374d7102cdb7512829201a3523bf18651`  
		Last Modified: Wed, 01 Nov 2023 14:06:07 GMT  
		Size: 2.6 MB (2588117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1054b2cdb0ae435d87e3e0639b8193017b5398ee5b0eaea47fdc006106c251`  
		Last Modified: Wed, 01 Nov 2023 14:06:07 GMT  
		Size: 5.9 MB (5943824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9f1f2cd64f6ffb6a8ee7e93593a1c42d359cee8002dd892784b78a80d12227`  
		Last Modified: Wed, 01 Nov 2023 14:06:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0cc5f74c2c351a1b0b71798cc8fc19583ec35bce479af57058e5857e676b72`  
		Last Modified: Wed, 01 Nov 2023 14:06:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:0d61d0a1ea5ac2651b170d9096365703860743a0df774ddcdc327b0915c4544f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36783306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287250c56678b233b997a1c6059e730e147815a68e1df4f12eda08a5eed1ebe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:42:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 16:42:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 16:44:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 16:44:19 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 16:44:22 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 16:44:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 16:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ff2608f3497720032e30b79ae5d65cfa2c8dd359565c1c8dd638f5b3a6f0d`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab7308e1ec6dfefbe63dcd0ffdd71389fcdc64536e65a12a0d4e0b039458285`  
		Last Modified: Tue, 21 Nov 2023 16:44:46 GMT  
		Size: 1.8 MB (1834326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bede55fcddef2dca32fd1854933f48d44eb852b04607b5ca0ee5f0ceede864c`  
		Last Modified: Tue, 21 Nov 2023 16:44:49 GMT  
		Size: 5.8 MB (5805479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8ac4180d595ed6276f96e62a762ce81e1cbc8d5adb99021d674d703250377a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6377814988f39cd05c902f86328248c9751a1903ed8401e8827bf7540cc4a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:99a36d31339087c56743fcd7b09255be818296337c1ee9b0b9e5caa4d6d2a629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42336939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbf18f5d582e136651ca47bbf5c8553330ac36b69e4beb1e957d147dbc321fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:49:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 12:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:49:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 12:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:49:48 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 12:49:48 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 12:49:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 12:49:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e3e9a6e83461086d799b3c35e7086e930106125c74069a1510c25bdb6afb6d`  
		Last Modified: Tue, 21 Nov 2023 12:50:01 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956ee3303181032f855a7b2887c1bdca6910e0cb1ec3c92b65d6509c2f907abb`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 2.8 MB (2770520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ddbd7552dcc1e8096f1f690fb7a8f6d94f6b14b70ac7c130e5224ccc99ae5`  
		Last Modified: Tue, 21 Nov 2023 12:50:03 GMT  
		Size: 6.4 MB (6423216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acdb31d4ba61d5a1503eb5bf6cd716ec162f811fe2c79c2ff5c2e727033efc0`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da63bf7cb4ff2b34de84cd9caefa0d255c9965665b50f421172e3d96c2ee315a`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:e55796d4c561e3f8eec223e5e69fb5d024ac8574c4aace38477a60420ff5414c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35164381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ea59dc57dc93fac49f303c8c58d6d153d1c8a8ffab3500ff5649eb63c8b568`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:54:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:54:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:54:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:54:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:54:34 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:54:34 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:54:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:54:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a1488c1c72f51fc67f2f92a4266ad144068e6265f09a6854a0edda69d1e634`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850f941b1cd09719d174b6a90cb013528879a956734598472118c9ba95f4f146`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 2.3 MB (2262458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647d17c59a394362c94984e56f3babc4addd9e026c843bede6b3b295b4b9439c`  
		Last Modified: Tue, 21 Nov 2023 05:54:55 GMT  
		Size: 5.4 MB (5387438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5763b7fbe5d4e9c3ba3f58020db82f8a9bba3e6a9a702f785249dd13161a253b`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d519c5ded3c9d38ab8b28f40d83037fc367671ed767a048f773b935af62381f`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:b16b2ca29175a26ad03e13d64b6651b78c9aa9261830f6cc430a7cc1eec48288
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
$ docker pull spiped@sha256:cc24224bd99278e1876c04bb6e4e86ff481f441119c8bb146fcde9e97c1651ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5453362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c46e70d917fdea2bc5e8a78881181f8dc6bf82b0674e0c5ea9c251dc3230b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:40:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:40:14 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:40:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:40:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:40:24 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:40:24 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:40:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:40:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:40:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29114bf1da8c1b11e9fcf86119c5269d5142fe62d78585681a33083719709699`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d218d8f221cdfa4ebebec11e4ea188b1aff58040bf996fc7f57d072554aa8f`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 1.4 MB (1433006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d18ea945514bf50934d00103879af4f457d93a676a4a35277ca195812581acd`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 616.6 KB (616650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fa3bcf042b898d0e4caf16fe882669892864bc993826acc6bfdf349acb40ea`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9311940b5d69ae121eba7f48594543d7cbd0f043e01006ed0b8675a5e48cd244`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9df8a0a34577ec497d4f3f9c496c80e25780fb1f7f65b7b4dca4ebeac8ae1519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4991026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1406a1e174e65b701e8309b0f54ca9baedca4ad65edc6f10a353bb3d572a13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:06:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:06:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:06:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:06:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:06:12 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:06:12 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:06:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:06:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d862c0d3de0fac486d6fadbba838d9e7f39d8a7dfc4bf9b581acadbda1fa5b`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3191ed9fa9a76370d05de08851632bb6705a7774f50f7665aa9d4e8116ccb0`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.2 MB (1236779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88370d736f5a7966cfdc651335576668afabbcc66a8194b21ff91e010f4c55b8`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 607.2 KB (607212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c59b5e58ec67619e90903390555d8eb0bdb23cc0abd3d1bf00650a37e7d9b7`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195a434068a95af750df05a3f069cad835530de205cfea200155c2bbb3d17bbc`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7e217a6b1042b741dc317dbc9f5aa1d0a6e846ffb75181e5b4f5a30ecfdf527f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4638967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17d535585fee20a92f1ac79b6c94a3b1217e954e28e5a8f8078c998df038557`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:32:35 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:32:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:32:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:32:45 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:32:45 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:32:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:32:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0685d1c97bb4ab51c253c5c084c6e78be0db7a3c5791be1c9d4602fce3953b79`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980deddc51628db59e13ee670457530ea101bc22548d04eb2eb5ddb82abe598`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 1.2 MB (1163903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882273c520366a5009c0c5ffff4ce6d70e9a8172dbc529636efffede2a77696a`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 573.4 KB (573421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336e75adcb6641cba93182ecfadbbc458f58873a923a6a73ccb7c2660db3b32d`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34003432a0d18065614a57c50acd83bd03210ffdc601a0c5f14c8eca3cdd072`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b3e6d8b6dba4bb203308f2890a66da1d82b1118bfd06f4388d7bb74947459a42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5318202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2979e47c65cc5da347c11efd63887a9a5d3c9a725fdb77d77881c953a600d7af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:04:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:04:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:04:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:04:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:04:32 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:04:33 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:04:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:04:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83a0f29ff084b101d2bedb67bd954464c8ea2c833f6d9e463637ce1e3b85570`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cf75f2a3111f44f8592427f7aa844af1ebf62fa9f9866aa379e5f18d39808f`  
		Last Modified: Sat, 21 Oct 2023 03:04:45 GMT  
		Size: 1.4 MB (1362691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33a4554df0c7945678d4b7f22a6c2516b8138ea1b7e2c83c2a1f18701c9546`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 621.9 KB (621941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0902852a7093c6199857d5a4667571b9d5e3760d5aadc7e95add0b0057fc489c`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5d88ecfb88d6b48191b0de36de2710a9103aef771473701ea711287a3afe1a`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:4a64fa7debbe2222651433cc328105fe1aa8b355b63ae4bba61400f4040ea000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5226880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac627aa6486fd0f2e81ceb74df0a13d52ae058d3f0f360e08a6675b84c84e9c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:04:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 02:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 02:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 02:04:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 02:04:44 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 02:04:44 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 02:04:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 02:04:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33b43d22e223fc31335df903a86b4f1171d08db94ddae5efe5d08e9698f98c1`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04497d2dbca17493cffd45065a4e72ff59533fc06618373387f34e38f0bb1cc0`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 1.4 MB (1353884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e332fd0c16912f90a54e5b24c4dafc83d5784af7379b6be3d69a819fffe3241f`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 635.5 KB (635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc81899e8c005908b85605328231e95708866ba7922deec256bd6437ad48e73`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73737104e3f919559d15046753e769e225f3b531266273778a4ae009548336f9`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f69c272bb3ae2e9b8a177329b2b5e54dc8802654de744089994cb7228ede3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5329375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b87c1a119db9fdddaaeb16754aa4b07f637b42436a69111204d05c75c186608`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:13:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:13:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:13:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:13:41 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:13:42 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:13:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d410f45a90c70f879443ba3946c24240dbe040601a76f35dcb5a380fdc82b60`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a364f51b947cc7eba299e40137deb29c1254d4515d6ef730313422214dbeb7c7`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.4 MB (1361736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7659f4cc5c2bdbf6a67f465a448677fa9c15a6ab68580bec70ffbd57aba9a3f3`  
		Last Modified: Sat, 21 Oct 2023 01:13:59 GMT  
		Size: 619.4 KB (619386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783eb3619067a542b443f39b00f570a8ab027ee35bf4b494c7f658d9ebd6f73`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c72af5246df895d51bbbcaa58fba103965d608a0e9e4bf6b18b08f614317a5`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:98284a17fa0c80767981bd99393cd484fe002e68450233bfaea1b5a88b9b22d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5053046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb467c3a7dc5ff285adfe703953cf1ab92bf7b5d99ff8fd56c7a06b24c551713`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:08:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:08:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:08:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:08:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:08:22 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:08:22 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:08:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:08:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:08:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892540ac0e1d481800201bd26b19bff2b8fb7676da32f32627f7608c581964e`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c30da304e376763e7fb5589b18a8fe13f6efb87563b6578db8f5c52527aae34`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.2 MB (1221479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dff0df9199f69591bd6f28e91cee32ed9da4b645d33d9b7e3f0b618122f4cda`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 614.7 KB (614722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58582257555f94a55275ed46f9a805fef4b3b420a10ba1e5df6382a465b42b6d`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0658640d198e3dd6b2e5b71a78c003d7578a7ab2d3d51b3aa6620b727ebcc370`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:b16b2ca29175a26ad03e13d64b6651b78c9aa9261830f6cc430a7cc1eec48288
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
$ docker pull spiped@sha256:cc24224bd99278e1876c04bb6e4e86ff481f441119c8bb146fcde9e97c1651ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5453362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c46e70d917fdea2bc5e8a78881181f8dc6bf82b0674e0c5ea9c251dc3230b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:40:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:40:14 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:40:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:40:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:40:24 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:40:24 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:40:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:40:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:40:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29114bf1da8c1b11e9fcf86119c5269d5142fe62d78585681a33083719709699`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d218d8f221cdfa4ebebec11e4ea188b1aff58040bf996fc7f57d072554aa8f`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 1.4 MB (1433006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d18ea945514bf50934d00103879af4f457d93a676a4a35277ca195812581acd`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 616.6 KB (616650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fa3bcf042b898d0e4caf16fe882669892864bc993826acc6bfdf349acb40ea`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9311940b5d69ae121eba7f48594543d7cbd0f043e01006ed0b8675a5e48cd244`  
		Last Modified: Sat, 21 Oct 2023 03:40:36 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9df8a0a34577ec497d4f3f9c496c80e25780fb1f7f65b7b4dca4ebeac8ae1519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4991026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1406a1e174e65b701e8309b0f54ca9baedca4ad65edc6f10a353bb3d572a13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:06:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:06:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:06:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:06:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:06:12 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:06:12 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:06:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:06:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d862c0d3de0fac486d6fadbba838d9e7f39d8a7dfc4bf9b581acadbda1fa5b`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3191ed9fa9a76370d05de08851632bb6705a7774f50f7665aa9d4e8116ccb0`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.2 MB (1236779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88370d736f5a7966cfdc651335576668afabbcc66a8194b21ff91e010f4c55b8`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 607.2 KB (607212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c59b5e58ec67619e90903390555d8eb0bdb23cc0abd3d1bf00650a37e7d9b7`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195a434068a95af750df05a3f069cad835530de205cfea200155c2bbb3d17bbc`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7e217a6b1042b741dc317dbc9f5aa1d0a6e846ffb75181e5b4f5a30ecfdf527f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4638967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17d535585fee20a92f1ac79b6c94a3b1217e954e28e5a8f8078c998df038557`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:32:35 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:32:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:32:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:32:45 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:32:45 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:32:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:32:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0685d1c97bb4ab51c253c5c084c6e78be0db7a3c5791be1c9d4602fce3953b79`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980deddc51628db59e13ee670457530ea101bc22548d04eb2eb5ddb82abe598`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 1.2 MB (1163903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882273c520366a5009c0c5ffff4ce6d70e9a8172dbc529636efffede2a77696a`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 573.4 KB (573421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336e75adcb6641cba93182ecfadbbc458f58873a923a6a73ccb7c2660db3b32d`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34003432a0d18065614a57c50acd83bd03210ffdc601a0c5f14c8eca3cdd072`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b3e6d8b6dba4bb203308f2890a66da1d82b1118bfd06f4388d7bb74947459a42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5318202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2979e47c65cc5da347c11efd63887a9a5d3c9a725fdb77d77881c953a600d7af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:04:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:04:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:04:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:04:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:04:32 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:04:33 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:04:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:04:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83a0f29ff084b101d2bedb67bd954464c8ea2c833f6d9e463637ce1e3b85570`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cf75f2a3111f44f8592427f7aa844af1ebf62fa9f9866aa379e5f18d39808f`  
		Last Modified: Sat, 21 Oct 2023 03:04:45 GMT  
		Size: 1.4 MB (1362691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33a4554df0c7945678d4b7f22a6c2516b8138ea1b7e2c83c2a1f18701c9546`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 621.9 KB (621941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0902852a7093c6199857d5a4667571b9d5e3760d5aadc7e95add0b0057fc489c`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5d88ecfb88d6b48191b0de36de2710a9103aef771473701ea711287a3afe1a`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:4a64fa7debbe2222651433cc328105fe1aa8b355b63ae4bba61400f4040ea000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5226880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac627aa6486fd0f2e81ceb74df0a13d52ae058d3f0f360e08a6675b84c84e9c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:04:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 02:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 02:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 02:04:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 02:04:44 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 02:04:44 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 02:04:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 02:04:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33b43d22e223fc31335df903a86b4f1171d08db94ddae5efe5d08e9698f98c1`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04497d2dbca17493cffd45065a4e72ff59533fc06618373387f34e38f0bb1cc0`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 1.4 MB (1353884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e332fd0c16912f90a54e5b24c4dafc83d5784af7379b6be3d69a819fffe3241f`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 635.5 KB (635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc81899e8c005908b85605328231e95708866ba7922deec256bd6437ad48e73`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73737104e3f919559d15046753e769e225f3b531266273778a4ae009548336f9`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f69c272bb3ae2e9b8a177329b2b5e54dc8802654de744089994cb7228ede3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5329375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b87c1a119db9fdddaaeb16754aa4b07f637b42436a69111204d05c75c186608`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:13:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:13:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:13:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:13:41 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:13:42 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:13:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d410f45a90c70f879443ba3946c24240dbe040601a76f35dcb5a380fdc82b60`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a364f51b947cc7eba299e40137deb29c1254d4515d6ef730313422214dbeb7c7`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.4 MB (1361736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7659f4cc5c2bdbf6a67f465a448677fa9c15a6ab68580bec70ffbd57aba9a3f3`  
		Last Modified: Sat, 21 Oct 2023 01:13:59 GMT  
		Size: 619.4 KB (619386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783eb3619067a542b443f39b00f570a8ab027ee35bf4b494c7f658d9ebd6f73`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c72af5246df895d51bbbcaa58fba103965d608a0e9e4bf6b18b08f614317a5`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:98284a17fa0c80767981bd99393cd484fe002e68450233bfaea1b5a88b9b22d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5053046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb467c3a7dc5ff285adfe703953cf1ab92bf7b5d99ff8fd56c7a06b24c551713`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:08:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:08:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:08:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:08:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:08:22 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:08:22 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:08:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:08:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:08:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892540ac0e1d481800201bd26b19bff2b8fb7676da32f32627f7608c581964e`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c30da304e376763e7fb5589b18a8fe13f6efb87563b6578db8f5c52527aae34`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.2 MB (1221479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dff0df9199f69591bd6f28e91cee32ed9da4b645d33d9b7e3f0b618122f4cda`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 614.7 KB (614722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58582257555f94a55275ed46f9a805fef4b3b420a10ba1e5df6382a465b42b6d`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0658640d198e3dd6b2e5b71a78c003d7578a7ab2d3d51b3aa6620b727ebcc370`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:23daec2ad9d865e8d83dce3b3853efa6d665082b70f54b7e3a163b6f6d224069
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
$ docker pull spiped@sha256:099048569b329879479b0b1ae1d9f8192e4268013efe8de12c90b8f2278c6c3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38217263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d04e78fe52f9fb4ae91b1ccce84e9b109608505db0d56fbff3ec70f3f803610f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:49 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 01 Nov 2023 00:20:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 15:58:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 15:58:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 15:58:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 15:58:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 15:58:28 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 15:58:28 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 15:58:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 15:58:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 15:58:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee77a37e1a0fae49537f1c45d174eb2156a9f73bdb4c17cdc4848a5d79450314`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a0ee31fece3b5baa9cfb4e7b7f8aea69c34d8c742b1d77ca99b4dd37f5a31f`  
		Last Modified: Wed, 01 Nov 2023 15:58:45 GMT  
		Size: 2.6 MB (2591903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf356231cfb90da4eb4d73b452416f07680c063365c51f4c50aaea003ce539`  
		Last Modified: Wed, 01 Nov 2023 15:58:45 GMT  
		Size: 6.5 MB (6473928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a667b5364abbbc9bb0a0bf62cd773c47ec6aafdea30ae8e31de144b73429c07`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447ca94f057c4abc2edebebf17fdf11a77bbbf3793415ce61c5db3c10304761c`  
		Last Modified: Wed, 01 Nov 2023 15:58:44 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a22fc52e1353a81c0b5e864f000d5b7c6f511f31d25d33161d7fff1fa66a128f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34250716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:805e4bd68f268c5a14b0391f350041c251fc5129caa5978c1f2bd4a998995836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:48:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:48:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:48:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:48:30 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:48:31 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:48:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c4d22227960e496eb464146dc866dad412f31aa91c728607dde4278de637ee`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53633f32e999cc192394918d73de2f3ad375e658d9e7dd207468ea6b664eb6d4`  
		Last Modified: Tue, 21 Nov 2023 05:48:39 GMT  
		Size: 2.2 MB (2186814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82ff098495f0ea42040c5184eb059c29c59d5d6e660aa0b1fbc7fff91b2ad4b`  
		Last Modified: Tue, 21 Nov 2023 05:48:40 GMT  
		Size: 5.1 MB (5140150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f734161b12b1fc00f0c981ce9f8176dacc5ca02b74484b806d289850efaa8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f8f249901f701b78f48d77ef49a7fe721309da08eae74507aec894e5a49af8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d49e38f255892c26d1cde15165c35c32cf857b3446c025ecbd69a009b6d59a12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31677806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97542227ddc0fffbebd6a1fa7da3015089ed0e15aa7d37d4d6c22aa77e4748e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 11:53:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 11:53:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 11:53:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 11:54:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 11:54:13 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 11:54:13 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 11:54:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 11:54:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac591a8672b5dba3bfcbe0fe6c21f8387ab9a4f56d6ea32f9eebf5e37feca3`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0fa0448ca0214cd73bf754ce7fd1d9686bd3de6b1bf5840a2c8bd3587f1109`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 2.0 MB (2046224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efda8a5518d4c16d427ac57f16268ce4060b4a3d1760ff2cd9b1743185072436`  
		Last Modified: Tue, 21 Nov 2023 11:54:28 GMT  
		Size: 4.9 MB (4881057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37767eb2f6144694ce685d9751a24751196daeb9c3b4a24cda3aa648169b599c`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac67ec8ea82fe47e96246ff7b13f0fbfe7d1fd1f42e5e299ada512bc129fb30`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:76090c55442b5a1a339e0225dbddf64ab112e7715560fa713020b6c391e56550
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37098158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c0a726f8e2e33221721363cb51bbadab29a3564c14f368b1fef9531e6e79f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:33:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 01:33:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:33:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 01:34:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:34:05 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 01:34:05 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 01:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:34:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:34:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9840676639201752d1c30641d8743f17724e8d0c4b718283519d30530b0e2ecc`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2d77be46e1eef3b22cb1d7dfa3dfa8994f40631525df55882881e81583f257`  
		Last Modified: Wed, 01 Nov 2023 01:34:21 GMT  
		Size: 2.4 MB (2434856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e264ffdd76ef3f847308508250d9ab77731cb866ad248402bf0c8fb7cff0f6`  
		Last Modified: Wed, 01 Nov 2023 01:34:21 GMT  
		Size: 5.5 MB (5482582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc3153f116074fd7762f1a27d3d9f26eb5250026557330b8bfb387d82267d4f`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d267862e7e1f6a7e6dad305f2478d4280f6c437aee2829f7cb20f0da8d7215`  
		Last Modified: Wed, 01 Nov 2023 01:34:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:7e372aa52f1b6408dc0e2b086c878acef1c58cd04298b97ab4330722880a4cdf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38697581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14bd1e31d1ffd0aa863dc962f3eaf69bdee6fab1ba6551761353f1825b115986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:56 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Wed, 01 Nov 2023 00:38:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 14:05:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Nov 2023 14:05:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 14:05:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Nov 2023 14:05:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 14:05:47 GMT
VOLUME [/spiped]
# Wed, 01 Nov 2023 14:05:48 GMT
WORKDIR /spiped
# Wed, 01 Nov 2023 14:05:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Nov 2023 14:05:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 14:05:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc51c75c31012b0fbe4656a6d608c47ed9dec06211b4197c7b5552d2444f51f2`  
		Last Modified: Wed, 01 Nov 2023 14:06:06 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a97bb8a3c4f684d59f1d85582646374d7102cdb7512829201a3523bf18651`  
		Last Modified: Wed, 01 Nov 2023 14:06:07 GMT  
		Size: 2.6 MB (2588117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1054b2cdb0ae435d87e3e0639b8193017b5398ee5b0eaea47fdc006106c251`  
		Last Modified: Wed, 01 Nov 2023 14:06:07 GMT  
		Size: 5.9 MB (5943824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9f1f2cd64f6ffb6a8ee7e93593a1c42d359cee8002dd892784b78a80d12227`  
		Last Modified: Wed, 01 Nov 2023 14:06:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0cc5f74c2c351a1b0b71798cc8fc19583ec35bce479af57058e5857e676b72`  
		Last Modified: Wed, 01 Nov 2023 14:06:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:0d61d0a1ea5ac2651b170d9096365703860743a0df774ddcdc327b0915c4544f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36783306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287250c56678b233b997a1c6059e730e147815a68e1df4f12eda08a5eed1ebe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:42:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 16:42:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 16:44:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 16:44:19 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 16:44:22 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 16:44:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 16:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ff2608f3497720032e30b79ae5d65cfa2c8dd359565c1c8dd638f5b3a6f0d`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab7308e1ec6dfefbe63dcd0ffdd71389fcdc64536e65a12a0d4e0b039458285`  
		Last Modified: Tue, 21 Nov 2023 16:44:46 GMT  
		Size: 1.8 MB (1834326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bede55fcddef2dca32fd1854933f48d44eb852b04607b5ca0ee5f0ceede864c`  
		Last Modified: Tue, 21 Nov 2023 16:44:49 GMT  
		Size: 5.8 MB (5805479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8ac4180d595ed6276f96e62a762ce81e1cbc8d5adb99021d674d703250377a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6377814988f39cd05c902f86328248c9751a1903ed8401e8827bf7540cc4a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:99a36d31339087c56743fcd7b09255be818296337c1ee9b0b9e5caa4d6d2a629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42336939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbf18f5d582e136651ca47bbf5c8553330ac36b69e4beb1e957d147dbc321fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:49:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 12:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:49:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 12:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:49:48 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 12:49:48 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 12:49:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 12:49:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e3e9a6e83461086d799b3c35e7086e930106125c74069a1510c25bdb6afb6d`  
		Last Modified: Tue, 21 Nov 2023 12:50:01 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956ee3303181032f855a7b2887c1bdca6910e0cb1ec3c92b65d6509c2f907abb`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 2.8 MB (2770520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ddbd7552dcc1e8096f1f690fb7a8f6d94f6b14b70ac7c130e5224ccc99ae5`  
		Last Modified: Tue, 21 Nov 2023 12:50:03 GMT  
		Size: 6.4 MB (6423216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acdb31d4ba61d5a1503eb5bf6cd716ec162f811fe2c79c2ff5c2e727033efc0`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da63bf7cb4ff2b34de84cd9caefa0d255c9965665b50f421172e3d96c2ee315a`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:e55796d4c561e3f8eec223e5e69fb5d024ac8574c4aace38477a60420ff5414c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35164381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ea59dc57dc93fac49f303c8c58d6d153d1c8a8ffab3500ff5649eb63c8b568`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:54:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:54:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:54:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:54:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:54:34 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:54:34 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:54:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:54:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a1488c1c72f51fc67f2f92a4266ad144068e6265f09a6854a0edda69d1e634`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850f941b1cd09719d174b6a90cb013528879a956734598472118c9ba95f4f146`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 2.3 MB (2262458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647d17c59a394362c94984e56f3babc4addd9e026c843bede6b3b295b4b9439c`  
		Last Modified: Tue, 21 Nov 2023 05:54:55 GMT  
		Size: 5.4 MB (5387438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5763b7fbe5d4e9c3ba3f58020db82f8a9bba3e6a9a702f785249dd13161a253b`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d519c5ded3c9d38ab8b28f40d83037fc367671ed767a048f773b935af62381f`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
