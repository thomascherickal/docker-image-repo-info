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
$ docker pull spiped@sha256:f6245dc244c77e9f4e90df27aae9438deedc5d6e955fef943fbe91e2d6ae8f30
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
$ docker pull spiped@sha256:2a1562d9a8c8bc88d3d6dd14ca19efb88a99fc683968c7e5c5bb643954121da8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36273352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c227ab9e0eaf1b392d1b5ad6a0c3ce294258575158df25fb6c6d0654ee53e911`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 16:10:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 16:10:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:10:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 16:10:12 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 16:10:13 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 16:10:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 16:10:44 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 16:10:44 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 16:10:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:10:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:10:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3417f37af9b9596fad115617f18df29172cc46a854cdc7055a23f38145a58f7`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed5044f1165e0e44070848df158eac6e4c5ec565dede6fe9b50224d8089d26c`  
		Last Modified: Wed, 18 Nov 2020 16:11:04 GMT  
		Size: 2.1 MB (2128095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db2077c0ed9103b638fe9f16fe236d093e5d52832f7df0295e05f0ede70ff45`  
		Last Modified: Wed, 18 Nov 2020 16:11:05 GMT  
		Size: 7.0 MB (7037598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4bad379660d3c468029ddb245cf2b551b49d9b11a892e0c3ab55d00816d856`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4787b232f101a29c0a4c7ca9a61effad8f7bbb98ef9f83a613b1815b923c38d`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:8382a6d947e1325a13a4418514b4e1778ca88be8206102eb0e3d3372ecc45ae9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32165056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33d4b761eea34290114eb674784d79a9ba452ccfc459a243cb5c63ef7589073`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 03:18:34 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 03:18:36 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 03:18:37 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 03:18:38 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 03:19:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 03:19:44 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 03:19:46 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 03:19:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:19:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db33d41ae1e9c76b9469640f87f593bb4644e3085f6a94fc2ed1985923392019`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e63c2f068f85d42076f8db5942ea78c569062bb6a52233f11c6baa2837c949`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 1.8 MB (1839441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bd0e0488057327d00c2c57a4d54689cbfc3bf3191ed03cb5f3461b70ee4a14`  
		Last Modified: Fri, 11 Dec 2020 03:20:13 GMT  
		Size: 5.5 MB (5479951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e867722c47de78ee7eddc4dabbed59b1c64da9e19394ea95d06872535d363`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe8c65d2ad6f0615a68f49a04f3388fedbe1fda01bbfd203fc4487a775ce6b`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c92653d99274d40ed92e53b51cd458c1c727bd16db66392e4ece2f0b00be2bba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29761232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2661d3a07d889d24fd48344b6e5491127cb4f992b7c6792f931e16aed75e01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:11:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 07:12:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:12:02 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 07:12:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 07:12:49 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 07:12:50 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 07:12:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 07:12:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 07:12:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cf66057f794f2070347e36745e45359107e121bbf72ef76a056d4d4fc427c8`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d27f2deb7663af698a4e93d06d910420b62eff5f2514cf63280715267d5e70`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2c064480e805187730287fd350b20cc30e1d074b9bf0a28d1d2a9a99934bc`  
		Last Modified: Wed, 18 Nov 2020 07:13:11 GMT  
		Size: 5.3 MB (5285408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c3e496f6405bc525c1b47e008b53a0702b5b3bad600d201daaefffd563a900`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070369842a89c55f148641e29030bb3456430e5b407bca9462c0845656ffa901`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:704c22b8b676b28651bdfbc6c270305a1d9c51dd839140ea45ac633c07afa4fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdf237415bc56dd43224e7632a35235757d01c6868a15b0053e72466291cd22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 16:23:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 16:24:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:24:08 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 16:24:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 16:24:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 16:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 16:25:23 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 16:25:34 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 16:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:25:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:25:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b998896ae01086d1d742538d6adf34407de566efe82ebee5c53075ea9cdf1cf`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09275dfac82d12984d43305a0c4751236ff1270dfa9d4233c677b164cbd7b997`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 2.0 MB (2007845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0a55a486b4a21452caace28f1c3f2202530083726583e2a4cd34ea385c9df`  
		Last Modified: Wed, 18 Nov 2020 16:26:11 GMT  
		Size: 5.9 MB (5905523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcab3d8fdb677571f99ea2d30d6662ffc0707ad0bc61ce5daf5793fd5ad700a`  
		Last Modified: Wed, 18 Nov 2020 16:26:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc91fb24b5ded88e1a0ae7d5da9a99894c51155f175d6485b1f2882bab175b3`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:eddfe3c52b1f4b047ef49c6894ac40c53dae8caa677970de4764755a754e2d13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41533953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9f2903e64f88c4e2273df5e291e5b21389aab4d0a9650d5208dc6b9554981a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:58:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 02:58:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:58:29 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 02:59:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 02:59:14 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 02:59:14 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 02:59:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 02:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 02:59:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264b3982a6da8264a3a2509542dd8f472e2d82b36d7390aae536e3610041397`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a88c082c81069b5976f79f328a9b78f7cb1c5f3401419d2f93e4bd215f38c6`  
		Last Modified: Wed, 18 Nov 2020 02:59:41 GMT  
		Size: 2.1 MB (2132327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574d0a70d657cc4f156f932200e3fb841eacd020f9786fda644f94670ea16967`  
		Last Modified: Wed, 18 Nov 2020 02:59:46 GMT  
		Size: 11.6 MB (11633270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08225d6c4b1f5a1e4901290593a71354dd7c6c676ad0319b46ca6f412e3b7ddc`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02262d310542335fc2631f9f33cc647034e6d1631581742ac01cc8aead9aac83`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:243dc5166fb19dded5aa7f688c64f8b13bf15e99a113733d155ab74f1f168a20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33907845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b92b94ba5487463c171553956b8c9a332f44c401cb8db357c44f7c19a570229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:59:15 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:59:27 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 23:00:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 23:00:36 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 23:00:36 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 23:00:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 23:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 23:00:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9c786dc23ade88d3972745848ed18089b024099778eb9bf9d5c735c7c4614`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2f2cc0e46aaf9c5d0d01e3ff5c89071efebe06cb0ea5051f316c674af976b`  
		Last Modified: Tue, 17 Nov 2020 23:01:03 GMT  
		Size: 1.7 MB (1712030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e296927f1a689719138bc125a62b2d185095d494c1a18e511c2892e5f7e6ebc`  
		Last Modified: Tue, 17 Nov 2020 23:01:09 GMT  
		Size: 6.4 MB (6416166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2df2217335c02b14a90f6c1795f3149d71d77ba2611651c6a679b4bcca6d78`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d899f01843caa25aba126202c9fb34048dffe56d82e9d6296c2ec3177157c39`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:801fff27925c8e87ed9c5de2b32b74b636299c69fdbae15c814213d2086e2ca9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39495394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e191926eaea1d0c33716adeb209444a2e64bfae48ecff245fd0ce5f35af1afc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:22:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 04:23:00 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 04:23:04 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:23:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:23:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:25:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 04:25:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:26:04 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:26:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:26:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:26:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8f5dac353b2538492cef6c8c584ca52b4b8a09452919772325c53333df359b`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51102f02eff28acc6eb89231a81a67a0f7586b40ec7c9406c5e73657b73f92c1`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 2.2 MB (2225214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec749be77d5a19cc47dedd00097160b1f0220d9d05ab73bd0d939594be46734f`  
		Last Modified: Fri, 11 Dec 2020 04:28:19 GMT  
		Size: 6.7 MB (6743253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6015004f4454ca6970c723ed1af34bbf7503bca68db79498b742edb6ce292c65`  
		Last Modified: Fri, 11 Dec 2020 04:28:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295c5c4333284617f343979a2ae448d1fbdb1580e6c6c41b24d15ee91c92029`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:e5008218bf420fafef6e87be629d8903d86b569f0a9e40adbd1302232fa9cb9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33481724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd0372682fb7ea9fbfeaa397b5fc426f5122b085df6c1ff7f4de4f8090e636e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 10:58:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 10:58:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:58:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 10:59:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 10:59:30 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 10:59:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:59:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 10:59:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b255ec039014b2ee98780609b6f7de5cfab1b7b38fd7004fdcf45ce1c9ecd6`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eeb81cfe4b40e78820d915e9bbf7799a22f74efcf8961799d7793d0a7b8d15`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.8 MB (1822007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4842d7c98c1db5b645a2bac4af45c5527ca36c0dabd0283998140df3b1245`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 5.9 MB (5943547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0cd6f3eb08cee56cf437100ba2abf610e71292759383a37248b31003b12347`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a46ada40dc3e992f07c972f362b7bb857e6f5649b38687ce9519f8948d0972`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:f6245dc244c77e9f4e90df27aae9438deedc5d6e955fef943fbe91e2d6ae8f30
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
$ docker pull spiped@sha256:2a1562d9a8c8bc88d3d6dd14ca19efb88a99fc683968c7e5c5bb643954121da8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36273352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c227ab9e0eaf1b392d1b5ad6a0c3ce294258575158df25fb6c6d0654ee53e911`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 16:10:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 16:10:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:10:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 16:10:12 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 16:10:13 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 16:10:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 16:10:44 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 16:10:44 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 16:10:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:10:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:10:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3417f37af9b9596fad115617f18df29172cc46a854cdc7055a23f38145a58f7`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed5044f1165e0e44070848df158eac6e4c5ec565dede6fe9b50224d8089d26c`  
		Last Modified: Wed, 18 Nov 2020 16:11:04 GMT  
		Size: 2.1 MB (2128095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db2077c0ed9103b638fe9f16fe236d093e5d52832f7df0295e05f0ede70ff45`  
		Last Modified: Wed, 18 Nov 2020 16:11:05 GMT  
		Size: 7.0 MB (7037598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4bad379660d3c468029ddb245cf2b551b49d9b11a892e0c3ab55d00816d856`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4787b232f101a29c0a4c7ca9a61effad8f7bbb98ef9f83a613b1815b923c38d`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:8382a6d947e1325a13a4418514b4e1778ca88be8206102eb0e3d3372ecc45ae9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32165056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33d4b761eea34290114eb674784d79a9ba452ccfc459a243cb5c63ef7589073`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 03:18:34 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 03:18:36 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 03:18:37 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 03:18:38 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 03:19:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 03:19:44 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 03:19:46 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 03:19:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:19:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db33d41ae1e9c76b9469640f87f593bb4644e3085f6a94fc2ed1985923392019`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e63c2f068f85d42076f8db5942ea78c569062bb6a52233f11c6baa2837c949`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 1.8 MB (1839441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bd0e0488057327d00c2c57a4d54689cbfc3bf3191ed03cb5f3461b70ee4a14`  
		Last Modified: Fri, 11 Dec 2020 03:20:13 GMT  
		Size: 5.5 MB (5479951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e867722c47de78ee7eddc4dabbed59b1c64da9e19394ea95d06872535d363`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe8c65d2ad6f0615a68f49a04f3388fedbe1fda01bbfd203fc4487a775ce6b`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c92653d99274d40ed92e53b51cd458c1c727bd16db66392e4ece2f0b00be2bba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29761232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2661d3a07d889d24fd48344b6e5491127cb4f992b7c6792f931e16aed75e01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:11:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 07:12:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:12:02 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 07:12:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 07:12:49 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 07:12:50 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 07:12:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 07:12:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 07:12:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cf66057f794f2070347e36745e45359107e121bbf72ef76a056d4d4fc427c8`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d27f2deb7663af698a4e93d06d910420b62eff5f2514cf63280715267d5e70`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2c064480e805187730287fd350b20cc30e1d074b9bf0a28d1d2a9a99934bc`  
		Last Modified: Wed, 18 Nov 2020 07:13:11 GMT  
		Size: 5.3 MB (5285408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c3e496f6405bc525c1b47e008b53a0702b5b3bad600d201daaefffd563a900`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070369842a89c55f148641e29030bb3456430e5b407bca9462c0845656ffa901`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:704c22b8b676b28651bdfbc6c270305a1d9c51dd839140ea45ac633c07afa4fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdf237415bc56dd43224e7632a35235757d01c6868a15b0053e72466291cd22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 16:23:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 16:24:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:24:08 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 16:24:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 16:24:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 16:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 16:25:23 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 16:25:34 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 16:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:25:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:25:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b998896ae01086d1d742538d6adf34407de566efe82ebee5c53075ea9cdf1cf`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09275dfac82d12984d43305a0c4751236ff1270dfa9d4233c677b164cbd7b997`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 2.0 MB (2007845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0a55a486b4a21452caace28f1c3f2202530083726583e2a4cd34ea385c9df`  
		Last Modified: Wed, 18 Nov 2020 16:26:11 GMT  
		Size: 5.9 MB (5905523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcab3d8fdb677571f99ea2d30d6662ffc0707ad0bc61ce5daf5793fd5ad700a`  
		Last Modified: Wed, 18 Nov 2020 16:26:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc91fb24b5ded88e1a0ae7d5da9a99894c51155f175d6485b1f2882bab175b3`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:eddfe3c52b1f4b047ef49c6894ac40c53dae8caa677970de4764755a754e2d13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41533953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9f2903e64f88c4e2273df5e291e5b21389aab4d0a9650d5208dc6b9554981a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:58:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 02:58:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:58:29 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 02:59:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 02:59:14 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 02:59:14 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 02:59:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 02:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 02:59:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264b3982a6da8264a3a2509542dd8f472e2d82b36d7390aae536e3610041397`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a88c082c81069b5976f79f328a9b78f7cb1c5f3401419d2f93e4bd215f38c6`  
		Last Modified: Wed, 18 Nov 2020 02:59:41 GMT  
		Size: 2.1 MB (2132327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574d0a70d657cc4f156f932200e3fb841eacd020f9786fda644f94670ea16967`  
		Last Modified: Wed, 18 Nov 2020 02:59:46 GMT  
		Size: 11.6 MB (11633270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08225d6c4b1f5a1e4901290593a71354dd7c6c676ad0319b46ca6f412e3b7ddc`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02262d310542335fc2631f9f33cc647034e6d1631581742ac01cc8aead9aac83`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:243dc5166fb19dded5aa7f688c64f8b13bf15e99a113733d155ab74f1f168a20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33907845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b92b94ba5487463c171553956b8c9a332f44c401cb8db357c44f7c19a570229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:59:15 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:59:27 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 23:00:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 23:00:36 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 23:00:36 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 23:00:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 23:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 23:00:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9c786dc23ade88d3972745848ed18089b024099778eb9bf9d5c735c7c4614`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2f2cc0e46aaf9c5d0d01e3ff5c89071efebe06cb0ea5051f316c674af976b`  
		Last Modified: Tue, 17 Nov 2020 23:01:03 GMT  
		Size: 1.7 MB (1712030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e296927f1a689719138bc125a62b2d185095d494c1a18e511c2892e5f7e6ebc`  
		Last Modified: Tue, 17 Nov 2020 23:01:09 GMT  
		Size: 6.4 MB (6416166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2df2217335c02b14a90f6c1795f3149d71d77ba2611651c6a679b4bcca6d78`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d899f01843caa25aba126202c9fb34048dffe56d82e9d6296c2ec3177157c39`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:801fff27925c8e87ed9c5de2b32b74b636299c69fdbae15c814213d2086e2ca9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39495394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e191926eaea1d0c33716adeb209444a2e64bfae48ecff245fd0ce5f35af1afc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:22:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 04:23:00 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 04:23:04 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:23:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:23:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:25:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 04:25:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:26:04 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:26:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:26:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:26:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8f5dac353b2538492cef6c8c584ca52b4b8a09452919772325c53333df359b`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51102f02eff28acc6eb89231a81a67a0f7586b40ec7c9406c5e73657b73f92c1`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 2.2 MB (2225214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec749be77d5a19cc47dedd00097160b1f0220d9d05ab73bd0d939594be46734f`  
		Last Modified: Fri, 11 Dec 2020 04:28:19 GMT  
		Size: 6.7 MB (6743253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6015004f4454ca6970c723ed1af34bbf7503bca68db79498b742edb6ce292c65`  
		Last Modified: Fri, 11 Dec 2020 04:28:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295c5c4333284617f343979a2ae448d1fbdb1580e6c6c41b24d15ee91c92029`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:e5008218bf420fafef6e87be629d8903d86b569f0a9e40adbd1302232fa9cb9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33481724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd0372682fb7ea9fbfeaa397b5fc426f5122b085df6c1ff7f4de4f8090e636e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 10:58:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 10:58:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:58:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 10:59:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 10:59:30 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 10:59:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:59:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 10:59:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b255ec039014b2ee98780609b6f7de5cfab1b7b38fd7004fdcf45ce1c9ecd6`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eeb81cfe4b40e78820d915e9bbf7799a22f74efcf8961799d7793d0a7b8d15`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.8 MB (1822007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4842d7c98c1db5b645a2bac4af45c5527ca36c0dabd0283998140df3b1245`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 5.9 MB (5943547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0cd6f3eb08cee56cf437100ba2abf610e71292759383a37248b31003b12347`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a46ada40dc3e992f07c972f362b7bb857e6f5649b38687ce9519f8948d0972`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:f6245dc244c77e9f4e90df27aae9438deedc5d6e955fef943fbe91e2d6ae8f30
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
$ docker pull spiped@sha256:2a1562d9a8c8bc88d3d6dd14ca19efb88a99fc683968c7e5c5bb643954121da8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36273352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c227ab9e0eaf1b392d1b5ad6a0c3ce294258575158df25fb6c6d0654ee53e911`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 16:10:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 16:10:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:10:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 16:10:12 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 16:10:13 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 16:10:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 16:10:44 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 16:10:44 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 16:10:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:10:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:10:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3417f37af9b9596fad115617f18df29172cc46a854cdc7055a23f38145a58f7`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed5044f1165e0e44070848df158eac6e4c5ec565dede6fe9b50224d8089d26c`  
		Last Modified: Wed, 18 Nov 2020 16:11:04 GMT  
		Size: 2.1 MB (2128095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db2077c0ed9103b638fe9f16fe236d093e5d52832f7df0295e05f0ede70ff45`  
		Last Modified: Wed, 18 Nov 2020 16:11:05 GMT  
		Size: 7.0 MB (7037598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4bad379660d3c468029ddb245cf2b551b49d9b11a892e0c3ab55d00816d856`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4787b232f101a29c0a4c7ca9a61effad8f7bbb98ef9f83a613b1815b923c38d`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:8382a6d947e1325a13a4418514b4e1778ca88be8206102eb0e3d3372ecc45ae9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32165056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33d4b761eea34290114eb674784d79a9ba452ccfc459a243cb5c63ef7589073`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 03:18:34 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 03:18:36 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 03:18:37 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 03:18:38 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 03:19:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 03:19:44 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 03:19:46 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 03:19:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:19:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db33d41ae1e9c76b9469640f87f593bb4644e3085f6a94fc2ed1985923392019`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e63c2f068f85d42076f8db5942ea78c569062bb6a52233f11c6baa2837c949`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 1.8 MB (1839441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bd0e0488057327d00c2c57a4d54689cbfc3bf3191ed03cb5f3461b70ee4a14`  
		Last Modified: Fri, 11 Dec 2020 03:20:13 GMT  
		Size: 5.5 MB (5479951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e867722c47de78ee7eddc4dabbed59b1c64da9e19394ea95d06872535d363`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe8c65d2ad6f0615a68f49a04f3388fedbe1fda01bbfd203fc4487a775ce6b`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c92653d99274d40ed92e53b51cd458c1c727bd16db66392e4ece2f0b00be2bba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29761232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2661d3a07d889d24fd48344b6e5491127cb4f992b7c6792f931e16aed75e01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:11:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 07:12:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:12:02 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 07:12:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 07:12:49 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 07:12:50 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 07:12:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 07:12:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 07:12:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cf66057f794f2070347e36745e45359107e121bbf72ef76a056d4d4fc427c8`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d27f2deb7663af698a4e93d06d910420b62eff5f2514cf63280715267d5e70`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2c064480e805187730287fd350b20cc30e1d074b9bf0a28d1d2a9a99934bc`  
		Last Modified: Wed, 18 Nov 2020 07:13:11 GMT  
		Size: 5.3 MB (5285408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c3e496f6405bc525c1b47e008b53a0702b5b3bad600d201daaefffd563a900`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070369842a89c55f148641e29030bb3456430e5b407bca9462c0845656ffa901`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:704c22b8b676b28651bdfbc6c270305a1d9c51dd839140ea45ac633c07afa4fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdf237415bc56dd43224e7632a35235757d01c6868a15b0053e72466291cd22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 16:23:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 16:24:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:24:08 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 16:24:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 16:24:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 16:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 16:25:23 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 16:25:34 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 16:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:25:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:25:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b998896ae01086d1d742538d6adf34407de566efe82ebee5c53075ea9cdf1cf`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09275dfac82d12984d43305a0c4751236ff1270dfa9d4233c677b164cbd7b997`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 2.0 MB (2007845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0a55a486b4a21452caace28f1c3f2202530083726583e2a4cd34ea385c9df`  
		Last Modified: Wed, 18 Nov 2020 16:26:11 GMT  
		Size: 5.9 MB (5905523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcab3d8fdb677571f99ea2d30d6662ffc0707ad0bc61ce5daf5793fd5ad700a`  
		Last Modified: Wed, 18 Nov 2020 16:26:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc91fb24b5ded88e1a0ae7d5da9a99894c51155f175d6485b1f2882bab175b3`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:eddfe3c52b1f4b047ef49c6894ac40c53dae8caa677970de4764755a754e2d13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41533953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9f2903e64f88c4e2273df5e291e5b21389aab4d0a9650d5208dc6b9554981a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:58:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 02:58:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:58:29 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 02:59:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 02:59:14 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 02:59:14 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 02:59:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 02:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 02:59:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264b3982a6da8264a3a2509542dd8f472e2d82b36d7390aae536e3610041397`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a88c082c81069b5976f79f328a9b78f7cb1c5f3401419d2f93e4bd215f38c6`  
		Last Modified: Wed, 18 Nov 2020 02:59:41 GMT  
		Size: 2.1 MB (2132327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574d0a70d657cc4f156f932200e3fb841eacd020f9786fda644f94670ea16967`  
		Last Modified: Wed, 18 Nov 2020 02:59:46 GMT  
		Size: 11.6 MB (11633270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08225d6c4b1f5a1e4901290593a71354dd7c6c676ad0319b46ca6f412e3b7ddc`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02262d310542335fc2631f9f33cc647034e6d1631581742ac01cc8aead9aac83`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:243dc5166fb19dded5aa7f688c64f8b13bf15e99a113733d155ab74f1f168a20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33907845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b92b94ba5487463c171553956b8c9a332f44c401cb8db357c44f7c19a570229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:59:15 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:59:27 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 23:00:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 23:00:36 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 23:00:36 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 23:00:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 23:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 23:00:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9c786dc23ade88d3972745848ed18089b024099778eb9bf9d5c735c7c4614`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2f2cc0e46aaf9c5d0d01e3ff5c89071efebe06cb0ea5051f316c674af976b`  
		Last Modified: Tue, 17 Nov 2020 23:01:03 GMT  
		Size: 1.7 MB (1712030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e296927f1a689719138bc125a62b2d185095d494c1a18e511c2892e5f7e6ebc`  
		Last Modified: Tue, 17 Nov 2020 23:01:09 GMT  
		Size: 6.4 MB (6416166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2df2217335c02b14a90f6c1795f3149d71d77ba2611651c6a679b4bcca6d78`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d899f01843caa25aba126202c9fb34048dffe56d82e9d6296c2ec3177157c39`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:801fff27925c8e87ed9c5de2b32b74b636299c69fdbae15c814213d2086e2ca9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39495394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e191926eaea1d0c33716adeb209444a2e64bfae48ecff245fd0ce5f35af1afc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:22:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 04:23:00 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 04:23:04 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:23:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:23:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:25:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 04:25:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:26:04 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:26:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:26:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:26:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8f5dac353b2538492cef6c8c584ca52b4b8a09452919772325c53333df359b`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51102f02eff28acc6eb89231a81a67a0f7586b40ec7c9406c5e73657b73f92c1`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 2.2 MB (2225214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec749be77d5a19cc47dedd00097160b1f0220d9d05ab73bd0d939594be46734f`  
		Last Modified: Fri, 11 Dec 2020 04:28:19 GMT  
		Size: 6.7 MB (6743253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6015004f4454ca6970c723ed1af34bbf7503bca68db79498b742edb6ce292c65`  
		Last Modified: Fri, 11 Dec 2020 04:28:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295c5c4333284617f343979a2ae448d1fbdb1580e6c6c41b24d15ee91c92029`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:e5008218bf420fafef6e87be629d8903d86b569f0a9e40adbd1302232fa9cb9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33481724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd0372682fb7ea9fbfeaa397b5fc426f5122b085df6c1ff7f4de4f8090e636e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 10:58:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 10:58:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:58:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 10:59:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 10:59:30 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 10:59:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:59:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 10:59:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b255ec039014b2ee98780609b6f7de5cfab1b7b38fd7004fdcf45ce1c9ecd6`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eeb81cfe4b40e78820d915e9bbf7799a22f74efcf8961799d7793d0a7b8d15`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.8 MB (1822007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4842d7c98c1db5b645a2bac4af45c5527ca36c0dabd0283998140df3b1245`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 5.9 MB (5943547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0cd6f3eb08cee56cf437100ba2abf610e71292759383a37248b31003b12347`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a46ada40dc3e992f07c972f362b7bb857e6f5649b38687ce9519f8948d0972`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:a66b70ec9fed63f99d5ebb9a084fd6b4f2e48d3306b6d5963d5bab3a3554d099
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
$ docker pull spiped@sha256:e72efc9006cc88e74da18f8909e9a6d6cb80c024bc171e1de9a3bfa8082c7e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cd33bc57ff09ba0929eb9a1846e003f8ab8d35ac7f715f376161a9209fb7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:23:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 08:23:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 08:24:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 08:24:10 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 08:24:10 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 08:24:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2cfe9f1210973e807f22612ef44f79fdf4e9f1871ceb24da9c470ff4c6934a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebdc509a836b5478bba964b2f5c1712aa349a3761854c4f1193f580d18193`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2055abf7179bbbbaca992858134f6d59becb2b5cb2f516330f97082d7f4d272`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 211.4 KB (211432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a723ed90b1f6fc5a4bc245ba955d04306500cc3613e897f36a9246cb119a856`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8823b92e870bcac9a4efd674a3b7605e55d9877e47bb6d81c8d47f8e80d12a4a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a2c07b0fd8b8125bc764aec18cc6f9bc8bb426248f34561bd3ecc499d09346df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:677efa26ec938c048fee627507fc0da1cc62578addd97b08b687dd5b2ad77915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:43:03 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 05:43:05 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 05:43:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 05:43:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 05:43:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 05:43:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 05:43:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:43:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:43:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d656e33abe3d3601b321a868fc727b9be9c99b7488b724d484186750afcda4`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1772247a79d18f5b7de3c61484f065ffad9fd2ac52c4bf1391e9391d27a4312`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 6.8 KB (6764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ba7bffb31272cb6237ecfa4bf695187d6b5efb425f524479464784e4b970`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 198.4 KB (198368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5beb20421fe898cdae2849e5ce6bbf79e1393ffd677dc4d82b8271eebfd5cbe`  
		Last Modified: Fri, 11 Dec 2020 05:43:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a68e820deaacde91763058f7c4d28c1853ff02d626aa4516ad41ab4a155873`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1913a59773cf295dd8d96f26cc0ba23e5325c4b318f2e48b1668736a9a5ae532
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648a07e74593903bb0b5a422c8c3f677102d278b79b31a76cba4b51e1be16af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:59:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:59:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:59:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 03:00:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 03:00:11 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 03:00:12 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 03:00:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 03:00:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:00:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d19d74400f766b7b4a9239a805587a1523517a166d14ed12a1bc5435fcca7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a534ce800d06acec8b2e639d97798306f250838441b482b3dba8a16bc6ff45f`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194e2e34702b51562d461ab44982ea3720b4edf6bcf81e135005398c1f9bdc7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 191.6 KB (191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d152e941e8212f73f472183f3c9742b6a5c8670c44519dd69234bc46428dcc04`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41531b30548b2b91cc5b6563486356d5a291b1e56c550ce60fa95fcd766c25`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:22e076d0704999df6954352a61322c7aff9e84102fb209dca8c67047f0f9ec55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12732fc9350260a757debfd45b04e105fa193198c820121c8fb104c75e4090e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:13:00 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:13:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:13:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:13:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:13:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:13:37 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:13:38 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:13:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ac12de1615c4fcf136e9caab1c56384e869fa371fb1aa91fa6a50584aede8`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49ab63c0d72d683d01704eb4d538cac06f6cccc649a32c793531090a507d758`  
		Last Modified: Thu, 22 Oct 2020 09:14:05 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7c72e8f699aad2c97e9e3116224f712f7a66a5bacec74cb4db459e9275f8d2`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 203.8 KB (203833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc60fd10df854316c0653b5c11cd733c7191a08efa7aa164d9d9e6cb76de12`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47396fd59d212f4a22fd40665e6647db1065fd9aebe2fe3394e3c973688ad64`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:69a8f9d0101fda57680f27c30ca9864f021d69a013d0d876c7f010296105365d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aeca41fe853b4af9d83ed356e1a338abb14a58e5645c3cb4a0756640886dc5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:58:32 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 05:58:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 05:58:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 05:58:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 05:58:53 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 05:58:53 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 05:58:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:58:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 05:58:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cf7cc4c20069210dbf0b03ab1fecd91e3d95b49c97e98cae7c670b28f0033`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf8eec65d1d720af4b0e901af92897e91841e174ac0414999f9174673879238`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca18ab8a4b82f11e9d159625a64a3b9923866ef0471b97f803fb09071405476`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 221.2 KB (221209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cce939bb90551e9a0f849ecdfad6c57fde68602a16c1a208154aaa6a5d2c49b`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230d405b698f37c531145e3d12d6c2db6858a39fb6b5bd2a61b1e6dec0a9f38f`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8cfe707e6883e571a9e283c137fdf05c89795e813fea9d113d73243ef6e48f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0c32ce328376d6604c2cc1e3afddc420d50421031efcdfb5a64d471012cff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 04:26:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 04:26:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 04:26:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:26:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:26:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:27:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 04:27:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:27:38 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:27:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:27:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd13015bd20b24fa3de00964923d4174689fe24331cd6727149578ab140e77`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b7f2c12df52bfd764a9425a51ff9ea78c401b7ae35f4fee967e6dc290fe8a9`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a24b5a19799707647440b61dd5ce769a9faa7b9744c65a66566489782fd707`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 219.0 KB (219037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09209609f22c3956871b0ff04b1ee5a283f44fdac5054f39cdb898fbc3409c38`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeb1e3e8c1ae99b6192e09f333e05a6c38f2221cb348ac0f1aa336366022926`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f7bf86a59e1d8e7919ad60f3b4befb3cc3becb3510cd67ce32b77dad9078fc81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b6fc7550d85db051cb5ce945e2ff2f95ceb8d9e1618662ebd31a939f01e941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 10:59:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 10:59:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:59:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 10:59:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 11:00:00 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 11:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 11:00:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 11:00:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37953528e8223e90b4e88a8a082c9401b1dd5031df1927c13c1d05f57f22bfcc`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020488e0695a0946ae274aa0cd9236f69d418d2fb7e49221239ad9865fb65449`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207c4586d11b5c35ec2fb1003a5758b677ff9ff4a429824c4d92df7d7776f9c8`  
		Last Modified: Fri, 11 Dec 2020 11:00:32 GMT  
		Size: 203.0 KB (203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94329927d876dd9e10fdb405a5efc5229c1dd1ea6378287049c464675dfd09`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732197a35fbacfe3e9f631341124aee7fef90f63a252187b86cbbcdba9534ae`  
		Last Modified: Fri, 11 Dec 2020 11:00:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:a66b70ec9fed63f99d5ebb9a084fd6b4f2e48d3306b6d5963d5bab3a3554d099
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
$ docker pull spiped@sha256:e72efc9006cc88e74da18f8909e9a6d6cb80c024bc171e1de9a3bfa8082c7e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cd33bc57ff09ba0929eb9a1846e003f8ab8d35ac7f715f376161a9209fb7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:23:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 08:23:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 08:24:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 08:24:10 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 08:24:10 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 08:24:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2cfe9f1210973e807f22612ef44f79fdf4e9f1871ceb24da9c470ff4c6934a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebdc509a836b5478bba964b2f5c1712aa349a3761854c4f1193f580d18193`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2055abf7179bbbbaca992858134f6d59becb2b5cb2f516330f97082d7f4d272`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 211.4 KB (211432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a723ed90b1f6fc5a4bc245ba955d04306500cc3613e897f36a9246cb119a856`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8823b92e870bcac9a4efd674a3b7605e55d9877e47bb6d81c8d47f8e80d12a4a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a2c07b0fd8b8125bc764aec18cc6f9bc8bb426248f34561bd3ecc499d09346df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:677efa26ec938c048fee627507fc0da1cc62578addd97b08b687dd5b2ad77915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:43:03 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 05:43:05 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 05:43:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 05:43:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 05:43:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 05:43:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 05:43:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:43:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:43:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d656e33abe3d3601b321a868fc727b9be9c99b7488b724d484186750afcda4`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1772247a79d18f5b7de3c61484f065ffad9fd2ac52c4bf1391e9391d27a4312`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 6.8 KB (6764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ba7bffb31272cb6237ecfa4bf695187d6b5efb425f524479464784e4b970`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 198.4 KB (198368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5beb20421fe898cdae2849e5ce6bbf79e1393ffd677dc4d82b8271eebfd5cbe`  
		Last Modified: Fri, 11 Dec 2020 05:43:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a68e820deaacde91763058f7c4d28c1853ff02d626aa4516ad41ab4a155873`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1913a59773cf295dd8d96f26cc0ba23e5325c4b318f2e48b1668736a9a5ae532
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648a07e74593903bb0b5a422c8c3f677102d278b79b31a76cba4b51e1be16af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:59:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:59:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:59:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 03:00:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 03:00:11 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 03:00:12 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 03:00:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 03:00:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:00:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d19d74400f766b7b4a9239a805587a1523517a166d14ed12a1bc5435fcca7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a534ce800d06acec8b2e639d97798306f250838441b482b3dba8a16bc6ff45f`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194e2e34702b51562d461ab44982ea3720b4edf6bcf81e135005398c1f9bdc7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 191.6 KB (191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d152e941e8212f73f472183f3c9742b6a5c8670c44519dd69234bc46428dcc04`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41531b30548b2b91cc5b6563486356d5a291b1e56c550ce60fa95fcd766c25`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:22e076d0704999df6954352a61322c7aff9e84102fb209dca8c67047f0f9ec55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12732fc9350260a757debfd45b04e105fa193198c820121c8fb104c75e4090e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:13:00 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:13:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:13:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:13:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:13:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:13:37 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:13:38 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:13:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ac12de1615c4fcf136e9caab1c56384e869fa371fb1aa91fa6a50584aede8`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49ab63c0d72d683d01704eb4d538cac06f6cccc649a32c793531090a507d758`  
		Last Modified: Thu, 22 Oct 2020 09:14:05 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7c72e8f699aad2c97e9e3116224f712f7a66a5bacec74cb4db459e9275f8d2`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 203.8 KB (203833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc60fd10df854316c0653b5c11cd733c7191a08efa7aa164d9d9e6cb76de12`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47396fd59d212f4a22fd40665e6647db1065fd9aebe2fe3394e3c973688ad64`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:69a8f9d0101fda57680f27c30ca9864f021d69a013d0d876c7f010296105365d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aeca41fe853b4af9d83ed356e1a338abb14a58e5645c3cb4a0756640886dc5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:58:32 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 05:58:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 05:58:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 05:58:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 05:58:53 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 05:58:53 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 05:58:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:58:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 05:58:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cf7cc4c20069210dbf0b03ab1fecd91e3d95b49c97e98cae7c670b28f0033`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf8eec65d1d720af4b0e901af92897e91841e174ac0414999f9174673879238`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca18ab8a4b82f11e9d159625a64a3b9923866ef0471b97f803fb09071405476`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 221.2 KB (221209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cce939bb90551e9a0f849ecdfad6c57fde68602a16c1a208154aaa6a5d2c49b`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230d405b698f37c531145e3d12d6c2db6858a39fb6b5bd2a61b1e6dec0a9f38f`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8cfe707e6883e571a9e283c137fdf05c89795e813fea9d113d73243ef6e48f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0c32ce328376d6604c2cc1e3afddc420d50421031efcdfb5a64d471012cff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 04:26:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 04:26:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 04:26:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:26:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:26:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:27:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 04:27:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:27:38 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:27:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:27:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd13015bd20b24fa3de00964923d4174689fe24331cd6727149578ab140e77`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b7f2c12df52bfd764a9425a51ff9ea78c401b7ae35f4fee967e6dc290fe8a9`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a24b5a19799707647440b61dd5ce769a9faa7b9744c65a66566489782fd707`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 219.0 KB (219037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09209609f22c3956871b0ff04b1ee5a283f44fdac5054f39cdb898fbc3409c38`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeb1e3e8c1ae99b6192e09f333e05a6c38f2221cb348ac0f1aa336366022926`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f7bf86a59e1d8e7919ad60f3b4befb3cc3becb3510cd67ce32b77dad9078fc81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b6fc7550d85db051cb5ce945e2ff2f95ceb8d9e1618662ebd31a939f01e941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 10:59:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 10:59:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:59:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 10:59:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 11:00:00 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 11:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 11:00:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 11:00:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37953528e8223e90b4e88a8a082c9401b1dd5031df1927c13c1d05f57f22bfcc`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020488e0695a0946ae274aa0cd9236f69d418d2fb7e49221239ad9865fb65449`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207c4586d11b5c35ec2fb1003a5758b677ff9ff4a429824c4d92df7d7776f9c8`  
		Last Modified: Fri, 11 Dec 2020 11:00:32 GMT  
		Size: 203.0 KB (203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94329927d876dd9e10fdb405a5efc5229c1dd1ea6378287049c464675dfd09`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732197a35fbacfe3e9f631341124aee7fef90f63a252187b86cbbcdba9534ae`  
		Last Modified: Fri, 11 Dec 2020 11:00:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:a66b70ec9fed63f99d5ebb9a084fd6b4f2e48d3306b6d5963d5bab3a3554d099
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
$ docker pull spiped@sha256:e72efc9006cc88e74da18f8909e9a6d6cb80c024bc171e1de9a3bfa8082c7e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cd33bc57ff09ba0929eb9a1846e003f8ab8d35ac7f715f376161a9209fb7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:23:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 08:23:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 08:24:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 08:24:10 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 08:24:10 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 08:24:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2cfe9f1210973e807f22612ef44f79fdf4e9f1871ceb24da9c470ff4c6934a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebdc509a836b5478bba964b2f5c1712aa349a3761854c4f1193f580d18193`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2055abf7179bbbbaca992858134f6d59becb2b5cb2f516330f97082d7f4d272`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 211.4 KB (211432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a723ed90b1f6fc5a4bc245ba955d04306500cc3613e897f36a9246cb119a856`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8823b92e870bcac9a4efd674a3b7605e55d9877e47bb6d81c8d47f8e80d12a4a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a2c07b0fd8b8125bc764aec18cc6f9bc8bb426248f34561bd3ecc499d09346df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:677efa26ec938c048fee627507fc0da1cc62578addd97b08b687dd5b2ad77915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:43:03 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 05:43:05 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 05:43:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 05:43:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 05:43:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 05:43:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 05:43:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:43:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:43:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d656e33abe3d3601b321a868fc727b9be9c99b7488b724d484186750afcda4`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1772247a79d18f5b7de3c61484f065ffad9fd2ac52c4bf1391e9391d27a4312`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 6.8 KB (6764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ba7bffb31272cb6237ecfa4bf695187d6b5efb425f524479464784e4b970`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 198.4 KB (198368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5beb20421fe898cdae2849e5ce6bbf79e1393ffd677dc4d82b8271eebfd5cbe`  
		Last Modified: Fri, 11 Dec 2020 05:43:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a68e820deaacde91763058f7c4d28c1853ff02d626aa4516ad41ab4a155873`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1913a59773cf295dd8d96f26cc0ba23e5325c4b318f2e48b1668736a9a5ae532
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648a07e74593903bb0b5a422c8c3f677102d278b79b31a76cba4b51e1be16af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:59:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:59:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:59:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 03:00:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 03:00:11 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 03:00:12 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 03:00:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 03:00:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:00:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d19d74400f766b7b4a9239a805587a1523517a166d14ed12a1bc5435fcca7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a534ce800d06acec8b2e639d97798306f250838441b482b3dba8a16bc6ff45f`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194e2e34702b51562d461ab44982ea3720b4edf6bcf81e135005398c1f9bdc7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 191.6 KB (191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d152e941e8212f73f472183f3c9742b6a5c8670c44519dd69234bc46428dcc04`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41531b30548b2b91cc5b6563486356d5a291b1e56c550ce60fa95fcd766c25`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:22e076d0704999df6954352a61322c7aff9e84102fb209dca8c67047f0f9ec55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12732fc9350260a757debfd45b04e105fa193198c820121c8fb104c75e4090e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:13:00 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:13:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:13:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:13:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:13:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:13:37 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:13:38 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:13:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ac12de1615c4fcf136e9caab1c56384e869fa371fb1aa91fa6a50584aede8`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49ab63c0d72d683d01704eb4d538cac06f6cccc649a32c793531090a507d758`  
		Last Modified: Thu, 22 Oct 2020 09:14:05 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7c72e8f699aad2c97e9e3116224f712f7a66a5bacec74cb4db459e9275f8d2`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 203.8 KB (203833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc60fd10df854316c0653b5c11cd733c7191a08efa7aa164d9d9e6cb76de12`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47396fd59d212f4a22fd40665e6647db1065fd9aebe2fe3394e3c973688ad64`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:69a8f9d0101fda57680f27c30ca9864f021d69a013d0d876c7f010296105365d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aeca41fe853b4af9d83ed356e1a338abb14a58e5645c3cb4a0756640886dc5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:58:32 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 05:58:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 05:58:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 05:58:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 05:58:53 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 05:58:53 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 05:58:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:58:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 05:58:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cf7cc4c20069210dbf0b03ab1fecd91e3d95b49c97e98cae7c670b28f0033`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf8eec65d1d720af4b0e901af92897e91841e174ac0414999f9174673879238`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca18ab8a4b82f11e9d159625a64a3b9923866ef0471b97f803fb09071405476`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 221.2 KB (221209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cce939bb90551e9a0f849ecdfad6c57fde68602a16c1a208154aaa6a5d2c49b`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230d405b698f37c531145e3d12d6c2db6858a39fb6b5bd2a61b1e6dec0a9f38f`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8cfe707e6883e571a9e283c137fdf05c89795e813fea9d113d73243ef6e48f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0c32ce328376d6604c2cc1e3afddc420d50421031efcdfb5a64d471012cff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 04:26:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 04:26:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 04:26:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:26:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:26:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:27:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 04:27:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:27:38 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:27:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:27:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd13015bd20b24fa3de00964923d4174689fe24331cd6727149578ab140e77`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b7f2c12df52bfd764a9425a51ff9ea78c401b7ae35f4fee967e6dc290fe8a9`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a24b5a19799707647440b61dd5ce769a9faa7b9744c65a66566489782fd707`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 219.0 KB (219037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09209609f22c3956871b0ff04b1ee5a283f44fdac5054f39cdb898fbc3409c38`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeb1e3e8c1ae99b6192e09f333e05a6c38f2221cb348ac0f1aa336366022926`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f7bf86a59e1d8e7919ad60f3b4befb3cc3becb3510cd67ce32b77dad9078fc81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b6fc7550d85db051cb5ce945e2ff2f95ceb8d9e1618662ebd31a939f01e941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 10:59:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 10:59:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:59:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 10:59:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 11:00:00 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 11:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 11:00:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 11:00:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37953528e8223e90b4e88a8a082c9401b1dd5031df1927c13c1d05f57f22bfcc`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020488e0695a0946ae274aa0cd9236f69d418d2fb7e49221239ad9865fb65449`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207c4586d11b5c35ec2fb1003a5758b677ff9ff4a429824c4d92df7d7776f9c8`  
		Last Modified: Fri, 11 Dec 2020 11:00:32 GMT  
		Size: 203.0 KB (203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94329927d876dd9e10fdb405a5efc5229c1dd1ea6378287049c464675dfd09`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732197a35fbacfe3e9f631341124aee7fef90f63a252187b86cbbcdba9534ae`  
		Last Modified: Fri, 11 Dec 2020 11:00:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:a66b70ec9fed63f99d5ebb9a084fd6b4f2e48d3306b6d5963d5bab3a3554d099
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
$ docker pull spiped@sha256:e72efc9006cc88e74da18f8909e9a6d6cb80c024bc171e1de9a3bfa8082c7e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cd33bc57ff09ba0929eb9a1846e003f8ab8d35ac7f715f376161a9209fb7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:23:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 08:23:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 08:24:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 08:24:10 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 08:24:10 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 08:24:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2cfe9f1210973e807f22612ef44f79fdf4e9f1871ceb24da9c470ff4c6934a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebdc509a836b5478bba964b2f5c1712aa349a3761854c4f1193f580d18193`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2055abf7179bbbbaca992858134f6d59becb2b5cb2f516330f97082d7f4d272`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 211.4 KB (211432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a723ed90b1f6fc5a4bc245ba955d04306500cc3613e897f36a9246cb119a856`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8823b92e870bcac9a4efd674a3b7605e55d9877e47bb6d81c8d47f8e80d12a4a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a2c07b0fd8b8125bc764aec18cc6f9bc8bb426248f34561bd3ecc499d09346df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:677efa26ec938c048fee627507fc0da1cc62578addd97b08b687dd5b2ad77915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:43:03 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 05:43:05 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 05:43:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 05:43:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 05:43:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 05:43:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 05:43:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:43:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:43:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d656e33abe3d3601b321a868fc727b9be9c99b7488b724d484186750afcda4`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1772247a79d18f5b7de3c61484f065ffad9fd2ac52c4bf1391e9391d27a4312`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 6.8 KB (6764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ba7bffb31272cb6237ecfa4bf695187d6b5efb425f524479464784e4b970`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 198.4 KB (198368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5beb20421fe898cdae2849e5ce6bbf79e1393ffd677dc4d82b8271eebfd5cbe`  
		Last Modified: Fri, 11 Dec 2020 05:43:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a68e820deaacde91763058f7c4d28c1853ff02d626aa4516ad41ab4a155873`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1913a59773cf295dd8d96f26cc0ba23e5325c4b318f2e48b1668736a9a5ae532
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648a07e74593903bb0b5a422c8c3f677102d278b79b31a76cba4b51e1be16af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:59:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:59:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:59:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 03:00:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 03:00:11 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 03:00:12 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 03:00:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 03:00:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:00:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d19d74400f766b7b4a9239a805587a1523517a166d14ed12a1bc5435fcca7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a534ce800d06acec8b2e639d97798306f250838441b482b3dba8a16bc6ff45f`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194e2e34702b51562d461ab44982ea3720b4edf6bcf81e135005398c1f9bdc7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 191.6 KB (191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d152e941e8212f73f472183f3c9742b6a5c8670c44519dd69234bc46428dcc04`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41531b30548b2b91cc5b6563486356d5a291b1e56c550ce60fa95fcd766c25`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:22e076d0704999df6954352a61322c7aff9e84102fb209dca8c67047f0f9ec55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12732fc9350260a757debfd45b04e105fa193198c820121c8fb104c75e4090e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:13:00 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:13:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:13:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:13:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:13:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:13:37 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:13:38 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:13:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ac12de1615c4fcf136e9caab1c56384e869fa371fb1aa91fa6a50584aede8`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49ab63c0d72d683d01704eb4d538cac06f6cccc649a32c793531090a507d758`  
		Last Modified: Thu, 22 Oct 2020 09:14:05 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7c72e8f699aad2c97e9e3116224f712f7a66a5bacec74cb4db459e9275f8d2`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 203.8 KB (203833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc60fd10df854316c0653b5c11cd733c7191a08efa7aa164d9d9e6cb76de12`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47396fd59d212f4a22fd40665e6647db1065fd9aebe2fe3394e3c973688ad64`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:69a8f9d0101fda57680f27c30ca9864f021d69a013d0d876c7f010296105365d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aeca41fe853b4af9d83ed356e1a338abb14a58e5645c3cb4a0756640886dc5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:58:32 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 05:58:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 05:58:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 05:58:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 05:58:53 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 05:58:53 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 05:58:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:58:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 05:58:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cf7cc4c20069210dbf0b03ab1fecd91e3d95b49c97e98cae7c670b28f0033`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf8eec65d1d720af4b0e901af92897e91841e174ac0414999f9174673879238`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca18ab8a4b82f11e9d159625a64a3b9923866ef0471b97f803fb09071405476`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 221.2 KB (221209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cce939bb90551e9a0f849ecdfad6c57fde68602a16c1a208154aaa6a5d2c49b`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230d405b698f37c531145e3d12d6c2db6858a39fb6b5bd2a61b1e6dec0a9f38f`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8cfe707e6883e571a9e283c137fdf05c89795e813fea9d113d73243ef6e48f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0c32ce328376d6604c2cc1e3afddc420d50421031efcdfb5a64d471012cff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 04:26:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 04:26:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 04:26:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:26:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:26:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:27:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 04:27:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:27:38 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:27:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:27:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd13015bd20b24fa3de00964923d4174689fe24331cd6727149578ab140e77`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b7f2c12df52bfd764a9425a51ff9ea78c401b7ae35f4fee967e6dc290fe8a9`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a24b5a19799707647440b61dd5ce769a9faa7b9744c65a66566489782fd707`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 219.0 KB (219037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09209609f22c3956871b0ff04b1ee5a283f44fdac5054f39cdb898fbc3409c38`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeb1e3e8c1ae99b6192e09f333e05a6c38f2221cb348ac0f1aa336366022926`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f7bf86a59e1d8e7919ad60f3b4befb3cc3becb3510cd67ce32b77dad9078fc81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b6fc7550d85db051cb5ce945e2ff2f95ceb8d9e1618662ebd31a939f01e941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 10:59:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 10:59:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:59:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 10:59:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 11:00:00 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 11:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 11:00:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 11:00:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37953528e8223e90b4e88a8a082c9401b1dd5031df1927c13c1d05f57f22bfcc`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020488e0695a0946ae274aa0cd9236f69d418d2fb7e49221239ad9865fb65449`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207c4586d11b5c35ec2fb1003a5758b677ff9ff4a429824c4d92df7d7776f9c8`  
		Last Modified: Fri, 11 Dec 2020 11:00:32 GMT  
		Size: 203.0 KB (203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94329927d876dd9e10fdb405a5efc5229c1dd1ea6378287049c464675dfd09`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732197a35fbacfe3e9f631341124aee7fef90f63a252187b86cbbcdba9534ae`  
		Last Modified: Fri, 11 Dec 2020 11:00:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:f6245dc244c77e9f4e90df27aae9438deedc5d6e955fef943fbe91e2d6ae8f30
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
$ docker pull spiped@sha256:2a1562d9a8c8bc88d3d6dd14ca19efb88a99fc683968c7e5c5bb643954121da8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36273352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c227ab9e0eaf1b392d1b5ad6a0c3ce294258575158df25fb6c6d0654ee53e911`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 16:10:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 16:10:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:10:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 16:10:12 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 16:10:13 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 16:10:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 16:10:44 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 16:10:44 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 16:10:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:10:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:10:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3417f37af9b9596fad115617f18df29172cc46a854cdc7055a23f38145a58f7`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed5044f1165e0e44070848df158eac6e4c5ec565dede6fe9b50224d8089d26c`  
		Last Modified: Wed, 18 Nov 2020 16:11:04 GMT  
		Size: 2.1 MB (2128095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db2077c0ed9103b638fe9f16fe236d093e5d52832f7df0295e05f0ede70ff45`  
		Last Modified: Wed, 18 Nov 2020 16:11:05 GMT  
		Size: 7.0 MB (7037598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4bad379660d3c468029ddb245cf2b551b49d9b11a892e0c3ab55d00816d856`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4787b232f101a29c0a4c7ca9a61effad8f7bbb98ef9f83a613b1815b923c38d`  
		Last Modified: Wed, 18 Nov 2020 16:11:03 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:8382a6d947e1325a13a4418514b4e1778ca88be8206102eb0e3d3372ecc45ae9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32165056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33d4b761eea34290114eb674784d79a9ba452ccfc459a243cb5c63ef7589073`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 03:18:34 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 03:18:36 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 03:18:37 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 03:18:38 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 03:19:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 03:19:44 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 03:19:46 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 03:19:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:19:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db33d41ae1e9c76b9469640f87f593bb4644e3085f6a94fc2ed1985923392019`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e63c2f068f85d42076f8db5942ea78c569062bb6a52233f11c6baa2837c949`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 1.8 MB (1839441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bd0e0488057327d00c2c57a4d54689cbfc3bf3191ed03cb5f3461b70ee4a14`  
		Last Modified: Fri, 11 Dec 2020 03:20:13 GMT  
		Size: 5.5 MB (5479951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e867722c47de78ee7eddc4dabbed59b1c64da9e19394ea95d06872535d363`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe8c65d2ad6f0615a68f49a04f3388fedbe1fda01bbfd203fc4487a775ce6b`  
		Last Modified: Fri, 11 Dec 2020 03:20:11 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c92653d99274d40ed92e53b51cd458c1c727bd16db66392e4ece2f0b00be2bba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29761232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2661d3a07d889d24fd48344b6e5491127cb4f992b7c6792f931e16aed75e01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:11:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 07:12:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:12:02 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 07:12:03 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 07:12:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 07:12:49 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 07:12:50 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 07:12:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 07:12:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 07:12:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cf66057f794f2070347e36745e45359107e121bbf72ef76a056d4d4fc427c8`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d27f2deb7663af698a4e93d06d910420b62eff5f2514cf63280715267d5e70`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2c064480e805187730287fd350b20cc30e1d074b9bf0a28d1d2a9a99934bc`  
		Last Modified: Wed, 18 Nov 2020 07:13:11 GMT  
		Size: 5.3 MB (5285408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c3e496f6405bc525c1b47e008b53a0702b5b3bad600d201daaefffd563a900`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070369842a89c55f148641e29030bb3456430e5b407bca9462c0845656ffa901`  
		Last Modified: Wed, 18 Nov 2020 07:13:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:704c22b8b676b28651bdfbc6c270305a1d9c51dd839140ea45ac633c07afa4fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdf237415bc56dd43224e7632a35235757d01c6868a15b0053e72466291cd22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 16:23:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 16:24:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:24:08 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 16:24:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 16:24:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 16:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 16:25:23 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 16:25:34 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 16:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:25:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:25:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b998896ae01086d1d742538d6adf34407de566efe82ebee5c53075ea9cdf1cf`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09275dfac82d12984d43305a0c4751236ff1270dfa9d4233c677b164cbd7b997`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 2.0 MB (2007845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0a55a486b4a21452caace28f1c3f2202530083726583e2a4cd34ea385c9df`  
		Last Modified: Wed, 18 Nov 2020 16:26:11 GMT  
		Size: 5.9 MB (5905523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcab3d8fdb677571f99ea2d30d6662ffc0707ad0bc61ce5daf5793fd5ad700a`  
		Last Modified: Wed, 18 Nov 2020 16:26:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc91fb24b5ded88e1a0ae7d5da9a99894c51155f175d6485b1f2882bab175b3`  
		Last Modified: Wed, 18 Nov 2020 16:26:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:eddfe3c52b1f4b047ef49c6894ac40c53dae8caa677970de4764755a754e2d13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41533953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9f2903e64f88c4e2273df5e291e5b21389aab4d0a9650d5208dc6b9554981a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:58:21 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 18 Nov 2020 02:58:29 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:58:29 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 18 Nov 2020 02:58:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 18 Nov 2020 02:59:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 18 Nov 2020 02:59:14 GMT
VOLUME [/spiped]
# Wed, 18 Nov 2020 02:59:14 GMT
WORKDIR /spiped
# Wed, 18 Nov 2020 02:59:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 18 Nov 2020 02:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 02:59:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f264b3982a6da8264a3a2509542dd8f472e2d82b36d7390aae536e3610041397`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a88c082c81069b5976f79f328a9b78f7cb1c5f3401419d2f93e4bd215f38c6`  
		Last Modified: Wed, 18 Nov 2020 02:59:41 GMT  
		Size: 2.1 MB (2132327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574d0a70d657cc4f156f932200e3fb841eacd020f9786fda644f94670ea16967`  
		Last Modified: Wed, 18 Nov 2020 02:59:46 GMT  
		Size: 11.6 MB (11633270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08225d6c4b1f5a1e4901290593a71354dd7c6c676ad0319b46ca6f412e3b7ddc`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02262d310542335fc2631f9f33cc647034e6d1631581742ac01cc8aead9aac83`  
		Last Modified: Wed, 18 Nov 2020 02:59:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:243dc5166fb19dded5aa7f688c64f8b13bf15e99a113733d155ab74f1f168a20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33907845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b92b94ba5487463c171553956b8c9a332f44c401cb8db357c44f7c19a570229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:59:15 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 17 Nov 2020 22:59:27 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 17 Nov 2020 22:59:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 17 Nov 2020 23:00:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 17 Nov 2020 23:00:36 GMT
VOLUME [/spiped]
# Tue, 17 Nov 2020 23:00:36 GMT
WORKDIR /spiped
# Tue, 17 Nov 2020 23:00:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 17 Nov 2020 23:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 23:00:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9c786dc23ade88d3972745848ed18089b024099778eb9bf9d5c735c7c4614`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2f2cc0e46aaf9c5d0d01e3ff5c89071efebe06cb0ea5051f316c674af976b`  
		Last Modified: Tue, 17 Nov 2020 23:01:03 GMT  
		Size: 1.7 MB (1712030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e296927f1a689719138bc125a62b2d185095d494c1a18e511c2892e5f7e6ebc`  
		Last Modified: Tue, 17 Nov 2020 23:01:09 GMT  
		Size: 6.4 MB (6416166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2df2217335c02b14a90f6c1795f3149d71d77ba2611651c6a679b4bcca6d78`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d899f01843caa25aba126202c9fb34048dffe56d82e9d6296c2ec3177157c39`  
		Last Modified: Tue, 17 Nov 2020 23:01:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:801fff27925c8e87ed9c5de2b32b74b636299c69fdbae15c814213d2086e2ca9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39495394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e191926eaea1d0c33716adeb209444a2e64bfae48ecff245fd0ce5f35af1afc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:22:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 04:23:00 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 04:23:04 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:23:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:23:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:25:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 04:25:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:26:04 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:26:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:26:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:26:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8f5dac353b2538492cef6c8c584ca52b4b8a09452919772325c53333df359b`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51102f02eff28acc6eb89231a81a67a0f7586b40ec7c9406c5e73657b73f92c1`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 2.2 MB (2225214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec749be77d5a19cc47dedd00097160b1f0220d9d05ab73bd0d939594be46734f`  
		Last Modified: Fri, 11 Dec 2020 04:28:19 GMT  
		Size: 6.7 MB (6743253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6015004f4454ca6970c723ed1af34bbf7503bca68db79498b742edb6ce292c65`  
		Last Modified: Fri, 11 Dec 2020 04:28:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3295c5c4333284617f343979a2ae448d1fbdb1580e6c6c41b24d15ee91c92029`  
		Last Modified: Fri, 11 Dec 2020 04:28:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:e5008218bf420fafef6e87be629d8903d86b569f0a9e40adbd1302232fa9cb9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33481724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd0372682fb7ea9fbfeaa397b5fc426f5122b085df6c1ff7f4de4f8090e636e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 10:58:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 11 Dec 2020 10:58:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:58:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:58:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 11 Dec 2020 10:59:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 10:59:30 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 10:59:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:59:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 10:59:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b255ec039014b2ee98780609b6f7de5cfab1b7b38fd7004fdcf45ce1c9ecd6`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eeb81cfe4b40e78820d915e9bbf7799a22f74efcf8961799d7793d0a7b8d15`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 1.8 MB (1822007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4842d7c98c1db5b645a2bac4af45c5527ca36c0dabd0283998140df3b1245`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 5.9 MB (5943547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0cd6f3eb08cee56cf437100ba2abf610e71292759383a37248b31003b12347`  
		Last Modified: Fri, 11 Dec 2020 11:00:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a46ada40dc3e992f07c972f362b7bb857e6f5649b38687ce9519f8948d0972`  
		Last Modified: Fri, 11 Dec 2020 11:00:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
