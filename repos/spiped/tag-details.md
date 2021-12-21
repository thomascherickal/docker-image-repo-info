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
$ docker pull spiped@sha256:72d5844d36f4a0ae5b0828c8e434c770fe7ca47b2e901fbeaf9670adcefc44ce
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
$ docker pull spiped@sha256:2bd2286a40c61a56f280444f68f9c3d0ae7a310858860aba77b0403b8890c9f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37321326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4914da9141203212b68712b5f3a3711294f5e0e02a612eec74bd1b2e1241b9b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 12:54:46 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 12:54:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:54:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 12:55:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 12:55:16 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 12:55:16 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 12:55:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 12:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 12:55:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5942a3089c9d199ffd7567fc18e1491777fdade26ec8bdf4d160bf3c8d83f324`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643f2d189091c21b4eee0a6fe6553c7c7ad5a1fba49319eac9c272a96ac7fbdd`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f16287ae7ba5070d7edb0070fe71b973932136de80e4a4dd1013707e336b0c7`  
		Last Modified: Tue, 21 Dec 2021 12:55:41 GMT  
		Size: 6.0 MB (5960446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e68e4478591fe99bf722077de675519de67d719f9677d67f1ddc4d8f2cec294`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587fde5003f001f256acac00acf4ea7b0205ea8770d68ee6a9a2d3c87c369d95`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:613ef7662f31f09717e32907426042a146b7a0dc66e68870888cb83f73518f22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33939189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f0656da52ff3c99f44f7de064c2a87f0da72fa7fbe3ed879cb8732d6b9c4313`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:37 GMT
ADD file:7debbdb237139cb08189976f79cfa64cfd71f5cc98dfb2f560b558acb5f7cec9 in / 
# Thu, 02 Dec 2021 02:50:38 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 19:44:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 19:44:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 19:44:43 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 19:45:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 19:45:46 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 19:45:46 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 19:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 19:45:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 19:45:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c5e429166894878430c39748965935f89ffa957667340c3c8bd872418dbce663`  
		Last Modified: Thu, 02 Dec 2021 03:09:28 GMT  
		Size: 28.9 MB (28910824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902a05874d1937e2586f2056f8e8c160fbcb072ecdf334c40d7d34b8c31d9943`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd0a53456b53b30461bd45c9e7454a16fe2efaf6f01fc7ba2d50b7010313872`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4abfa33026a378154de67b10639d745576834a515a1c132083ffda2a7d1c4d`  
		Last Modified: Thu, 02 Dec 2021 19:46:28 GMT  
		Size: 5.0 MB (5025111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e2166e45f5a0464a961c1a3f02059b4157a81ee9c7409a710a0aa5691cecee`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df3005de126704451e5d5a4bfc395ec490bce9a5df481a2a33cb5903873405`  
		Last Modified: Thu, 02 Dec 2021 19:46:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cd3cc375afa908acf4552d16cdb624e941a6315bbfe494df1c6b35e01d413a54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31322033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ec4a5f35bb1890066d68b0ee550709c5f39b841dd141dfcbb9582f2e1c3fc86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:00:09 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 17:00:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:00:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 17:01:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 17:01:17 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 17:01:17 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 17:01:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:01:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:01:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce69134f0203d1fe5115a1020137046d1c890b6f1a46f116d7923e7ce02d4b8`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bdbc3a8aa8079aaea6f5d5bd5b05bddcc86c669a7140435e2b3021beba5928`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5681b086406e5a0268c2b3349357d0fd9c5ddf7e6ad703841e962f1c16b81e`  
		Last Modified: Thu, 02 Dec 2021 17:02:24 GMT  
		Size: 4.7 MB (4745590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbddc9b5c4f841ea7887df8c071cc34894f11accda6eb68f03ac972530d2092`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d29046b99bda35823f2af6e8b7eda1ea3a2dda13cc35c63d5f388bf1c6ed9ab`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:076eed23d69622023465551277b292c4b20c7e53ff970f4ec2c0c88c721002a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35310451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558381a048e4dd5c28f2a72bdfb28f021302afc0b9044d17373f8513e2c57b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:37:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 13:37:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:37:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 13:37:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 13:37:57 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 13:37:58 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 13:38:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 13:38:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 13:38:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11307cfb62981d1477c624d0946d440cae59b97d5241be5622b4a1a2170b7087`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0b4f4a9f9d7183fa8a6390427dd6151121434bd32d1539e46a81b5b7195e9e`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498cf759f2f5ad49bf12c6c9162ea1c630f9fba1005c0a5cd96d9d40f3c3bc9c`  
		Last Modified: Tue, 21 Dec 2021 13:38:30 GMT  
		Size: 5.3 MB (5263680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7310cca9b3933670873fa963c55ba0370617e570124050a904a3eabfd50f0b8a`  
		Last Modified: Tue, 21 Dec 2021 13:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ebb7feec0bee35aea3ecb3f98485656fa38f1ef9c1c9faccf4d07b68e3ebbe`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:5b3875cce8fad4903a3c884cef05e5abad051bc9951e8e5410114e95e0dac53e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40258475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302f102ca38e8fbd96146e30bc1ab35ebeaf9330138e5b0b7d258e8c9cb0b61c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 21:50:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 21:50:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 21:50:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 21:51:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 21:51:10 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 21:51:11 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 21:51:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 21:51:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 21:51:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489da5566cb0c924c029e46f8dad5bcafab6d42a56da88a93f2801d29558ff51`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db213f8397acea926fb592d3befbbdb2c002c268a3d54cb1d5c2d98de07b6f00`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5a4ea8b87e71f3244324d2ead099212bccde6f64ef51cbe9d8ec4d43b36028`  
		Last Modified: Tue, 21 Dec 2021 21:52:08 GMT  
		Size: 7.9 MB (7884366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5619dad69ca0adbec11d01730713268fe39795d31498b6b4fe5494a59579236`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3945ddda45549df85f0eed7cab7fef6325fd37f1b4ef32546894d2af03acfd`  
		Last Modified: Tue, 21 Dec 2021 21:52:04 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:fbd96eab48f0706b211bc89e1e78f7630d8d467ac4c32a9a27b78651c2329258
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b3265725ae631fc1fa2baaa91faa5aac9b516c810f7ca4ece4cbf3c1dc55c65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 03:09:10 GMT
ADD file:419aff162077eb16923c3ede6455ca86756a929a5a837bc6ac6b8dc67913503a in / 
# Thu, 02 Dec 2021 03:09:10 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 12:30:36 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 03 Dec 2021 12:30:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 12:30:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 03 Dec 2021 12:31:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 03 Dec 2021 12:31:58 GMT
VOLUME [/spiped]
# Fri, 03 Dec 2021 12:31:58 GMT
WORKDIR /spiped
# Fri, 03 Dec 2021 12:31:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 03 Dec 2021 12:31:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 12:32:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df61fb15db6391af55d70bc3c0db3e9014438c81bf802619fb527221adf5e8a8`  
		Last Modified: Thu, 02 Dec 2021 03:17:58 GMT  
		Size: 29.6 MB (29630496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4804017e9aaf0b2cb114927e3f0bc9e8f6bf173f5add775eb58fdac387f7c23`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3edbf43f07b9dbfec975a7a185719337d830354ede383efbf8964fd29e88d7`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81edd02fe261e7da19a1774f5be1249c6084f65e17d566a33e234ccb73c61d60`  
		Last Modified: Fri, 03 Dec 2021 12:32:16 GMT  
		Size: 5.7 MB (5706134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d174fb700fa19b4b4f80aeba64057df901a4197213c60299a2721db837bb5a`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013cb4b0da609efc6a5d97090c932a4d4c2c7438057ee994b3df9828ae89072c`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:c4ab963378b566c625302fe8f6c2b541809cf43971b0e2bf17f9469446444777
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41276244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adaff4ae366ea0ae358b47d0091afe6566648f17243e25696f1d34b3650def8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:51:38 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 20:51:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 20:51:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 20:53:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 20:53:56 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 20:54:00 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 20:54:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 20:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 20:54:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880dff15961bfe01347887de4bb7d190126f69b5a3854acfe06c435f9a6f626e`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5e1e31bc84bb0bae8ebf518013f4bb5d706f4272c1805bbc5f219a5a7eba2c`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af77ac291d1f734c93e02eff952dcdc14b498d4e4139e1a940654a936255dd92`  
		Last Modified: Thu, 02 Dec 2021 20:54:48 GMT  
		Size: 6.0 MB (6001592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a814520e36f0aaaa383f2659b8a9ca3b25c94875ecc23578898ebebdd5fb26`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721756d3adc4340983195bc3bf63aeaad3faaad5a572a351213a923b3d9b458`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:6ca814db8831771b57c2fc6fec100a2a7172d558595020784313b259c022266e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34829005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123f2f35891cf31904936c0d30cebe83dde721ab69f4d0b103091bc34e002fe6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 11:22:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 11:22:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 11:22:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 11:23:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 11:23:21 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 11:23:22 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 11:23:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 11:23:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 11:23:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1ef12e9110fade1b5f49cd9bd409a215546e6a659caf0b7c782b63e68b435d`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc8f56cc872687f2f42c48ebccd7820d167ec5866466852bb6646f18e519803`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5ad9022f51f5dafe11dbde04206e78d75fffe06678398a3ed65c9cdf16e303`  
		Last Modified: Tue, 21 Dec 2021 11:24:01 GMT  
		Size: 5.2 MB (5184106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f5e0810a75c82e2c625f9723799e72c4c00697d471245d2df256a5490e7049`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcfe444b90c33b185e97434acae972e7f8cdcb010a7fa9709cef3db394bc323`  
		Last Modified: Tue, 21 Dec 2021 11:24:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:1447fc83864d467400e6d1b2a87532955de7649123545804894c2a8c86d6a34a
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
$ docker pull spiped@sha256:5759c6e68d7e93789c7fc574722f42f3d3bafcaab2c4a8aeeeac5bb4772012a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc3e3a8422cee08ac18b30d97939a3a6bd28e94a61d0caaaa96ff86dd8f425c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:30:36 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 07:30:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 07:30:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 07:31:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 07:31:02 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 07:31:03 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 07:31:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 07:31:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 07:31:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d272f2608cb29aaf56aaa58c4e8245793833d52257971c0a4a90c1445945548`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bebf547583661fb31be182d777849262971941c241f7b072c041f54e3c4ff`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f41a1ab4447065d651caf78075639eb1027290f0756c4d489a10c43a745af`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 213.1 KB (213113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7a22ad75e07e938780270586c7d97ddd070bf6b70ee31e6fbe14b6c79cda6`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b484100590c35b883633e127830518528f9cc47bce7f4b864394b4bd85acb54`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:e54c9ae8aa1651b3704440b6b74cbdd5ac80086e8fa25252df5ffbe44591eade
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2847905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b358d015e8acc6b6eac3e79c5fc5302785d8bce806dc4640e51e684fc73495`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:56:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 06:56:48 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 06:56:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 06:57:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 06:57:27 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 06:57:27 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 06:57:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 06:57:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:57:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbee8633a3e2da897713dd8453113fc924e1ad102e43bc673e5aa4e72a3c5ff6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421d84dfbecebc99f29f801626a8781142421b8affb55b6dac49de522afdd86`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 7.8 KB (7780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67a331696441ca0da524281edcd53ee4b8d52a24b4fdaab4f5b2e3833ab74a`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 203.0 KB (202993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ab514374a45d9fd16341748dc013e94fd9ddf0b15c2f3666bea84a2c2db7dd`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526ec51047ed2d4267785d4387f46cebef6e388cb755c73b640a73e44db871b6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8b3e418343ca28cc6af7c79a9c92f500d16214863644d56f2e6a6c6a66f457d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2644452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edd8179550b7c42a3827056d11ba4da9c0f384e1b5ac66177b911a1a9f75acc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:09:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:09:21 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:09:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:09:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:09:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:09:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2462c3e2387f9df1b6daae812a3674ccd49db10b9b7251881ea1a034a39185b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e4892bdd8b9be427ec2794ea13c95ec6cca78353d3c032d0fd2ba5acf9bae3`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 7.8 KB (7791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624ff05273c8a204e1361bc188430fe618799c3ec5471284aa49a1f9bd365020`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 196.3 KB (196302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f127d56c30dd5e8a58309b3d42c9c4f974256b6b1f1f9ff32b0ff78d8c372b3b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab7e0d291c6010513c0721d4abf0cd1f407a631c23f515859004dddf983c5f5`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ed9db1b4a0c65f0ca88573ca4e82bafaedde5032f465971dba93432ddcf67f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3064332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04afce967f7cf45ad1faa0b6e1d955f2bad9d1aff37c3659db5e809170762140`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:40:39 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 20:40:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 20:40:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 20:41:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 20:41:14 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 20:41:14 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 20:41:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 20:41:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea20678ed9ffc78867f8fc9674162184169da3d7c198cd24ec6b7439e0c88`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f04cc4ba71752a6b9075421e6b0b7f08625406fb105f85e23547c4eb23b25f3`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae957cbfbd7f9f36494cb3954e91d1ead35e68d61bbddf48904c4b6133c4c878`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 223.9 KB (223875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911b8888c5d7d41e887ed34d5f9c93d1d3241ad814e69f4d7def6b5debc96ae8`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d46a3df042754e1b8e655e102bf789f899a1f3758442759be66fe90573dbd2`  
		Last Modified: Fri, 12 Nov 2021 20:41:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:892b50ba6b7bed8e6253a2577dcb2c38d0e60b1ae71968d978a808094e610768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3048694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7522decac983b5c7f6951cee379a5207bdbe044c9371a89a784e025923deb04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:29:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 15:29:55 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 15:29:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 15:30:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 15:30:32 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 15:30:34 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 15:30:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 15:30:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63441839c077959763f01da2aec624ff02d5765af3e923419046fe79761bf71d`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907f83f2fcbfe22132bde253d7c486b65870dc9635bc53461fab20a90a87ad73`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 7.8 KB (7777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6096cf0d6847df2dfecdd48192e3922a4bbc85ed08ddfab7f33b335ffb6dc77`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 221.7 KB (221712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51da854d577591f12d32b8d52aeb0c4576b7254377303693f07d6a4854ef5f`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1d81a9ee14a2ec2938cd589d2bda48191378ac5f8717102a0203b9d37df9ff`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:118a8c071df238ccc4affa6c1ad90ecaa58fd6f20861ee190449b34b1f5734bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2824562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a068554fae2e46941a18261fe2601c6c40df867a7b227b9bf154694451ba5390`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:55:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:55:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:55:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:56:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:56:06 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:56:06 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:56:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:56:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc797db23a37010d6b83bb8a9eaa1336ed352043857e5a44d68a4b8efad9e0b5`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e810eed7330856c73daba855bc8adf50fdde87ccab6697c3416ee314886ca`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 7.8 KB (7775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a425358f95dbc88c89aac4c0c745bacaceb3d4598a051af18b0df4a28d76e`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 205.8 KB (205773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c7009eddad4f11d690d41e57f47828edf66b3f5113d35cf2a68eee8beed75`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522513383757fa4cc180054c6b6b641c302050e0dce5ddfdd2a8881e7efcfa2`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:72d5844d36f4a0ae5b0828c8e434c770fe7ca47b2e901fbeaf9670adcefc44ce
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
$ docker pull spiped@sha256:2bd2286a40c61a56f280444f68f9c3d0ae7a310858860aba77b0403b8890c9f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37321326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4914da9141203212b68712b5f3a3711294f5e0e02a612eec74bd1b2e1241b9b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 12:54:46 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 12:54:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:54:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 12:55:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 12:55:16 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 12:55:16 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 12:55:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 12:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 12:55:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5942a3089c9d199ffd7567fc18e1491777fdade26ec8bdf4d160bf3c8d83f324`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643f2d189091c21b4eee0a6fe6553c7c7ad5a1fba49319eac9c272a96ac7fbdd`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f16287ae7ba5070d7edb0070fe71b973932136de80e4a4dd1013707e336b0c7`  
		Last Modified: Tue, 21 Dec 2021 12:55:41 GMT  
		Size: 6.0 MB (5960446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e68e4478591fe99bf722077de675519de67d719f9677d67f1ddc4d8f2cec294`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587fde5003f001f256acac00acf4ea7b0205ea8770d68ee6a9a2d3c87c369d95`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:613ef7662f31f09717e32907426042a146b7a0dc66e68870888cb83f73518f22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33939189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f0656da52ff3c99f44f7de064c2a87f0da72fa7fbe3ed879cb8732d6b9c4313`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:37 GMT
ADD file:7debbdb237139cb08189976f79cfa64cfd71f5cc98dfb2f560b558acb5f7cec9 in / 
# Thu, 02 Dec 2021 02:50:38 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 19:44:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 19:44:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 19:44:43 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 19:45:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 19:45:46 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 19:45:46 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 19:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 19:45:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 19:45:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c5e429166894878430c39748965935f89ffa957667340c3c8bd872418dbce663`  
		Last Modified: Thu, 02 Dec 2021 03:09:28 GMT  
		Size: 28.9 MB (28910824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902a05874d1937e2586f2056f8e8c160fbcb072ecdf334c40d7d34b8c31d9943`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd0a53456b53b30461bd45c9e7454a16fe2efaf6f01fc7ba2d50b7010313872`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4abfa33026a378154de67b10639d745576834a515a1c132083ffda2a7d1c4d`  
		Last Modified: Thu, 02 Dec 2021 19:46:28 GMT  
		Size: 5.0 MB (5025111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e2166e45f5a0464a961c1a3f02059b4157a81ee9c7409a710a0aa5691cecee`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df3005de126704451e5d5a4bfc395ec490bce9a5df481a2a33cb5903873405`  
		Last Modified: Thu, 02 Dec 2021 19:46:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cd3cc375afa908acf4552d16cdb624e941a6315bbfe494df1c6b35e01d413a54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31322033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ec4a5f35bb1890066d68b0ee550709c5f39b841dd141dfcbb9582f2e1c3fc86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:00:09 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 17:00:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:00:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 17:01:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 17:01:17 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 17:01:17 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 17:01:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:01:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:01:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce69134f0203d1fe5115a1020137046d1c890b6f1a46f116d7923e7ce02d4b8`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bdbc3a8aa8079aaea6f5d5bd5b05bddcc86c669a7140435e2b3021beba5928`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5681b086406e5a0268c2b3349357d0fd9c5ddf7e6ad703841e962f1c16b81e`  
		Last Modified: Thu, 02 Dec 2021 17:02:24 GMT  
		Size: 4.7 MB (4745590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbddc9b5c4f841ea7887df8c071cc34894f11accda6eb68f03ac972530d2092`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d29046b99bda35823f2af6e8b7eda1ea3a2dda13cc35c63d5f388bf1c6ed9ab`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:076eed23d69622023465551277b292c4b20c7e53ff970f4ec2c0c88c721002a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35310451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558381a048e4dd5c28f2a72bdfb28f021302afc0b9044d17373f8513e2c57b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:37:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 13:37:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:37:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 13:37:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 13:37:57 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 13:37:58 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 13:38:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 13:38:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 13:38:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11307cfb62981d1477c624d0946d440cae59b97d5241be5622b4a1a2170b7087`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0b4f4a9f9d7183fa8a6390427dd6151121434bd32d1539e46a81b5b7195e9e`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498cf759f2f5ad49bf12c6c9162ea1c630f9fba1005c0a5cd96d9d40f3c3bc9c`  
		Last Modified: Tue, 21 Dec 2021 13:38:30 GMT  
		Size: 5.3 MB (5263680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7310cca9b3933670873fa963c55ba0370617e570124050a904a3eabfd50f0b8a`  
		Last Modified: Tue, 21 Dec 2021 13:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ebb7feec0bee35aea3ecb3f98485656fa38f1ef9c1c9faccf4d07b68e3ebbe`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:5b3875cce8fad4903a3c884cef05e5abad051bc9951e8e5410114e95e0dac53e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40258475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302f102ca38e8fbd96146e30bc1ab35ebeaf9330138e5b0b7d258e8c9cb0b61c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 21:50:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 21:50:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 21:50:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 21:51:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 21:51:10 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 21:51:11 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 21:51:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 21:51:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 21:51:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489da5566cb0c924c029e46f8dad5bcafab6d42a56da88a93f2801d29558ff51`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db213f8397acea926fb592d3befbbdb2c002c268a3d54cb1d5c2d98de07b6f00`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5a4ea8b87e71f3244324d2ead099212bccde6f64ef51cbe9d8ec4d43b36028`  
		Last Modified: Tue, 21 Dec 2021 21:52:08 GMT  
		Size: 7.9 MB (7884366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5619dad69ca0adbec11d01730713268fe39795d31498b6b4fe5494a59579236`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3945ddda45549df85f0eed7cab7fef6325fd37f1b4ef32546894d2af03acfd`  
		Last Modified: Tue, 21 Dec 2021 21:52:04 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:fbd96eab48f0706b211bc89e1e78f7630d8d467ac4c32a9a27b78651c2329258
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b3265725ae631fc1fa2baaa91faa5aac9b516c810f7ca4ece4cbf3c1dc55c65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 03:09:10 GMT
ADD file:419aff162077eb16923c3ede6455ca86756a929a5a837bc6ac6b8dc67913503a in / 
# Thu, 02 Dec 2021 03:09:10 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 12:30:36 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 03 Dec 2021 12:30:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 12:30:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 03 Dec 2021 12:31:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 03 Dec 2021 12:31:58 GMT
VOLUME [/spiped]
# Fri, 03 Dec 2021 12:31:58 GMT
WORKDIR /spiped
# Fri, 03 Dec 2021 12:31:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 03 Dec 2021 12:31:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 12:32:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df61fb15db6391af55d70bc3c0db3e9014438c81bf802619fb527221adf5e8a8`  
		Last Modified: Thu, 02 Dec 2021 03:17:58 GMT  
		Size: 29.6 MB (29630496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4804017e9aaf0b2cb114927e3f0bc9e8f6bf173f5add775eb58fdac387f7c23`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3edbf43f07b9dbfec975a7a185719337d830354ede383efbf8964fd29e88d7`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81edd02fe261e7da19a1774f5be1249c6084f65e17d566a33e234ccb73c61d60`  
		Last Modified: Fri, 03 Dec 2021 12:32:16 GMT  
		Size: 5.7 MB (5706134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d174fb700fa19b4b4f80aeba64057df901a4197213c60299a2721db837bb5a`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013cb4b0da609efc6a5d97090c932a4d4c2c7438057ee994b3df9828ae89072c`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:c4ab963378b566c625302fe8f6c2b541809cf43971b0e2bf17f9469446444777
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41276244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adaff4ae366ea0ae358b47d0091afe6566648f17243e25696f1d34b3650def8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:51:38 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 20:51:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 20:51:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 20:53:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 20:53:56 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 20:54:00 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 20:54:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 20:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 20:54:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880dff15961bfe01347887de4bb7d190126f69b5a3854acfe06c435f9a6f626e`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5e1e31bc84bb0bae8ebf518013f4bb5d706f4272c1805bbc5f219a5a7eba2c`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af77ac291d1f734c93e02eff952dcdc14b498d4e4139e1a940654a936255dd92`  
		Last Modified: Thu, 02 Dec 2021 20:54:48 GMT  
		Size: 6.0 MB (6001592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a814520e36f0aaaa383f2659b8a9ca3b25c94875ecc23578898ebebdd5fb26`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721756d3adc4340983195bc3bf63aeaad3faaad5a572a351213a923b3d9b458`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:6ca814db8831771b57c2fc6fec100a2a7172d558595020784313b259c022266e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34829005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123f2f35891cf31904936c0d30cebe83dde721ab69f4d0b103091bc34e002fe6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 11:22:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 11:22:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 11:22:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 11:23:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 11:23:21 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 11:23:22 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 11:23:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 11:23:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 11:23:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1ef12e9110fade1b5f49cd9bd409a215546e6a659caf0b7c782b63e68b435d`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc8f56cc872687f2f42c48ebccd7820d167ec5866466852bb6646f18e519803`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5ad9022f51f5dafe11dbde04206e78d75fffe06678398a3ed65c9cdf16e303`  
		Last Modified: Tue, 21 Dec 2021 11:24:01 GMT  
		Size: 5.2 MB (5184106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f5e0810a75c82e2c625f9723799e72c4c00697d471245d2df256a5490e7049`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcfe444b90c33b185e97434acae972e7f8cdcb010a7fa9709cef3db394bc323`  
		Last Modified: Tue, 21 Dec 2021 11:24:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:1447fc83864d467400e6d1b2a87532955de7649123545804894c2a8c86d6a34a
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
$ docker pull spiped@sha256:5759c6e68d7e93789c7fc574722f42f3d3bafcaab2c4a8aeeeac5bb4772012a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc3e3a8422cee08ac18b30d97939a3a6bd28e94a61d0caaaa96ff86dd8f425c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:30:36 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 07:30:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 07:30:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 07:31:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 07:31:02 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 07:31:03 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 07:31:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 07:31:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 07:31:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d272f2608cb29aaf56aaa58c4e8245793833d52257971c0a4a90c1445945548`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bebf547583661fb31be182d777849262971941c241f7b072c041f54e3c4ff`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f41a1ab4447065d651caf78075639eb1027290f0756c4d489a10c43a745af`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 213.1 KB (213113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7a22ad75e07e938780270586c7d97ddd070bf6b70ee31e6fbe14b6c79cda6`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b484100590c35b883633e127830518528f9cc47bce7f4b864394b4bd85acb54`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:e54c9ae8aa1651b3704440b6b74cbdd5ac80086e8fa25252df5ffbe44591eade
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2847905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b358d015e8acc6b6eac3e79c5fc5302785d8bce806dc4640e51e684fc73495`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:56:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 06:56:48 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 06:56:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 06:57:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 06:57:27 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 06:57:27 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 06:57:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 06:57:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:57:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbee8633a3e2da897713dd8453113fc924e1ad102e43bc673e5aa4e72a3c5ff6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421d84dfbecebc99f29f801626a8781142421b8affb55b6dac49de522afdd86`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 7.8 KB (7780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67a331696441ca0da524281edcd53ee4b8d52a24b4fdaab4f5b2e3833ab74a`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 203.0 KB (202993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ab514374a45d9fd16341748dc013e94fd9ddf0b15c2f3666bea84a2c2db7dd`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526ec51047ed2d4267785d4387f46cebef6e388cb755c73b640a73e44db871b6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8b3e418343ca28cc6af7c79a9c92f500d16214863644d56f2e6a6c6a66f457d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2644452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edd8179550b7c42a3827056d11ba4da9c0f384e1b5ac66177b911a1a9f75acc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:09:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:09:21 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:09:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:09:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:09:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:09:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2462c3e2387f9df1b6daae812a3674ccd49db10b9b7251881ea1a034a39185b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e4892bdd8b9be427ec2794ea13c95ec6cca78353d3c032d0fd2ba5acf9bae3`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 7.8 KB (7791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624ff05273c8a204e1361bc188430fe618799c3ec5471284aa49a1f9bd365020`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 196.3 KB (196302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f127d56c30dd5e8a58309b3d42c9c4f974256b6b1f1f9ff32b0ff78d8c372b3b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab7e0d291c6010513c0721d4abf0cd1f407a631c23f515859004dddf983c5f5`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ed9db1b4a0c65f0ca88573ca4e82bafaedde5032f465971dba93432ddcf67f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3064332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04afce967f7cf45ad1faa0b6e1d955f2bad9d1aff37c3659db5e809170762140`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:40:39 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 20:40:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 20:40:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 20:41:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 20:41:14 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 20:41:14 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 20:41:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 20:41:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea20678ed9ffc78867f8fc9674162184169da3d7c198cd24ec6b7439e0c88`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f04cc4ba71752a6b9075421e6b0b7f08625406fb105f85e23547c4eb23b25f3`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae957cbfbd7f9f36494cb3954e91d1ead35e68d61bbddf48904c4b6133c4c878`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 223.9 KB (223875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911b8888c5d7d41e887ed34d5f9c93d1d3241ad814e69f4d7def6b5debc96ae8`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d46a3df042754e1b8e655e102bf789f899a1f3758442759be66fe90573dbd2`  
		Last Modified: Fri, 12 Nov 2021 20:41:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:892b50ba6b7bed8e6253a2577dcb2c38d0e60b1ae71968d978a808094e610768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3048694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7522decac983b5c7f6951cee379a5207bdbe044c9371a89a784e025923deb04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:29:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 15:29:55 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 15:29:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 15:30:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 15:30:32 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 15:30:34 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 15:30:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 15:30:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63441839c077959763f01da2aec624ff02d5765af3e923419046fe79761bf71d`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907f83f2fcbfe22132bde253d7c486b65870dc9635bc53461fab20a90a87ad73`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 7.8 KB (7777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6096cf0d6847df2dfecdd48192e3922a4bbc85ed08ddfab7f33b335ffb6dc77`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 221.7 KB (221712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51da854d577591f12d32b8d52aeb0c4576b7254377303693f07d6a4854ef5f`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1d81a9ee14a2ec2938cd589d2bda48191378ac5f8717102a0203b9d37df9ff`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:118a8c071df238ccc4affa6c1ad90ecaa58fd6f20861ee190449b34b1f5734bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2824562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a068554fae2e46941a18261fe2601c6c40df867a7b227b9bf154694451ba5390`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:55:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:55:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:55:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:56:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:56:06 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:56:06 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:56:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:56:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc797db23a37010d6b83bb8a9eaa1336ed352043857e5a44d68a4b8efad9e0b5`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e810eed7330856c73daba855bc8adf50fdde87ccab6697c3416ee314886ca`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 7.8 KB (7775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a425358f95dbc88c89aac4c0c745bacaceb3d4598a051af18b0df4a28d76e`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 205.8 KB (205773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c7009eddad4f11d690d41e57f47828edf66b3f5113d35cf2a68eee8beed75`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522513383757fa4cc180054c6b6b641c302050e0dce5ddfdd2a8881e7efcfa2`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:72d5844d36f4a0ae5b0828c8e434c770fe7ca47b2e901fbeaf9670adcefc44ce
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
$ docker pull spiped@sha256:2bd2286a40c61a56f280444f68f9c3d0ae7a310858860aba77b0403b8890c9f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37321326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4914da9141203212b68712b5f3a3711294f5e0e02a612eec74bd1b2e1241b9b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 12:54:46 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 12:54:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:54:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 12:55:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 12:55:16 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 12:55:16 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 12:55:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 12:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 12:55:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5942a3089c9d199ffd7567fc18e1491777fdade26ec8bdf4d160bf3c8d83f324`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643f2d189091c21b4eee0a6fe6553c7c7ad5a1fba49319eac9c272a96ac7fbdd`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f16287ae7ba5070d7edb0070fe71b973932136de80e4a4dd1013707e336b0c7`  
		Last Modified: Tue, 21 Dec 2021 12:55:41 GMT  
		Size: 6.0 MB (5960446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e68e4478591fe99bf722077de675519de67d719f9677d67f1ddc4d8f2cec294`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587fde5003f001f256acac00acf4ea7b0205ea8770d68ee6a9a2d3c87c369d95`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:613ef7662f31f09717e32907426042a146b7a0dc66e68870888cb83f73518f22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33939189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f0656da52ff3c99f44f7de064c2a87f0da72fa7fbe3ed879cb8732d6b9c4313`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:37 GMT
ADD file:7debbdb237139cb08189976f79cfa64cfd71f5cc98dfb2f560b558acb5f7cec9 in / 
# Thu, 02 Dec 2021 02:50:38 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 19:44:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 19:44:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 19:44:43 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 19:45:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 19:45:46 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 19:45:46 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 19:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 19:45:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 19:45:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c5e429166894878430c39748965935f89ffa957667340c3c8bd872418dbce663`  
		Last Modified: Thu, 02 Dec 2021 03:09:28 GMT  
		Size: 28.9 MB (28910824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902a05874d1937e2586f2056f8e8c160fbcb072ecdf334c40d7d34b8c31d9943`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd0a53456b53b30461bd45c9e7454a16fe2efaf6f01fc7ba2d50b7010313872`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4abfa33026a378154de67b10639d745576834a515a1c132083ffda2a7d1c4d`  
		Last Modified: Thu, 02 Dec 2021 19:46:28 GMT  
		Size: 5.0 MB (5025111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e2166e45f5a0464a961c1a3f02059b4157a81ee9c7409a710a0aa5691cecee`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df3005de126704451e5d5a4bfc395ec490bce9a5df481a2a33cb5903873405`  
		Last Modified: Thu, 02 Dec 2021 19:46:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cd3cc375afa908acf4552d16cdb624e941a6315bbfe494df1c6b35e01d413a54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31322033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ec4a5f35bb1890066d68b0ee550709c5f39b841dd141dfcbb9582f2e1c3fc86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:00:09 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 17:00:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:00:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 17:01:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 17:01:17 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 17:01:17 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 17:01:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:01:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:01:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce69134f0203d1fe5115a1020137046d1c890b6f1a46f116d7923e7ce02d4b8`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bdbc3a8aa8079aaea6f5d5bd5b05bddcc86c669a7140435e2b3021beba5928`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5681b086406e5a0268c2b3349357d0fd9c5ddf7e6ad703841e962f1c16b81e`  
		Last Modified: Thu, 02 Dec 2021 17:02:24 GMT  
		Size: 4.7 MB (4745590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbddc9b5c4f841ea7887df8c071cc34894f11accda6eb68f03ac972530d2092`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d29046b99bda35823f2af6e8b7eda1ea3a2dda13cc35c63d5f388bf1c6ed9ab`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:076eed23d69622023465551277b292c4b20c7e53ff970f4ec2c0c88c721002a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35310451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558381a048e4dd5c28f2a72bdfb28f021302afc0b9044d17373f8513e2c57b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:37:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 13:37:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:37:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 13:37:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 13:37:57 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 13:37:58 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 13:38:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 13:38:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 13:38:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11307cfb62981d1477c624d0946d440cae59b97d5241be5622b4a1a2170b7087`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0b4f4a9f9d7183fa8a6390427dd6151121434bd32d1539e46a81b5b7195e9e`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498cf759f2f5ad49bf12c6c9162ea1c630f9fba1005c0a5cd96d9d40f3c3bc9c`  
		Last Modified: Tue, 21 Dec 2021 13:38:30 GMT  
		Size: 5.3 MB (5263680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7310cca9b3933670873fa963c55ba0370617e570124050a904a3eabfd50f0b8a`  
		Last Modified: Tue, 21 Dec 2021 13:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ebb7feec0bee35aea3ecb3f98485656fa38f1ef9c1c9faccf4d07b68e3ebbe`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:5b3875cce8fad4903a3c884cef05e5abad051bc9951e8e5410114e95e0dac53e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40258475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302f102ca38e8fbd96146e30bc1ab35ebeaf9330138e5b0b7d258e8c9cb0b61c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 21:50:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 21:50:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 21:50:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 21:51:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 21:51:10 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 21:51:11 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 21:51:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 21:51:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 21:51:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489da5566cb0c924c029e46f8dad5bcafab6d42a56da88a93f2801d29558ff51`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db213f8397acea926fb592d3befbbdb2c002c268a3d54cb1d5c2d98de07b6f00`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5a4ea8b87e71f3244324d2ead099212bccde6f64ef51cbe9d8ec4d43b36028`  
		Last Modified: Tue, 21 Dec 2021 21:52:08 GMT  
		Size: 7.9 MB (7884366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5619dad69ca0adbec11d01730713268fe39795d31498b6b4fe5494a59579236`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3945ddda45549df85f0eed7cab7fef6325fd37f1b4ef32546894d2af03acfd`  
		Last Modified: Tue, 21 Dec 2021 21:52:04 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:fbd96eab48f0706b211bc89e1e78f7630d8d467ac4c32a9a27b78651c2329258
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b3265725ae631fc1fa2baaa91faa5aac9b516c810f7ca4ece4cbf3c1dc55c65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 03:09:10 GMT
ADD file:419aff162077eb16923c3ede6455ca86756a929a5a837bc6ac6b8dc67913503a in / 
# Thu, 02 Dec 2021 03:09:10 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 12:30:36 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 03 Dec 2021 12:30:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 12:30:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 03 Dec 2021 12:31:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 03 Dec 2021 12:31:58 GMT
VOLUME [/spiped]
# Fri, 03 Dec 2021 12:31:58 GMT
WORKDIR /spiped
# Fri, 03 Dec 2021 12:31:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 03 Dec 2021 12:31:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 12:32:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df61fb15db6391af55d70bc3c0db3e9014438c81bf802619fb527221adf5e8a8`  
		Last Modified: Thu, 02 Dec 2021 03:17:58 GMT  
		Size: 29.6 MB (29630496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4804017e9aaf0b2cb114927e3f0bc9e8f6bf173f5add775eb58fdac387f7c23`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3edbf43f07b9dbfec975a7a185719337d830354ede383efbf8964fd29e88d7`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81edd02fe261e7da19a1774f5be1249c6084f65e17d566a33e234ccb73c61d60`  
		Last Modified: Fri, 03 Dec 2021 12:32:16 GMT  
		Size: 5.7 MB (5706134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d174fb700fa19b4b4f80aeba64057df901a4197213c60299a2721db837bb5a`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013cb4b0da609efc6a5d97090c932a4d4c2c7438057ee994b3df9828ae89072c`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:c4ab963378b566c625302fe8f6c2b541809cf43971b0e2bf17f9469446444777
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41276244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adaff4ae366ea0ae358b47d0091afe6566648f17243e25696f1d34b3650def8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:51:38 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 20:51:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 20:51:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 20:53:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 20:53:56 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 20:54:00 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 20:54:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 20:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 20:54:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880dff15961bfe01347887de4bb7d190126f69b5a3854acfe06c435f9a6f626e`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5e1e31bc84bb0bae8ebf518013f4bb5d706f4272c1805bbc5f219a5a7eba2c`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af77ac291d1f734c93e02eff952dcdc14b498d4e4139e1a940654a936255dd92`  
		Last Modified: Thu, 02 Dec 2021 20:54:48 GMT  
		Size: 6.0 MB (6001592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a814520e36f0aaaa383f2659b8a9ca3b25c94875ecc23578898ebebdd5fb26`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721756d3adc4340983195bc3bf63aeaad3faaad5a572a351213a923b3d9b458`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:6ca814db8831771b57c2fc6fec100a2a7172d558595020784313b259c022266e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34829005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123f2f35891cf31904936c0d30cebe83dde721ab69f4d0b103091bc34e002fe6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 11:22:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 11:22:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 11:22:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 11:23:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 11:23:21 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 11:23:22 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 11:23:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 11:23:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 11:23:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1ef12e9110fade1b5f49cd9bd409a215546e6a659caf0b7c782b63e68b435d`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc8f56cc872687f2f42c48ebccd7820d167ec5866466852bb6646f18e519803`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5ad9022f51f5dafe11dbde04206e78d75fffe06678398a3ed65c9cdf16e303`  
		Last Modified: Tue, 21 Dec 2021 11:24:01 GMT  
		Size: 5.2 MB (5184106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f5e0810a75c82e2c625f9723799e72c4c00697d471245d2df256a5490e7049`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcfe444b90c33b185e97434acae972e7f8cdcb010a7fa9709cef3db394bc323`  
		Last Modified: Tue, 21 Dec 2021 11:24:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:1447fc83864d467400e6d1b2a87532955de7649123545804894c2a8c86d6a34a
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
$ docker pull spiped@sha256:5759c6e68d7e93789c7fc574722f42f3d3bafcaab2c4a8aeeeac5bb4772012a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc3e3a8422cee08ac18b30d97939a3a6bd28e94a61d0caaaa96ff86dd8f425c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:30:36 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 07:30:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 07:30:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 07:31:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 07:31:02 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 07:31:03 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 07:31:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 07:31:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 07:31:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d272f2608cb29aaf56aaa58c4e8245793833d52257971c0a4a90c1445945548`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bebf547583661fb31be182d777849262971941c241f7b072c041f54e3c4ff`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f41a1ab4447065d651caf78075639eb1027290f0756c4d489a10c43a745af`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 213.1 KB (213113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7a22ad75e07e938780270586c7d97ddd070bf6b70ee31e6fbe14b6c79cda6`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b484100590c35b883633e127830518528f9cc47bce7f4b864394b4bd85acb54`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:e54c9ae8aa1651b3704440b6b74cbdd5ac80086e8fa25252df5ffbe44591eade
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2847905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b358d015e8acc6b6eac3e79c5fc5302785d8bce806dc4640e51e684fc73495`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:56:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 06:56:48 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 06:56:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 06:57:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 06:57:27 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 06:57:27 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 06:57:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 06:57:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:57:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbee8633a3e2da897713dd8453113fc924e1ad102e43bc673e5aa4e72a3c5ff6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421d84dfbecebc99f29f801626a8781142421b8affb55b6dac49de522afdd86`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 7.8 KB (7780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67a331696441ca0da524281edcd53ee4b8d52a24b4fdaab4f5b2e3833ab74a`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 203.0 KB (202993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ab514374a45d9fd16341748dc013e94fd9ddf0b15c2f3666bea84a2c2db7dd`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526ec51047ed2d4267785d4387f46cebef6e388cb755c73b640a73e44db871b6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8b3e418343ca28cc6af7c79a9c92f500d16214863644d56f2e6a6c6a66f457d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2644452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edd8179550b7c42a3827056d11ba4da9c0f384e1b5ac66177b911a1a9f75acc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:09:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:09:21 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:09:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:09:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:09:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:09:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2462c3e2387f9df1b6daae812a3674ccd49db10b9b7251881ea1a034a39185b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e4892bdd8b9be427ec2794ea13c95ec6cca78353d3c032d0fd2ba5acf9bae3`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 7.8 KB (7791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624ff05273c8a204e1361bc188430fe618799c3ec5471284aa49a1f9bd365020`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 196.3 KB (196302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f127d56c30dd5e8a58309b3d42c9c4f974256b6b1f1f9ff32b0ff78d8c372b3b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab7e0d291c6010513c0721d4abf0cd1f407a631c23f515859004dddf983c5f5`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ed9db1b4a0c65f0ca88573ca4e82bafaedde5032f465971dba93432ddcf67f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3064332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04afce967f7cf45ad1faa0b6e1d955f2bad9d1aff37c3659db5e809170762140`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:40:39 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 20:40:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 20:40:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 20:41:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 20:41:14 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 20:41:14 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 20:41:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 20:41:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea20678ed9ffc78867f8fc9674162184169da3d7c198cd24ec6b7439e0c88`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f04cc4ba71752a6b9075421e6b0b7f08625406fb105f85e23547c4eb23b25f3`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae957cbfbd7f9f36494cb3954e91d1ead35e68d61bbddf48904c4b6133c4c878`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 223.9 KB (223875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911b8888c5d7d41e887ed34d5f9c93d1d3241ad814e69f4d7def6b5debc96ae8`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d46a3df042754e1b8e655e102bf789f899a1f3758442759be66fe90573dbd2`  
		Last Modified: Fri, 12 Nov 2021 20:41:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:892b50ba6b7bed8e6253a2577dcb2c38d0e60b1ae71968d978a808094e610768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3048694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7522decac983b5c7f6951cee379a5207bdbe044c9371a89a784e025923deb04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:29:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 15:29:55 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 15:29:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 15:30:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 15:30:32 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 15:30:34 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 15:30:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 15:30:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63441839c077959763f01da2aec624ff02d5765af3e923419046fe79761bf71d`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907f83f2fcbfe22132bde253d7c486b65870dc9635bc53461fab20a90a87ad73`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 7.8 KB (7777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6096cf0d6847df2dfecdd48192e3922a4bbc85ed08ddfab7f33b335ffb6dc77`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 221.7 KB (221712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51da854d577591f12d32b8d52aeb0c4576b7254377303693f07d6a4854ef5f`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1d81a9ee14a2ec2938cd589d2bda48191378ac5f8717102a0203b9d37df9ff`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:118a8c071df238ccc4affa6c1ad90ecaa58fd6f20861ee190449b34b1f5734bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2824562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a068554fae2e46941a18261fe2601c6c40df867a7b227b9bf154694451ba5390`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:55:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:55:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:55:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:56:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:56:06 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:56:06 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:56:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:56:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc797db23a37010d6b83bb8a9eaa1336ed352043857e5a44d68a4b8efad9e0b5`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e810eed7330856c73daba855bc8adf50fdde87ccab6697c3416ee314886ca`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 7.8 KB (7775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a425358f95dbc88c89aac4c0c745bacaceb3d4598a051af18b0df4a28d76e`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 205.8 KB (205773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c7009eddad4f11d690d41e57f47828edf66b3f5113d35cf2a68eee8beed75`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522513383757fa4cc180054c6b6b641c302050e0dce5ddfdd2a8881e7efcfa2`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:1447fc83864d467400e6d1b2a87532955de7649123545804894c2a8c86d6a34a
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
$ docker pull spiped@sha256:5759c6e68d7e93789c7fc574722f42f3d3bafcaab2c4a8aeeeac5bb4772012a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc3e3a8422cee08ac18b30d97939a3a6bd28e94a61d0caaaa96ff86dd8f425c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:30:36 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 07:30:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 07:30:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 07:31:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 07:31:02 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 07:31:03 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 07:31:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 07:31:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 07:31:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d272f2608cb29aaf56aaa58c4e8245793833d52257971c0a4a90c1445945548`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bebf547583661fb31be182d777849262971941c241f7b072c041f54e3c4ff`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f41a1ab4447065d651caf78075639eb1027290f0756c4d489a10c43a745af`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 213.1 KB (213113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7a22ad75e07e938780270586c7d97ddd070bf6b70ee31e6fbe14b6c79cda6`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b484100590c35b883633e127830518528f9cc47bce7f4b864394b4bd85acb54`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:e54c9ae8aa1651b3704440b6b74cbdd5ac80086e8fa25252df5ffbe44591eade
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2847905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b358d015e8acc6b6eac3e79c5fc5302785d8bce806dc4640e51e684fc73495`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:56:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 06:56:48 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 06:56:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 06:57:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 06:57:27 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 06:57:27 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 06:57:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 06:57:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:57:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbee8633a3e2da897713dd8453113fc924e1ad102e43bc673e5aa4e72a3c5ff6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421d84dfbecebc99f29f801626a8781142421b8affb55b6dac49de522afdd86`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 7.8 KB (7780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67a331696441ca0da524281edcd53ee4b8d52a24b4fdaab4f5b2e3833ab74a`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 203.0 KB (202993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ab514374a45d9fd16341748dc013e94fd9ddf0b15c2f3666bea84a2c2db7dd`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526ec51047ed2d4267785d4387f46cebef6e388cb755c73b640a73e44db871b6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8b3e418343ca28cc6af7c79a9c92f500d16214863644d56f2e6a6c6a66f457d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2644452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edd8179550b7c42a3827056d11ba4da9c0f384e1b5ac66177b911a1a9f75acc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:09:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:09:21 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:09:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:09:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:09:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:09:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2462c3e2387f9df1b6daae812a3674ccd49db10b9b7251881ea1a034a39185b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e4892bdd8b9be427ec2794ea13c95ec6cca78353d3c032d0fd2ba5acf9bae3`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 7.8 KB (7791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624ff05273c8a204e1361bc188430fe618799c3ec5471284aa49a1f9bd365020`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 196.3 KB (196302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f127d56c30dd5e8a58309b3d42c9c4f974256b6b1f1f9ff32b0ff78d8c372b3b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab7e0d291c6010513c0721d4abf0cd1f407a631c23f515859004dddf983c5f5`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:ed9db1b4a0c65f0ca88573ca4e82bafaedde5032f465971dba93432ddcf67f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3064332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04afce967f7cf45ad1faa0b6e1d955f2bad9d1aff37c3659db5e809170762140`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:40:39 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 20:40:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 20:40:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 20:41:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 20:41:14 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 20:41:14 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 20:41:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 20:41:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea20678ed9ffc78867f8fc9674162184169da3d7c198cd24ec6b7439e0c88`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f04cc4ba71752a6b9075421e6b0b7f08625406fb105f85e23547c4eb23b25f3`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae957cbfbd7f9f36494cb3954e91d1ead35e68d61bbddf48904c4b6133c4c878`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 223.9 KB (223875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911b8888c5d7d41e887ed34d5f9c93d1d3241ad814e69f4d7def6b5debc96ae8`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d46a3df042754e1b8e655e102bf789f899a1f3758442759be66fe90573dbd2`  
		Last Modified: Fri, 12 Nov 2021 20:41:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:892b50ba6b7bed8e6253a2577dcb2c38d0e60b1ae71968d978a808094e610768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3048694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7522decac983b5c7f6951cee379a5207bdbe044c9371a89a784e025923deb04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:29:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 15:29:55 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 15:29:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 15:30:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 15:30:32 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 15:30:34 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 15:30:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 15:30:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63441839c077959763f01da2aec624ff02d5765af3e923419046fe79761bf71d`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907f83f2fcbfe22132bde253d7c486b65870dc9635bc53461fab20a90a87ad73`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 7.8 KB (7777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6096cf0d6847df2dfecdd48192e3922a4bbc85ed08ddfab7f33b335ffb6dc77`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 221.7 KB (221712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51da854d577591f12d32b8d52aeb0c4576b7254377303693f07d6a4854ef5f`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1d81a9ee14a2ec2938cd589d2bda48191378ac5f8717102a0203b9d37df9ff`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:118a8c071df238ccc4affa6c1ad90ecaa58fd6f20861ee190449b34b1f5734bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2824562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a068554fae2e46941a18261fe2601c6c40df867a7b227b9bf154694451ba5390`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:55:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:55:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:55:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:56:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:56:06 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:56:06 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:56:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:56:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc797db23a37010d6b83bb8a9eaa1336ed352043857e5a44d68a4b8efad9e0b5`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e810eed7330856c73daba855bc8adf50fdde87ccab6697c3416ee314886ca`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 7.8 KB (7775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a425358f95dbc88c89aac4c0c745bacaceb3d4598a051af18b0df4a28d76e`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 205.8 KB (205773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c7009eddad4f11d690d41e57f47828edf66b3f5113d35cf2a68eee8beed75`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522513383757fa4cc180054c6b6b641c302050e0dce5ddfdd2a8881e7efcfa2`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:72d5844d36f4a0ae5b0828c8e434c770fe7ca47b2e901fbeaf9670adcefc44ce
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
$ docker pull spiped@sha256:2bd2286a40c61a56f280444f68f9c3d0ae7a310858860aba77b0403b8890c9f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37321326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4914da9141203212b68712b5f3a3711294f5e0e02a612eec74bd1b2e1241b9b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 12:54:46 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 12:54:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:54:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 12:55:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 12:55:16 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 12:55:16 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 12:55:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 12:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 12:55:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5942a3089c9d199ffd7567fc18e1491777fdade26ec8bdf4d160bf3c8d83f324`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643f2d189091c21b4eee0a6fe6553c7c7ad5a1fba49319eac9c272a96ac7fbdd`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f16287ae7ba5070d7edb0070fe71b973932136de80e4a4dd1013707e336b0c7`  
		Last Modified: Tue, 21 Dec 2021 12:55:41 GMT  
		Size: 6.0 MB (5960446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e68e4478591fe99bf722077de675519de67d719f9677d67f1ddc4d8f2cec294`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587fde5003f001f256acac00acf4ea7b0205ea8770d68ee6a9a2d3c87c369d95`  
		Last Modified: Tue, 21 Dec 2021 12:55:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:613ef7662f31f09717e32907426042a146b7a0dc66e68870888cb83f73518f22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33939189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f0656da52ff3c99f44f7de064c2a87f0da72fa7fbe3ed879cb8732d6b9c4313`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:37 GMT
ADD file:7debbdb237139cb08189976f79cfa64cfd71f5cc98dfb2f560b558acb5f7cec9 in / 
# Thu, 02 Dec 2021 02:50:38 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 19:44:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 19:44:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 19:44:43 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 19:45:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 19:45:46 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 19:45:46 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 19:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 19:45:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 19:45:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c5e429166894878430c39748965935f89ffa957667340c3c8bd872418dbce663`  
		Last Modified: Thu, 02 Dec 2021 03:09:28 GMT  
		Size: 28.9 MB (28910824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902a05874d1937e2586f2056f8e8c160fbcb072ecdf334c40d7d34b8c31d9943`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd0a53456b53b30461bd45c9e7454a16fe2efaf6f01fc7ba2d50b7010313872`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4abfa33026a378154de67b10639d745576834a515a1c132083ffda2a7d1c4d`  
		Last Modified: Thu, 02 Dec 2021 19:46:28 GMT  
		Size: 5.0 MB (5025111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e2166e45f5a0464a961c1a3f02059b4157a81ee9c7409a710a0aa5691cecee`  
		Last Modified: Thu, 02 Dec 2021 19:46:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df3005de126704451e5d5a4bfc395ec490bce9a5df481a2a33cb5903873405`  
		Last Modified: Thu, 02 Dec 2021 19:46:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cd3cc375afa908acf4552d16cdb624e941a6315bbfe494df1c6b35e01d413a54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31322033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ec4a5f35bb1890066d68b0ee550709c5f39b841dd141dfcbb9582f2e1c3fc86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:00:09 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 17:00:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:00:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 17:01:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 17:01:17 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 17:01:17 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 17:01:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:01:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:01:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce69134f0203d1fe5115a1020137046d1c890b6f1a46f116d7923e7ce02d4b8`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bdbc3a8aa8079aaea6f5d5bd5b05bddcc86c669a7140435e2b3021beba5928`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5681b086406e5a0268c2b3349357d0fd9c5ddf7e6ad703841e962f1c16b81e`  
		Last Modified: Thu, 02 Dec 2021 17:02:24 GMT  
		Size: 4.7 MB (4745590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbddc9b5c4f841ea7887df8c071cc34894f11accda6eb68f03ac972530d2092`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d29046b99bda35823f2af6e8b7eda1ea3a2dda13cc35c63d5f388bf1c6ed9ab`  
		Last Modified: Thu, 02 Dec 2021 17:02:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:076eed23d69622023465551277b292c4b20c7e53ff970f4ec2c0c88c721002a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35310451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558381a048e4dd5c28f2a72bdfb28f021302afc0b9044d17373f8513e2c57b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:37:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 13:37:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:37:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 13:37:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 13:37:57 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 13:37:58 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 13:38:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 13:38:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 13:38:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11307cfb62981d1477c624d0946d440cae59b97d5241be5622b4a1a2170b7087`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0b4f4a9f9d7183fa8a6390427dd6151121434bd32d1539e46a81b5b7195e9e`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498cf759f2f5ad49bf12c6c9162ea1c630f9fba1005c0a5cd96d9d40f3c3bc9c`  
		Last Modified: Tue, 21 Dec 2021 13:38:30 GMT  
		Size: 5.3 MB (5263680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7310cca9b3933670873fa963c55ba0370617e570124050a904a3eabfd50f0b8a`  
		Last Modified: Tue, 21 Dec 2021 13:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ebb7feec0bee35aea3ecb3f98485656fa38f1ef9c1c9faccf4d07b68e3ebbe`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:5b3875cce8fad4903a3c884cef05e5abad051bc9951e8e5410114e95e0dac53e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40258475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302f102ca38e8fbd96146e30bc1ab35ebeaf9330138e5b0b7d258e8c9cb0b61c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 21:50:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 21:50:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 21:50:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 21:51:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 21:51:10 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 21:51:11 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 21:51:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 21:51:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 21:51:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489da5566cb0c924c029e46f8dad5bcafab6d42a56da88a93f2801d29558ff51`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db213f8397acea926fb592d3befbbdb2c002c268a3d54cb1d5c2d98de07b6f00`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5a4ea8b87e71f3244324d2ead099212bccde6f64ef51cbe9d8ec4d43b36028`  
		Last Modified: Tue, 21 Dec 2021 21:52:08 GMT  
		Size: 7.9 MB (7884366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5619dad69ca0adbec11d01730713268fe39795d31498b6b4fe5494a59579236`  
		Last Modified: Tue, 21 Dec 2021 21:52:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3945ddda45549df85f0eed7cab7fef6325fd37f1b4ef32546894d2af03acfd`  
		Last Modified: Tue, 21 Dec 2021 21:52:04 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:fbd96eab48f0706b211bc89e1e78f7630d8d467ac4c32a9a27b78651c2329258
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b3265725ae631fc1fa2baaa91faa5aac9b516c810f7ca4ece4cbf3c1dc55c65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 03:09:10 GMT
ADD file:419aff162077eb16923c3ede6455ca86756a929a5a837bc6ac6b8dc67913503a in / 
# Thu, 02 Dec 2021 03:09:10 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 12:30:36 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 03 Dec 2021 12:30:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 12:30:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 03 Dec 2021 12:31:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 03 Dec 2021 12:31:58 GMT
VOLUME [/spiped]
# Fri, 03 Dec 2021 12:31:58 GMT
WORKDIR /spiped
# Fri, 03 Dec 2021 12:31:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 03 Dec 2021 12:31:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 12:32:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df61fb15db6391af55d70bc3c0db3e9014438c81bf802619fb527221adf5e8a8`  
		Last Modified: Thu, 02 Dec 2021 03:17:58 GMT  
		Size: 29.6 MB (29630496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4804017e9aaf0b2cb114927e3f0bc9e8f6bf173f5add775eb58fdac387f7c23`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3edbf43f07b9dbfec975a7a185719337d830354ede383efbf8964fd29e88d7`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81edd02fe261e7da19a1774f5be1249c6084f65e17d566a33e234ccb73c61d60`  
		Last Modified: Fri, 03 Dec 2021 12:32:16 GMT  
		Size: 5.7 MB (5706134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d174fb700fa19b4b4f80aeba64057df901a4197213c60299a2721db837bb5a`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013cb4b0da609efc6a5d97090c932a4d4c2c7438057ee994b3df9828ae89072c`  
		Last Modified: Fri, 03 Dec 2021 12:32:10 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:c4ab963378b566c625302fe8f6c2b541809cf43971b0e2bf17f9469446444777
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41276244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adaff4ae366ea0ae358b47d0091afe6566648f17243e25696f1d34b3650def8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:51:38 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 02 Dec 2021 20:51:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 20:51:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 02 Dec 2021 20:53:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 02 Dec 2021 20:53:56 GMT
VOLUME [/spiped]
# Thu, 02 Dec 2021 20:54:00 GMT
WORKDIR /spiped
# Thu, 02 Dec 2021 20:54:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 02 Dec 2021 20:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 20:54:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880dff15961bfe01347887de4bb7d190126f69b5a3854acfe06c435f9a6f626e`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5e1e31bc84bb0bae8ebf518013f4bb5d706f4272c1805bbc5f219a5a7eba2c`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af77ac291d1f734c93e02eff952dcdc14b498d4e4139e1a940654a936255dd92`  
		Last Modified: Thu, 02 Dec 2021 20:54:48 GMT  
		Size: 6.0 MB (6001592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a814520e36f0aaaa383f2659b8a9ca3b25c94875ecc23578898ebebdd5fb26`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721756d3adc4340983195bc3bf63aeaad3faaad5a572a351213a923b3d9b458`  
		Last Modified: Thu, 02 Dec 2021 20:54:46 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:6ca814db8831771b57c2fc6fec100a2a7172d558595020784313b259c022266e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34829005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123f2f35891cf31904936c0d30cebe83dde721ab69f4d0b103091bc34e002fe6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 11:22:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 11:22:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 11:22:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 11:23:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 11:23:21 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 11:23:22 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 11:23:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 11:23:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 11:23:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1ef12e9110fade1b5f49cd9bd409a215546e6a659caf0b7c782b63e68b435d`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc8f56cc872687f2f42c48ebccd7820d167ec5866466852bb6646f18e519803`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5ad9022f51f5dafe11dbde04206e78d75fffe06678398a3ed65c9cdf16e303`  
		Last Modified: Tue, 21 Dec 2021 11:24:01 GMT  
		Size: 5.2 MB (5184106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f5e0810a75c82e2c625f9723799e72c4c00697d471245d2df256a5490e7049`  
		Last Modified: Tue, 21 Dec 2021 11:24:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcfe444b90c33b185e97434acae972e7f8cdcb010a7fa9709cef3db394bc323`  
		Last Modified: Tue, 21 Dec 2021 11:24:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
