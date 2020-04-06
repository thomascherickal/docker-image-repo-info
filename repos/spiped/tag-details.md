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
$ docker pull spiped@sha256:836fc9b2c3d9321be72ed598f0c6d1261cb3d90393d6f00bf85d4c36ab09178c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:be1e1273f203254dbe788f80482ad7eb3dda4a61446fa4d8fe046d8d6b342ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de3a9d7ad126b00ea958b4f0240d31d91c8a8582af4ddac8570e1935de03c70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 17:53:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 17:54:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:12:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 21:12:54 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:12:55 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:12:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:12:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:12:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af711a0248b008edeb7fc3ec89d9b65d0e6bc9a7812f17e7c0e1981713091b0`  
		Last Modified: Tue, 31 Mar 2020 17:54:57 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf07c97371206072919de7231d4a5b645fc9214d9477f21dff3c4bcf2d836ca`  
		Last Modified: Tue, 31 Mar 2020 17:54:57 GMT  
		Size: 2.1 MB (2128010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf676d0d98d691716d2c2ac3f58d9300f97af52c37052d44f1991d468c20da`  
		Last Modified: Mon, 06 Apr 2020 21:13:51 GMT  
		Size: 7.0 MB (7037456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772658cc02099a47df92d23a2dc7b78ff48f02f3c5eae197d45e5595ca79dae3`  
		Last Modified: Mon, 06 Apr 2020 21:13:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9fba6c68631c186e227ec9fc3a8bec328a5ea49571cbd3718c6872dfa9474`  
		Last Modified: Mon, 06 Apr 2020 21:13:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:f1512fe235b70e455d37fddc35e243dff2ecf609dce90da107a166c6c540c525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32151424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c7ad750a45d0754af70700f3d5e90ef6f33eccae12c2028f74c6a55296138a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:54 GMT
ADD file:e08ed9e60228d351de400af5746474777a562d99f17e0cb1ce3e3d352e9ec751 in / 
# Tue, 31 Mar 2020 01:24:56 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 04:13:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 04:14:07 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:48:31 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:48:32 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:48:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:49:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:49:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:49:30 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:49:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:49:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:49:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:440df189aa3df85587f2d7d348500930481b3752dcb887d212de9b44b49076dd`  
		Last Modified: Tue, 31 Mar 2020 01:33:04 GMT  
		Size: 24.8 MB (24830324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3031ff195bb3799ebe4254f93022cc97bda6966cf5340f247941ae0a236bc8`  
		Last Modified: Tue, 31 Mar 2020 04:15:31 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e9b06f7ebf1fc3799d2a0fa1664e11b861e3055c54dcfd0283a0aef5350a0b`  
		Last Modified: Tue, 31 Mar 2020 04:15:32 GMT  
		Size: 1.8 MB (1839102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba06c78ab671b13c2cfd74f9c9cf70c5fae20022228334b4a980c1027c61b482`  
		Last Modified: Mon, 06 Apr 2020 19:49:55 GMT  
		Size: 5.5 MB (5479794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf7920a9f6fa89d2c56f50bd15154b9fafd77611107ba7e49820bf8bc72e407`  
		Last Modified: Mon, 06 Apr 2020 19:49:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d244a050acaaad3567ce421740a244acb6e028829c1cca06d9a1012d5c50eb`  
		Last Modified: Mon, 06 Apr 2020 19:49:52 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:eeac0857b6e2761fcb93405df2e77ec321bb99be3c1c74373781393b2ee92003
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29746810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ad38fadc7fdd89befc82a3c614c010ea03aacb9450975cb60cf90f9b0535a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:48:12 GMT
ADD file:8c3ed0df404a6bcaf7583e71796cb4c1f40e87288953a21d4ee5946079c3274f in / 
# Tue, 31 Mar 2020 01:48:13 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 08:18:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 08:19:21 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:58:19 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:58:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:58:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:59:07 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:08 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98098fa10651fdba12c848231b7428536a120e17637f1f9e0d25c63880483fcc`  
		Last Modified: Tue, 31 Mar 2020 01:56:24 GMT  
		Size: 22.7 MB (22699731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7922ddf1b86ac7ad159d24a62da9689447caf7b4c69ce081a02a73d055bff`  
		Last Modified: Tue, 31 Mar 2020 08:21:20 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754834d90b58f45e25a8bfa558985a0ced452414dde7e9d70e222afd86be2fa8`  
		Last Modified: Tue, 31 Mar 2020 08:21:20 GMT  
		Size: 1.8 MB (1759473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272af2fbbb3f2aed36f1844fb765e9759fdf25d0772754b0513fe9ddecc40b9d`  
		Last Modified: Mon, 06 Apr 2020 20:00:06 GMT  
		Size: 5.3 MB (5285397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daae49ef671f0947b4b1cab63d653ad548252e336511375fe7140efe4905f0e`  
		Last Modified: Mon, 06 Apr 2020 20:00:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63e1cc9b947e96c2587111ad56ab86d54be60134ccd9a807f0389c15ea3f61b`  
		Last Modified: Mon, 06 Apr 2020 20:00:04 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:78c250c7e5d01ce41983b2753680ba9b101af8c543f5c397b55ae10814cc22c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33766998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472dc2c5d0c415f63d802bf98ff0a6bd86cf5d0ccff488506dea4be4217c9ab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:32:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 20:32:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:52:02 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:52:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:52:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:52:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:52:52 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:52:53 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:52:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:52:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744144498f3e2946eaba16e1fc06cc2a6ed34447976d59e141a9f9156aa19624`  
		Last Modified: Tue, 31 Mar 2020 20:34:01 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c968861bade4527ff71063fced63ca4143f9886781be1af7a07993354297a112`  
		Last Modified: Tue, 31 Mar 2020 20:34:00 GMT  
		Size: 2.0 MB (2007812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf54b87406d4a55b55235b7c10eb81445f9e40f99ebbbc8eb130efa13646e25`  
		Last Modified: Mon, 06 Apr 2020 19:54:08 GMT  
		Size: 5.9 MB (5905328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3f664cad2767e1664990b44fa7e4d9e8c3388dbaf2e3bc0e651ae046f9656a`  
		Last Modified: Mon, 06 Apr 2020 19:53:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb3daa1131a9b59530b0c0153041fb324468bceadf2c9d1711ceb1ab935a3ff`  
		Last Modified: Mon, 06 Apr 2020 19:53:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:976ddfd647eff5d898a8247eebd96683505517ad3e705c1ca73a8c092504d336
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41515262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1cbef7c8e6271e24f80c06efcf46d494fb5b3575c7c33bc96e6a7e2ef120b2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 13:19:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 13:19:17 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:43:17 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:18 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1033102c2fb2ed5037246c60787ba3376aaf2e983140ea88b05d2fe1dcca139`  
		Last Modified: Tue, 31 Mar 2020 13:20:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a518aadc532142e2d36b269c309d07235a326660c35df16af78cf09726dc67dc`  
		Last Modified: Tue, 31 Mar 2020 13:20:04 GMT  
		Size: 2.1 MB (2132319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f408e0d5cb38c8d8bf6c2e778d473aa0a5b82f3c69420ff18840c2fe70390c4a`  
		Last Modified: Mon, 06 Apr 2020 19:44:01 GMT  
		Size: 11.6 MB (11633125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95a05714cd0087efcd7817104cf284e0a88823599b290eaf117bd64e6960c64`  
		Last Modified: Mon, 06 Apr 2020 19:43:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e6b7e5bc2f22c3c986e055952e8670bb45920a95990f5b4ab02eaa009baca6`  
		Last Modified: Mon, 06 Apr 2020 19:43:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:d3ba4984825c204c3dc09c4fa4cc5cffcdd761eed19e785d78dbbf577ef3510e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0562eea684e4b3839767d99691be0187e1f3b1bd1e3a717e660857408763f538`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:42 GMT
ADD file:36c02e92574faba45b64cfed78a0a0359d65ad175b17128bf554a2a5c0086ff5 in / 
# Tue, 31 Mar 2020 01:32:47 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 12:58:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 12:59:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 20:23:17 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:23:21 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:23:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 20:25:50 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:25:53 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:25:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:25:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:26:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9df6bbae5eeb29e9aac2f39cff517c694cce60f01ee477abcdedcd8e8c01c38f`  
		Last Modified: Tue, 31 Mar 2020 01:45:59 GMT  
		Size: 30.5 MB (30518493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37935977f73cdb1a6219601b542235e6d8e644936b8cf25366cfde43e1ffdb5`  
		Last Modified: Tue, 31 Mar 2020 13:04:08 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f328075e02d989b14a9b2b80c6c025a52291d2fc1f692ae3e8354924a392e4`  
		Last Modified: Tue, 31 Mar 2020 13:04:08 GMT  
		Size: 2.2 MB (2224877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298cb17784c1da449adb5c22b3f5e4da7284e660bfa447905d3264595bb1b89f`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 6.7 MB (6743105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fc4775083d830cf8f5101c142affec2c507fe362d52b28df774d20f2be322a`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5b79331cc66cc391aaeac509af5f09930e6ac200f10334870ddc8bb00e6dde`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:84492a658080293507f780e30491b19f59999451ca2d9425cc7d5a74dd40dbd4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33473205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b891634784f97556b880a94bd3454bfdb17662e0d3b99672ff1c8912b6eb6ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:09:01 GMT
ADD file:012f7224d56eafd61d4fbf99bc0a12ce4afa4a228fb04a849a9e9398ae8e0969 in / 
# Tue, 31 Mar 2020 01:09:02 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:09:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 05:09:09 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:46:10 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b59fc323cb12d31b5e0b5e812b5ca8436f3753a6e6cc9004edbac36ffa7be8e0`  
		Last Modified: Tue, 31 Mar 2020 01:12:39 GMT  
		Size: 25.7 MB (25706014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e90b7c17de6092271c5f2c7d25a486f43a721eade119c158e196f86e227a029`  
		Last Modified: Tue, 31 Mar 2020 05:09:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888ad2b98a72be689e3df8c4c6f48f20eca3db61f4cb1b64ee4cb087776af495`  
		Last Modified: Tue, 31 Mar 2020 05:09:46 GMT  
		Size: 1.8 MB (1821695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207f73f920ef68dfce3700a684ba3bdfd3777f0ff29fb6cb9cfa686653898cbc`  
		Last Modified: Mon, 06 Apr 2020 19:46:40 GMT  
		Size: 5.9 MB (5943283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184a104b64648c41946a15ebafd1d7a3dd82b87a2656bd345e3e39e1d25c3572`  
		Last Modified: Mon, 06 Apr 2020 19:46:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7170c7834aa4e04f288d90ce4e40063c79e8a0b0f5d0bef87b0008b68e389a7`  
		Last Modified: Mon, 06 Apr 2020 19:46:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:836fc9b2c3d9321be72ed598f0c6d1261cb3d90393d6f00bf85d4c36ab09178c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:be1e1273f203254dbe788f80482ad7eb3dda4a61446fa4d8fe046d8d6b342ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de3a9d7ad126b00ea958b4f0240d31d91c8a8582af4ddac8570e1935de03c70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 17:53:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 17:54:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:12:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 21:12:54 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:12:55 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:12:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:12:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:12:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af711a0248b008edeb7fc3ec89d9b65d0e6bc9a7812f17e7c0e1981713091b0`  
		Last Modified: Tue, 31 Mar 2020 17:54:57 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf07c97371206072919de7231d4a5b645fc9214d9477f21dff3c4bcf2d836ca`  
		Last Modified: Tue, 31 Mar 2020 17:54:57 GMT  
		Size: 2.1 MB (2128010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf676d0d98d691716d2c2ac3f58d9300f97af52c37052d44f1991d468c20da`  
		Last Modified: Mon, 06 Apr 2020 21:13:51 GMT  
		Size: 7.0 MB (7037456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772658cc02099a47df92d23a2dc7b78ff48f02f3c5eae197d45e5595ca79dae3`  
		Last Modified: Mon, 06 Apr 2020 21:13:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9fba6c68631c186e227ec9fc3a8bec328a5ea49571cbd3718c6872dfa9474`  
		Last Modified: Mon, 06 Apr 2020 21:13:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:f1512fe235b70e455d37fddc35e243dff2ecf609dce90da107a166c6c540c525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32151424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c7ad750a45d0754af70700f3d5e90ef6f33eccae12c2028f74c6a55296138a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:54 GMT
ADD file:e08ed9e60228d351de400af5746474777a562d99f17e0cb1ce3e3d352e9ec751 in / 
# Tue, 31 Mar 2020 01:24:56 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 04:13:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 04:14:07 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:48:31 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:48:32 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:48:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:49:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:49:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:49:30 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:49:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:49:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:49:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:440df189aa3df85587f2d7d348500930481b3752dcb887d212de9b44b49076dd`  
		Last Modified: Tue, 31 Mar 2020 01:33:04 GMT  
		Size: 24.8 MB (24830324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3031ff195bb3799ebe4254f93022cc97bda6966cf5340f247941ae0a236bc8`  
		Last Modified: Tue, 31 Mar 2020 04:15:31 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e9b06f7ebf1fc3799d2a0fa1664e11b861e3055c54dcfd0283a0aef5350a0b`  
		Last Modified: Tue, 31 Mar 2020 04:15:32 GMT  
		Size: 1.8 MB (1839102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba06c78ab671b13c2cfd74f9c9cf70c5fae20022228334b4a980c1027c61b482`  
		Last Modified: Mon, 06 Apr 2020 19:49:55 GMT  
		Size: 5.5 MB (5479794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf7920a9f6fa89d2c56f50bd15154b9fafd77611107ba7e49820bf8bc72e407`  
		Last Modified: Mon, 06 Apr 2020 19:49:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d244a050acaaad3567ce421740a244acb6e028829c1cca06d9a1012d5c50eb`  
		Last Modified: Mon, 06 Apr 2020 19:49:52 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:eeac0857b6e2761fcb93405df2e77ec321bb99be3c1c74373781393b2ee92003
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29746810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ad38fadc7fdd89befc82a3c614c010ea03aacb9450975cb60cf90f9b0535a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:48:12 GMT
ADD file:8c3ed0df404a6bcaf7583e71796cb4c1f40e87288953a21d4ee5946079c3274f in / 
# Tue, 31 Mar 2020 01:48:13 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 08:18:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 08:19:21 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:58:19 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:58:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:58:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:59:07 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:08 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98098fa10651fdba12c848231b7428536a120e17637f1f9e0d25c63880483fcc`  
		Last Modified: Tue, 31 Mar 2020 01:56:24 GMT  
		Size: 22.7 MB (22699731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7922ddf1b86ac7ad159d24a62da9689447caf7b4c69ce081a02a73d055bff`  
		Last Modified: Tue, 31 Mar 2020 08:21:20 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754834d90b58f45e25a8bfa558985a0ced452414dde7e9d70e222afd86be2fa8`  
		Last Modified: Tue, 31 Mar 2020 08:21:20 GMT  
		Size: 1.8 MB (1759473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272af2fbbb3f2aed36f1844fb765e9759fdf25d0772754b0513fe9ddecc40b9d`  
		Last Modified: Mon, 06 Apr 2020 20:00:06 GMT  
		Size: 5.3 MB (5285397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daae49ef671f0947b4b1cab63d653ad548252e336511375fe7140efe4905f0e`  
		Last Modified: Mon, 06 Apr 2020 20:00:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63e1cc9b947e96c2587111ad56ab86d54be60134ccd9a807f0389c15ea3f61b`  
		Last Modified: Mon, 06 Apr 2020 20:00:04 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:78c250c7e5d01ce41983b2753680ba9b101af8c543f5c397b55ae10814cc22c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33766998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472dc2c5d0c415f63d802bf98ff0a6bd86cf5d0ccff488506dea4be4217c9ab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:32:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 20:32:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:52:02 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:52:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:52:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:52:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:52:52 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:52:53 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:52:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:52:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744144498f3e2946eaba16e1fc06cc2a6ed34447976d59e141a9f9156aa19624`  
		Last Modified: Tue, 31 Mar 2020 20:34:01 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c968861bade4527ff71063fced63ca4143f9886781be1af7a07993354297a112`  
		Last Modified: Tue, 31 Mar 2020 20:34:00 GMT  
		Size: 2.0 MB (2007812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf54b87406d4a55b55235b7c10eb81445f9e40f99ebbbc8eb130efa13646e25`  
		Last Modified: Mon, 06 Apr 2020 19:54:08 GMT  
		Size: 5.9 MB (5905328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3f664cad2767e1664990b44fa7e4d9e8c3388dbaf2e3bc0e651ae046f9656a`  
		Last Modified: Mon, 06 Apr 2020 19:53:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb3daa1131a9b59530b0c0153041fb324468bceadf2c9d1711ceb1ab935a3ff`  
		Last Modified: Mon, 06 Apr 2020 19:53:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:976ddfd647eff5d898a8247eebd96683505517ad3e705c1ca73a8c092504d336
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41515262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1cbef7c8e6271e24f80c06efcf46d494fb5b3575c7c33bc96e6a7e2ef120b2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 13:19:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 13:19:17 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:43:17 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:18 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1033102c2fb2ed5037246c60787ba3376aaf2e983140ea88b05d2fe1dcca139`  
		Last Modified: Tue, 31 Mar 2020 13:20:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a518aadc532142e2d36b269c309d07235a326660c35df16af78cf09726dc67dc`  
		Last Modified: Tue, 31 Mar 2020 13:20:04 GMT  
		Size: 2.1 MB (2132319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f408e0d5cb38c8d8bf6c2e778d473aa0a5b82f3c69420ff18840c2fe70390c4a`  
		Last Modified: Mon, 06 Apr 2020 19:44:01 GMT  
		Size: 11.6 MB (11633125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95a05714cd0087efcd7817104cf284e0a88823599b290eaf117bd64e6960c64`  
		Last Modified: Mon, 06 Apr 2020 19:43:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e6b7e5bc2f22c3c986e055952e8670bb45920a95990f5b4ab02eaa009baca6`  
		Last Modified: Mon, 06 Apr 2020 19:43:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:d3ba4984825c204c3dc09c4fa4cc5cffcdd761eed19e785d78dbbf577ef3510e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0562eea684e4b3839767d99691be0187e1f3b1bd1e3a717e660857408763f538`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:42 GMT
ADD file:36c02e92574faba45b64cfed78a0a0359d65ad175b17128bf554a2a5c0086ff5 in / 
# Tue, 31 Mar 2020 01:32:47 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 12:58:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 12:59:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 20:23:17 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:23:21 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:23:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 20:25:50 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:25:53 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:25:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:25:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:26:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9df6bbae5eeb29e9aac2f39cff517c694cce60f01ee477abcdedcd8e8c01c38f`  
		Last Modified: Tue, 31 Mar 2020 01:45:59 GMT  
		Size: 30.5 MB (30518493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37935977f73cdb1a6219601b542235e6d8e644936b8cf25366cfde43e1ffdb5`  
		Last Modified: Tue, 31 Mar 2020 13:04:08 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f328075e02d989b14a9b2b80c6c025a52291d2fc1f692ae3e8354924a392e4`  
		Last Modified: Tue, 31 Mar 2020 13:04:08 GMT  
		Size: 2.2 MB (2224877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298cb17784c1da449adb5c22b3f5e4da7284e660bfa447905d3264595bb1b89f`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 6.7 MB (6743105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fc4775083d830cf8f5101c142affec2c507fe362d52b28df774d20f2be322a`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5b79331cc66cc391aaeac509af5f09930e6ac200f10334870ddc8bb00e6dde`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:84492a658080293507f780e30491b19f59999451ca2d9425cc7d5a74dd40dbd4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33473205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b891634784f97556b880a94bd3454bfdb17662e0d3b99672ff1c8912b6eb6ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:09:01 GMT
ADD file:012f7224d56eafd61d4fbf99bc0a12ce4afa4a228fb04a849a9e9398ae8e0969 in / 
# Tue, 31 Mar 2020 01:09:02 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:09:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 05:09:09 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:46:10 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b59fc323cb12d31b5e0b5e812b5ca8436f3753a6e6cc9004edbac36ffa7be8e0`  
		Last Modified: Tue, 31 Mar 2020 01:12:39 GMT  
		Size: 25.7 MB (25706014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e90b7c17de6092271c5f2c7d25a486f43a721eade119c158e196f86e227a029`  
		Last Modified: Tue, 31 Mar 2020 05:09:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888ad2b98a72be689e3df8c4c6f48f20eca3db61f4cb1b64ee4cb087776af495`  
		Last Modified: Tue, 31 Mar 2020 05:09:46 GMT  
		Size: 1.8 MB (1821695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207f73f920ef68dfce3700a684ba3bdfd3777f0ff29fb6cb9cfa686653898cbc`  
		Last Modified: Mon, 06 Apr 2020 19:46:40 GMT  
		Size: 5.9 MB (5943283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184a104b64648c41946a15ebafd1d7a3dd82b87a2656bd345e3e39e1d25c3572`  
		Last Modified: Mon, 06 Apr 2020 19:46:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7170c7834aa4e04f288d90ce4e40063c79e8a0b0f5d0bef87b0008b68e389a7`  
		Last Modified: Mon, 06 Apr 2020 19:46:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:836fc9b2c3d9321be72ed598f0c6d1261cb3d90393d6f00bf85d4c36ab09178c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.1` - linux; amd64

```console
$ docker pull spiped@sha256:be1e1273f203254dbe788f80482ad7eb3dda4a61446fa4d8fe046d8d6b342ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de3a9d7ad126b00ea958b4f0240d31d91c8a8582af4ddac8570e1935de03c70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 17:53:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 17:54:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:12:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 21:12:54 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:12:55 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:12:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:12:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:12:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af711a0248b008edeb7fc3ec89d9b65d0e6bc9a7812f17e7c0e1981713091b0`  
		Last Modified: Tue, 31 Mar 2020 17:54:57 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf07c97371206072919de7231d4a5b645fc9214d9477f21dff3c4bcf2d836ca`  
		Last Modified: Tue, 31 Mar 2020 17:54:57 GMT  
		Size: 2.1 MB (2128010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf676d0d98d691716d2c2ac3f58d9300f97af52c37052d44f1991d468c20da`  
		Last Modified: Mon, 06 Apr 2020 21:13:51 GMT  
		Size: 7.0 MB (7037456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772658cc02099a47df92d23a2dc7b78ff48f02f3c5eae197d45e5595ca79dae3`  
		Last Modified: Mon, 06 Apr 2020 21:13:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9fba6c68631c186e227ec9fc3a8bec328a5ea49571cbd3718c6872dfa9474`  
		Last Modified: Mon, 06 Apr 2020 21:13:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:f1512fe235b70e455d37fddc35e243dff2ecf609dce90da107a166c6c540c525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32151424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c7ad750a45d0754af70700f3d5e90ef6f33eccae12c2028f74c6a55296138a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:54 GMT
ADD file:e08ed9e60228d351de400af5746474777a562d99f17e0cb1ce3e3d352e9ec751 in / 
# Tue, 31 Mar 2020 01:24:56 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 04:13:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 04:14:07 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:48:31 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:48:32 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:48:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:49:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:49:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:49:30 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:49:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:49:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:49:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:440df189aa3df85587f2d7d348500930481b3752dcb887d212de9b44b49076dd`  
		Last Modified: Tue, 31 Mar 2020 01:33:04 GMT  
		Size: 24.8 MB (24830324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3031ff195bb3799ebe4254f93022cc97bda6966cf5340f247941ae0a236bc8`  
		Last Modified: Tue, 31 Mar 2020 04:15:31 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e9b06f7ebf1fc3799d2a0fa1664e11b861e3055c54dcfd0283a0aef5350a0b`  
		Last Modified: Tue, 31 Mar 2020 04:15:32 GMT  
		Size: 1.8 MB (1839102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba06c78ab671b13c2cfd74f9c9cf70c5fae20022228334b4a980c1027c61b482`  
		Last Modified: Mon, 06 Apr 2020 19:49:55 GMT  
		Size: 5.5 MB (5479794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf7920a9f6fa89d2c56f50bd15154b9fafd77611107ba7e49820bf8bc72e407`  
		Last Modified: Mon, 06 Apr 2020 19:49:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d244a050acaaad3567ce421740a244acb6e028829c1cca06d9a1012d5c50eb`  
		Last Modified: Mon, 06 Apr 2020 19:49:52 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:eeac0857b6e2761fcb93405df2e77ec321bb99be3c1c74373781393b2ee92003
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29746810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ad38fadc7fdd89befc82a3c614c010ea03aacb9450975cb60cf90f9b0535a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:48:12 GMT
ADD file:8c3ed0df404a6bcaf7583e71796cb4c1f40e87288953a21d4ee5946079c3274f in / 
# Tue, 31 Mar 2020 01:48:13 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 08:18:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 08:19:21 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:58:19 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:58:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:58:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:59:07 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:08 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98098fa10651fdba12c848231b7428536a120e17637f1f9e0d25c63880483fcc`  
		Last Modified: Tue, 31 Mar 2020 01:56:24 GMT  
		Size: 22.7 MB (22699731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7922ddf1b86ac7ad159d24a62da9689447caf7b4c69ce081a02a73d055bff`  
		Last Modified: Tue, 31 Mar 2020 08:21:20 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754834d90b58f45e25a8bfa558985a0ced452414dde7e9d70e222afd86be2fa8`  
		Last Modified: Tue, 31 Mar 2020 08:21:20 GMT  
		Size: 1.8 MB (1759473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272af2fbbb3f2aed36f1844fb765e9759fdf25d0772754b0513fe9ddecc40b9d`  
		Last Modified: Mon, 06 Apr 2020 20:00:06 GMT  
		Size: 5.3 MB (5285397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daae49ef671f0947b4b1cab63d653ad548252e336511375fe7140efe4905f0e`  
		Last Modified: Mon, 06 Apr 2020 20:00:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63e1cc9b947e96c2587111ad56ab86d54be60134ccd9a807f0389c15ea3f61b`  
		Last Modified: Mon, 06 Apr 2020 20:00:04 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:78c250c7e5d01ce41983b2753680ba9b101af8c543f5c397b55ae10814cc22c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33766998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472dc2c5d0c415f63d802bf98ff0a6bd86cf5d0ccff488506dea4be4217c9ab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:32:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 20:32:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:52:02 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:52:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:52:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:52:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:52:52 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:52:53 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:52:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:52:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744144498f3e2946eaba16e1fc06cc2a6ed34447976d59e141a9f9156aa19624`  
		Last Modified: Tue, 31 Mar 2020 20:34:01 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c968861bade4527ff71063fced63ca4143f9886781be1af7a07993354297a112`  
		Last Modified: Tue, 31 Mar 2020 20:34:00 GMT  
		Size: 2.0 MB (2007812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf54b87406d4a55b55235b7c10eb81445f9e40f99ebbbc8eb130efa13646e25`  
		Last Modified: Mon, 06 Apr 2020 19:54:08 GMT  
		Size: 5.9 MB (5905328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3f664cad2767e1664990b44fa7e4d9e8c3388dbaf2e3bc0e651ae046f9656a`  
		Last Modified: Mon, 06 Apr 2020 19:53:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb3daa1131a9b59530b0c0153041fb324468bceadf2c9d1711ceb1ab935a3ff`  
		Last Modified: Mon, 06 Apr 2020 19:53:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:976ddfd647eff5d898a8247eebd96683505517ad3e705c1ca73a8c092504d336
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41515262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1cbef7c8e6271e24f80c06efcf46d494fb5b3575c7c33bc96e6a7e2ef120b2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 13:19:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 13:19:17 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:43:17 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:18 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1033102c2fb2ed5037246c60787ba3376aaf2e983140ea88b05d2fe1dcca139`  
		Last Modified: Tue, 31 Mar 2020 13:20:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a518aadc532142e2d36b269c309d07235a326660c35df16af78cf09726dc67dc`  
		Last Modified: Tue, 31 Mar 2020 13:20:04 GMT  
		Size: 2.1 MB (2132319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f408e0d5cb38c8d8bf6c2e778d473aa0a5b82f3c69420ff18840c2fe70390c4a`  
		Last Modified: Mon, 06 Apr 2020 19:44:01 GMT  
		Size: 11.6 MB (11633125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95a05714cd0087efcd7817104cf284e0a88823599b290eaf117bd64e6960c64`  
		Last Modified: Mon, 06 Apr 2020 19:43:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e6b7e5bc2f22c3c986e055952e8670bb45920a95990f5b4ab02eaa009baca6`  
		Last Modified: Mon, 06 Apr 2020 19:43:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:d3ba4984825c204c3dc09c4fa4cc5cffcdd761eed19e785d78dbbf577ef3510e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0562eea684e4b3839767d99691be0187e1f3b1bd1e3a717e660857408763f538`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:42 GMT
ADD file:36c02e92574faba45b64cfed78a0a0359d65ad175b17128bf554a2a5c0086ff5 in / 
# Tue, 31 Mar 2020 01:32:47 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 12:58:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 12:59:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 20:23:17 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:23:21 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:23:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 20:25:50 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:25:53 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:25:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:25:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:26:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9df6bbae5eeb29e9aac2f39cff517c694cce60f01ee477abcdedcd8e8c01c38f`  
		Last Modified: Tue, 31 Mar 2020 01:45:59 GMT  
		Size: 30.5 MB (30518493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37935977f73cdb1a6219601b542235e6d8e644936b8cf25366cfde43e1ffdb5`  
		Last Modified: Tue, 31 Mar 2020 13:04:08 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f328075e02d989b14a9b2b80c6c025a52291d2fc1f692ae3e8354924a392e4`  
		Last Modified: Tue, 31 Mar 2020 13:04:08 GMT  
		Size: 2.2 MB (2224877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298cb17784c1da449adb5c22b3f5e4da7284e660bfa447905d3264595bb1b89f`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 6.7 MB (6743105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fc4775083d830cf8f5101c142affec2c507fe362d52b28df774d20f2be322a`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5b79331cc66cc391aaeac509af5f09930e6ac200f10334870ddc8bb00e6dde`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:84492a658080293507f780e30491b19f59999451ca2d9425cc7d5a74dd40dbd4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33473205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b891634784f97556b880a94bd3454bfdb17662e0d3b99672ff1c8912b6eb6ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:09:01 GMT
ADD file:012f7224d56eafd61d4fbf99bc0a12ce4afa4a228fb04a849a9e9398ae8e0969 in / 
# Tue, 31 Mar 2020 01:09:02 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:09:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 05:09:09 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:46:10 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b59fc323cb12d31b5e0b5e812b5ca8436f3753a6e6cc9004edbac36ffa7be8e0`  
		Last Modified: Tue, 31 Mar 2020 01:12:39 GMT  
		Size: 25.7 MB (25706014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e90b7c17de6092271c5f2c7d25a486f43a721eade119c158e196f86e227a029`  
		Last Modified: Tue, 31 Mar 2020 05:09:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888ad2b98a72be689e3df8c4c6f48f20eca3db61f4cb1b64ee4cb087776af495`  
		Last Modified: Tue, 31 Mar 2020 05:09:46 GMT  
		Size: 1.8 MB (1821695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207f73f920ef68dfce3700a684ba3bdfd3777f0ff29fb6cb9cfa686653898cbc`  
		Last Modified: Mon, 06 Apr 2020 19:46:40 GMT  
		Size: 5.9 MB (5943283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184a104b64648c41946a15ebafd1d7a3dd82b87a2656bd345e3e39e1d25c3572`  
		Last Modified: Mon, 06 Apr 2020 19:46:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7170c7834aa4e04f288d90ce4e40063c79e8a0b0f5d0bef87b0008b68e389a7`  
		Last Modified: Mon, 06 Apr 2020 19:46:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:429322e56bd429da567aab90232ba7941a4edb8e64c2c09b9373402f91a44d4d
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
$ docker pull spiped@sha256:bce46785c0a6ec6e48a45f297dd5796fe2e5d9fafb6a3cf034c6971e7ff2780f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2883892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b78eb499d78cb9b4325629fbc90c2735a1cf1c1bd4af69bd8ef608587d02cb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 21:13:07 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:13:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 21:13:34 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:13:34 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:13:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:13:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:13:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc29e947b9ccbbe548f4f1f66f2a845c61ab555b046909b89e4fd420a3e93f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 88.9 KB (88915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb514126aa1d85c9fc37f7d50649132790a408d0ddd0cd279c2a832ade0b08df`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90b1f71237aa2be63e283a61cdc07fc8342b12601060003bfa959a95253b0f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:6f13ddc4cb1716a895e69405631a68d99c7addad9078453402ad5938856a0687
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0bd97d067a154cda46a3674de70626059520bfaf9d8f8b3fc4557df053d73ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:49:34 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:49:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:49:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:50:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:50:08 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:50:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:50:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:50:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:50:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7a9eb0c9ab5fc279a9e98ef9e98de63123b64ca04af635a1f73af9a6d15b24`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 75.0 KB (74952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9967718642289f730242b2a77c0515672aec66c1a838dd2a4f80d444ee79b8`  
		Last Modified: Mon, 06 Apr 2020 19:50:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f4a4b862c429a85eeacb3270f4cc64c2c61e9357769a9c151d183ff8ca31a9`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d6d6923d0c2d9d8e954815efdf9c9669fa23bd9548d55ead413e69dfe7d52d7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa542a4d5cbae70b3e71e20948df53d2d5b7c0002792bacd5bbf792a6f52f6e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:59:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:59:49 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d441b71208c64b2bc2218499780ec39d9cfd3edbdd8e2e4d7c45a80f6d84bc5f`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 68.1 KB (68096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd2cbe47130d1b62eefe8efad8296a2e4160621db07811a387f646ec3c0589`  
		Last Modified: Mon, 06 Apr 2020 20:00:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d62488071b8b3ca44afce89ea5c8de19fdf6db9cc18bceda022deb8bfc6f79`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:33dd11964e68275c0de9bdd90576f1bd3b07ed9b35be0d3cdd3ca1f750a618c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2807814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371dcc8679ed28f64596dd03ffcbc8756f215a13eabd2677793a1cd1f4ff6ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:53:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:53:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:53:38 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:53:38 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:53:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:53:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:53:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b182ea73fc29e32821dfc68455a6582b2b46be25a46a61c72df2fc9787013`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 82.0 KB (81989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a5ef743131210844f90d7217bb848a2baa687b4c7831815cebb46a94ea8b`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01cf4b79b4817343f95634a3b4cdd1066462a5435b81c0147d585090b50051e`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:2f99e8ca94d16bef32ae67a69bf093ea7df131d656e0d5bf94d217755375eef3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc64ad00fc662dc2350d81e426695cc56dc2ee3fb92c25e9573a5e41edb6207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:43:44 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:45 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c23f29e92934601486929bc683a1c1ce6b5d17de8710ffb64ae444a6edf74bd`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 98.4 KB (98396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11754050cbbe0e5f1e3f040f12eb326523d160784b4bf4053eb29c607abb6106`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802418066b370d7b8c1b666fbd6ba2090c2f354f5a84ee7b3771c1d5181fa148`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:51027e899bfe55d1432c89de3d9b71bac3fbcc342373f1111aa03217c0d11b67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1d379d08a7d62d83cb2d138d3d260429659fe214c06248975f439fe8837fea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 20:26:12 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:26:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:26:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 20:26:46 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:26:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:26:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:26:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68e315a19f730564cead7324b439d4c893d7bb4661c6aa88a863dff413222be`  
		Last Modified: Mon, 06 Apr 2020 20:27:35 GMT  
		Size: 97.5 KB (97516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1fcb0a480d90f3ae48043a675f479aab1cc1f315674ce71db46b2b5ddea7e2`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad7ed01644a076eb4f0e4ee3ff1981a0383df44638b5cb6a1e811ac29b7affa`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9d875e8421a60f09bc74f0103800a7e000690cd17d9eac43042cdbb8308cf8a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2662697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbcb97371eba97b63ff9fbf44afe6eeaa0cdbc6bc9be9fe8494fcaa4e254d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:46:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:29 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66314c6e3c0080fcb0f7264c3aaa35fe5fd5d1bab9428aa378638125af56c3c`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 81.0 KB (81006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f3a2df50f521de78c8d5d6df53bf6bbc15080b09c18d64eb7cef65f3f516ba`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a08476e03d2df5c637df812d7ebb17ed6fc5dee82ea4da393a867a6c394db`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:429322e56bd429da567aab90232ba7941a4edb8e64c2c09b9373402f91a44d4d
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
$ docker pull spiped@sha256:bce46785c0a6ec6e48a45f297dd5796fe2e5d9fafb6a3cf034c6971e7ff2780f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2883892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b78eb499d78cb9b4325629fbc90c2735a1cf1c1bd4af69bd8ef608587d02cb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 21:13:07 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:13:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 21:13:34 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:13:34 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:13:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:13:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:13:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc29e947b9ccbbe548f4f1f66f2a845c61ab555b046909b89e4fd420a3e93f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 88.9 KB (88915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb514126aa1d85c9fc37f7d50649132790a408d0ddd0cd279c2a832ade0b08df`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90b1f71237aa2be63e283a61cdc07fc8342b12601060003bfa959a95253b0f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:6f13ddc4cb1716a895e69405631a68d99c7addad9078453402ad5938856a0687
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0bd97d067a154cda46a3674de70626059520bfaf9d8f8b3fc4557df053d73ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:49:34 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:49:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:49:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:50:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:50:08 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:50:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:50:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:50:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:50:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7a9eb0c9ab5fc279a9e98ef9e98de63123b64ca04af635a1f73af9a6d15b24`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 75.0 KB (74952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9967718642289f730242b2a77c0515672aec66c1a838dd2a4f80d444ee79b8`  
		Last Modified: Mon, 06 Apr 2020 19:50:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f4a4b862c429a85eeacb3270f4cc64c2c61e9357769a9c151d183ff8ca31a9`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d6d6923d0c2d9d8e954815efdf9c9669fa23bd9548d55ead413e69dfe7d52d7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa542a4d5cbae70b3e71e20948df53d2d5b7c0002792bacd5bbf792a6f52f6e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:59:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:59:49 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d441b71208c64b2bc2218499780ec39d9cfd3edbdd8e2e4d7c45a80f6d84bc5f`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 68.1 KB (68096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd2cbe47130d1b62eefe8efad8296a2e4160621db07811a387f646ec3c0589`  
		Last Modified: Mon, 06 Apr 2020 20:00:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d62488071b8b3ca44afce89ea5c8de19fdf6db9cc18bceda022deb8bfc6f79`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:33dd11964e68275c0de9bdd90576f1bd3b07ed9b35be0d3cdd3ca1f750a618c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2807814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371dcc8679ed28f64596dd03ffcbc8756f215a13eabd2677793a1cd1f4ff6ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:53:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:53:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:53:38 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:53:38 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:53:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:53:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:53:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b182ea73fc29e32821dfc68455a6582b2b46be25a46a61c72df2fc9787013`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 82.0 KB (81989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a5ef743131210844f90d7217bb848a2baa687b4c7831815cebb46a94ea8b`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01cf4b79b4817343f95634a3b4cdd1066462a5435b81c0147d585090b50051e`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:2f99e8ca94d16bef32ae67a69bf093ea7df131d656e0d5bf94d217755375eef3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc64ad00fc662dc2350d81e426695cc56dc2ee3fb92c25e9573a5e41edb6207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:43:44 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:45 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c23f29e92934601486929bc683a1c1ce6b5d17de8710ffb64ae444a6edf74bd`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 98.4 KB (98396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11754050cbbe0e5f1e3f040f12eb326523d160784b4bf4053eb29c607abb6106`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802418066b370d7b8c1b666fbd6ba2090c2f354f5a84ee7b3771c1d5181fa148`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:51027e899bfe55d1432c89de3d9b71bac3fbcc342373f1111aa03217c0d11b67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1d379d08a7d62d83cb2d138d3d260429659fe214c06248975f439fe8837fea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 20:26:12 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:26:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:26:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 20:26:46 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:26:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:26:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:26:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68e315a19f730564cead7324b439d4c893d7bb4661c6aa88a863dff413222be`  
		Last Modified: Mon, 06 Apr 2020 20:27:35 GMT  
		Size: 97.5 KB (97516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1fcb0a480d90f3ae48043a675f479aab1cc1f315674ce71db46b2b5ddea7e2`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad7ed01644a076eb4f0e4ee3ff1981a0383df44638b5cb6a1e811ac29b7affa`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9d875e8421a60f09bc74f0103800a7e000690cd17d9eac43042cdbb8308cf8a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2662697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbcb97371eba97b63ff9fbf44afe6eeaa0cdbc6bc9be9fe8494fcaa4e254d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:46:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:29 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66314c6e3c0080fcb0f7264c3aaa35fe5fd5d1bab9428aa378638125af56c3c`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 81.0 KB (81006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f3a2df50f521de78c8d5d6df53bf6bbc15080b09c18d64eb7cef65f3f516ba`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a08476e03d2df5c637df812d7ebb17ed6fc5dee82ea4da393a867a6c394db`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:429322e56bd429da567aab90232ba7941a4edb8e64c2c09b9373402f91a44d4d
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
$ docker pull spiped@sha256:bce46785c0a6ec6e48a45f297dd5796fe2e5d9fafb6a3cf034c6971e7ff2780f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2883892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b78eb499d78cb9b4325629fbc90c2735a1cf1c1bd4af69bd8ef608587d02cb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 21:13:07 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:13:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 21:13:34 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:13:34 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:13:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:13:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:13:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc29e947b9ccbbe548f4f1f66f2a845c61ab555b046909b89e4fd420a3e93f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 88.9 KB (88915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb514126aa1d85c9fc37f7d50649132790a408d0ddd0cd279c2a832ade0b08df`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90b1f71237aa2be63e283a61cdc07fc8342b12601060003bfa959a95253b0f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:6f13ddc4cb1716a895e69405631a68d99c7addad9078453402ad5938856a0687
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0bd97d067a154cda46a3674de70626059520bfaf9d8f8b3fc4557df053d73ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:49:34 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:49:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:49:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:50:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:50:08 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:50:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:50:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:50:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:50:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7a9eb0c9ab5fc279a9e98ef9e98de63123b64ca04af635a1f73af9a6d15b24`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 75.0 KB (74952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9967718642289f730242b2a77c0515672aec66c1a838dd2a4f80d444ee79b8`  
		Last Modified: Mon, 06 Apr 2020 19:50:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f4a4b862c429a85eeacb3270f4cc64c2c61e9357769a9c151d183ff8ca31a9`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d6d6923d0c2d9d8e954815efdf9c9669fa23bd9548d55ead413e69dfe7d52d7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa542a4d5cbae70b3e71e20948df53d2d5b7c0002792bacd5bbf792a6f52f6e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:59:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:59:49 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d441b71208c64b2bc2218499780ec39d9cfd3edbdd8e2e4d7c45a80f6d84bc5f`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 68.1 KB (68096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd2cbe47130d1b62eefe8efad8296a2e4160621db07811a387f646ec3c0589`  
		Last Modified: Mon, 06 Apr 2020 20:00:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d62488071b8b3ca44afce89ea5c8de19fdf6db9cc18bceda022deb8bfc6f79`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:33dd11964e68275c0de9bdd90576f1bd3b07ed9b35be0d3cdd3ca1f750a618c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2807814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371dcc8679ed28f64596dd03ffcbc8756f215a13eabd2677793a1cd1f4ff6ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:53:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:53:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:53:38 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:53:38 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:53:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:53:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:53:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b182ea73fc29e32821dfc68455a6582b2b46be25a46a61c72df2fc9787013`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 82.0 KB (81989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a5ef743131210844f90d7217bb848a2baa687b4c7831815cebb46a94ea8b`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01cf4b79b4817343f95634a3b4cdd1066462a5435b81c0147d585090b50051e`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:2f99e8ca94d16bef32ae67a69bf093ea7df131d656e0d5bf94d217755375eef3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc64ad00fc662dc2350d81e426695cc56dc2ee3fb92c25e9573a5e41edb6207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:43:44 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:45 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c23f29e92934601486929bc683a1c1ce6b5d17de8710ffb64ae444a6edf74bd`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 98.4 KB (98396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11754050cbbe0e5f1e3f040f12eb326523d160784b4bf4053eb29c607abb6106`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802418066b370d7b8c1b666fbd6ba2090c2f354f5a84ee7b3771c1d5181fa148`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:51027e899bfe55d1432c89de3d9b71bac3fbcc342373f1111aa03217c0d11b67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1d379d08a7d62d83cb2d138d3d260429659fe214c06248975f439fe8837fea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 20:26:12 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:26:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:26:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 20:26:46 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:26:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:26:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:26:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68e315a19f730564cead7324b439d4c893d7bb4661c6aa88a863dff413222be`  
		Last Modified: Mon, 06 Apr 2020 20:27:35 GMT  
		Size: 97.5 KB (97516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1fcb0a480d90f3ae48043a675f479aab1cc1f315674ce71db46b2b5ddea7e2`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad7ed01644a076eb4f0e4ee3ff1981a0383df44638b5cb6a1e811ac29b7affa`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9d875e8421a60f09bc74f0103800a7e000690cd17d9eac43042cdbb8308cf8a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2662697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbcb97371eba97b63ff9fbf44afe6eeaa0cdbc6bc9be9fe8494fcaa4e254d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:46:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:29 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66314c6e3c0080fcb0f7264c3aaa35fe5fd5d1bab9428aa378638125af56c3c`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 81.0 KB (81006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f3a2df50f521de78c8d5d6df53bf6bbc15080b09c18d64eb7cef65f3f516ba`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a08476e03d2df5c637df812d7ebb17ed6fc5dee82ea4da393a867a6c394db`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:429322e56bd429da567aab90232ba7941a4edb8e64c2c09b9373402f91a44d4d
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
$ docker pull spiped@sha256:bce46785c0a6ec6e48a45f297dd5796fe2e5d9fafb6a3cf034c6971e7ff2780f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2883892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b78eb499d78cb9b4325629fbc90c2735a1cf1c1bd4af69bd8ef608587d02cb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 21:13:07 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:13:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 21:13:34 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:13:34 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:13:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:13:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:13:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc29e947b9ccbbe548f4f1f66f2a845c61ab555b046909b89e4fd420a3e93f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 88.9 KB (88915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb514126aa1d85c9fc37f7d50649132790a408d0ddd0cd279c2a832ade0b08df`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90b1f71237aa2be63e283a61cdc07fc8342b12601060003bfa959a95253b0f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:6f13ddc4cb1716a895e69405631a68d99c7addad9078453402ad5938856a0687
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0bd97d067a154cda46a3674de70626059520bfaf9d8f8b3fc4557df053d73ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:49:34 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:49:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:49:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:50:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:50:08 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:50:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:50:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:50:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:50:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7a9eb0c9ab5fc279a9e98ef9e98de63123b64ca04af635a1f73af9a6d15b24`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 75.0 KB (74952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9967718642289f730242b2a77c0515672aec66c1a838dd2a4f80d444ee79b8`  
		Last Modified: Mon, 06 Apr 2020 19:50:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f4a4b862c429a85eeacb3270f4cc64c2c61e9357769a9c151d183ff8ca31a9`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d6d6923d0c2d9d8e954815efdf9c9669fa23bd9548d55ead413e69dfe7d52d7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa542a4d5cbae70b3e71e20948df53d2d5b7c0002792bacd5bbf792a6f52f6e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:59:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:59:49 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d441b71208c64b2bc2218499780ec39d9cfd3edbdd8e2e4d7c45a80f6d84bc5f`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 68.1 KB (68096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd2cbe47130d1b62eefe8efad8296a2e4160621db07811a387f646ec3c0589`  
		Last Modified: Mon, 06 Apr 2020 20:00:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d62488071b8b3ca44afce89ea5c8de19fdf6db9cc18bceda022deb8bfc6f79`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:33dd11964e68275c0de9bdd90576f1bd3b07ed9b35be0d3cdd3ca1f750a618c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2807814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371dcc8679ed28f64596dd03ffcbc8756f215a13eabd2677793a1cd1f4ff6ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:53:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:53:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:53:38 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:53:38 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:53:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:53:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:53:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b182ea73fc29e32821dfc68455a6582b2b46be25a46a61c72df2fc9787013`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 82.0 KB (81989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a5ef743131210844f90d7217bb848a2baa687b4c7831815cebb46a94ea8b`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01cf4b79b4817343f95634a3b4cdd1066462a5435b81c0147d585090b50051e`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:2f99e8ca94d16bef32ae67a69bf093ea7df131d656e0d5bf94d217755375eef3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc64ad00fc662dc2350d81e426695cc56dc2ee3fb92c25e9573a5e41edb6207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:43:44 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:45 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c23f29e92934601486929bc683a1c1ce6b5d17de8710ffb64ae444a6edf74bd`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 98.4 KB (98396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11754050cbbe0e5f1e3f040f12eb326523d160784b4bf4053eb29c607abb6106`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802418066b370d7b8c1b666fbd6ba2090c2f354f5a84ee7b3771c1d5181fa148`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:51027e899bfe55d1432c89de3d9b71bac3fbcc342373f1111aa03217c0d11b67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1d379d08a7d62d83cb2d138d3d260429659fe214c06248975f439fe8837fea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 20:26:12 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:26:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:26:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 20:26:46 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:26:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:26:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:26:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68e315a19f730564cead7324b439d4c893d7bb4661c6aa88a863dff413222be`  
		Last Modified: Mon, 06 Apr 2020 20:27:35 GMT  
		Size: 97.5 KB (97516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1fcb0a480d90f3ae48043a675f479aab1cc1f315674ce71db46b2b5ddea7e2`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad7ed01644a076eb4f0e4ee3ff1981a0383df44638b5cb6a1e811ac29b7affa`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9d875e8421a60f09bc74f0103800a7e000690cd17d9eac43042cdbb8308cf8a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2662697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbcb97371eba97b63ff9fbf44afe6eeaa0cdbc6bc9be9fe8494fcaa4e254d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:46:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:29 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66314c6e3c0080fcb0f7264c3aaa35fe5fd5d1bab9428aa378638125af56c3c`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 81.0 KB (81006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f3a2df50f521de78c8d5d6df53bf6bbc15080b09c18d64eb7cef65f3f516ba`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a08476e03d2df5c637df812d7ebb17ed6fc5dee82ea4da393a867a6c394db`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:836fc9b2c3d9321be72ed598f0c6d1261cb3d90393d6f00bf85d4c36ab09178c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:be1e1273f203254dbe788f80482ad7eb3dda4a61446fa4d8fe046d8d6b342ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de3a9d7ad126b00ea958b4f0240d31d91c8a8582af4ddac8570e1935de03c70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 17:53:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 17:54:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:12:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 21:12:54 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:12:55 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:12:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:12:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:12:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af711a0248b008edeb7fc3ec89d9b65d0e6bc9a7812f17e7c0e1981713091b0`  
		Last Modified: Tue, 31 Mar 2020 17:54:57 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf07c97371206072919de7231d4a5b645fc9214d9477f21dff3c4bcf2d836ca`  
		Last Modified: Tue, 31 Mar 2020 17:54:57 GMT  
		Size: 2.1 MB (2128010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf676d0d98d691716d2c2ac3f58d9300f97af52c37052d44f1991d468c20da`  
		Last Modified: Mon, 06 Apr 2020 21:13:51 GMT  
		Size: 7.0 MB (7037456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772658cc02099a47df92d23a2dc7b78ff48f02f3c5eae197d45e5595ca79dae3`  
		Last Modified: Mon, 06 Apr 2020 21:13:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9fba6c68631c186e227ec9fc3a8bec328a5ea49571cbd3718c6872dfa9474`  
		Last Modified: Mon, 06 Apr 2020 21:13:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:f1512fe235b70e455d37fddc35e243dff2ecf609dce90da107a166c6c540c525
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32151424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c7ad750a45d0754af70700f3d5e90ef6f33eccae12c2028f74c6a55296138a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:54 GMT
ADD file:e08ed9e60228d351de400af5746474777a562d99f17e0cb1ce3e3d352e9ec751 in / 
# Tue, 31 Mar 2020 01:24:56 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 04:13:57 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 04:14:07 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:48:31 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:48:32 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:48:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:49:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:49:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:49:30 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:49:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:49:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:49:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:440df189aa3df85587f2d7d348500930481b3752dcb887d212de9b44b49076dd`  
		Last Modified: Tue, 31 Mar 2020 01:33:04 GMT  
		Size: 24.8 MB (24830324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3031ff195bb3799ebe4254f93022cc97bda6966cf5340f247941ae0a236bc8`  
		Last Modified: Tue, 31 Mar 2020 04:15:31 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e9b06f7ebf1fc3799d2a0fa1664e11b861e3055c54dcfd0283a0aef5350a0b`  
		Last Modified: Tue, 31 Mar 2020 04:15:32 GMT  
		Size: 1.8 MB (1839102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba06c78ab671b13c2cfd74f9c9cf70c5fae20022228334b4a980c1027c61b482`  
		Last Modified: Mon, 06 Apr 2020 19:49:55 GMT  
		Size: 5.5 MB (5479794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf7920a9f6fa89d2c56f50bd15154b9fafd77611107ba7e49820bf8bc72e407`  
		Last Modified: Mon, 06 Apr 2020 19:49:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d244a050acaaad3567ce421740a244acb6e028829c1cca06d9a1012d5c50eb`  
		Last Modified: Mon, 06 Apr 2020 19:49:52 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:eeac0857b6e2761fcb93405df2e77ec321bb99be3c1c74373781393b2ee92003
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29746810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ad38fadc7fdd89befc82a3c614c010ea03aacb9450975cb60cf90f9b0535a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:48:12 GMT
ADD file:8c3ed0df404a6bcaf7583e71796cb4c1f40e87288953a21d4ee5946079c3274f in / 
# Tue, 31 Mar 2020 01:48:13 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 08:18:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 08:19:21 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:58:19 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:58:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:58:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:59:07 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:08 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98098fa10651fdba12c848231b7428536a120e17637f1f9e0d25c63880483fcc`  
		Last Modified: Tue, 31 Mar 2020 01:56:24 GMT  
		Size: 22.7 MB (22699731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7922ddf1b86ac7ad159d24a62da9689447caf7b4c69ce081a02a73d055bff`  
		Last Modified: Tue, 31 Mar 2020 08:21:20 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754834d90b58f45e25a8bfa558985a0ced452414dde7e9d70e222afd86be2fa8`  
		Last Modified: Tue, 31 Mar 2020 08:21:20 GMT  
		Size: 1.8 MB (1759473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272af2fbbb3f2aed36f1844fb765e9759fdf25d0772754b0513fe9ddecc40b9d`  
		Last Modified: Mon, 06 Apr 2020 20:00:06 GMT  
		Size: 5.3 MB (5285397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daae49ef671f0947b4b1cab63d653ad548252e336511375fe7140efe4905f0e`  
		Last Modified: Mon, 06 Apr 2020 20:00:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63e1cc9b947e96c2587111ad56ab86d54be60134ccd9a807f0389c15ea3f61b`  
		Last Modified: Mon, 06 Apr 2020 20:00:04 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:78c250c7e5d01ce41983b2753680ba9b101af8c543f5c397b55ae10814cc22c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33766998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472dc2c5d0c415f63d802bf98ff0a6bd86cf5d0ccff488506dea4be4217c9ab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:32:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 20:32:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:52:02 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:52:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:52:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:52:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:52:52 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:52:53 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:52:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:52:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744144498f3e2946eaba16e1fc06cc2a6ed34447976d59e141a9f9156aa19624`  
		Last Modified: Tue, 31 Mar 2020 20:34:01 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c968861bade4527ff71063fced63ca4143f9886781be1af7a07993354297a112`  
		Last Modified: Tue, 31 Mar 2020 20:34:00 GMT  
		Size: 2.0 MB (2007812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf54b87406d4a55b55235b7c10eb81445f9e40f99ebbbc8eb130efa13646e25`  
		Last Modified: Mon, 06 Apr 2020 19:54:08 GMT  
		Size: 5.9 MB (5905328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3f664cad2767e1664990b44fa7e4d9e8c3388dbaf2e3bc0e651ae046f9656a`  
		Last Modified: Mon, 06 Apr 2020 19:53:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb3daa1131a9b59530b0c0153041fb324468bceadf2c9d1711ceb1ab935a3ff`  
		Last Modified: Mon, 06 Apr 2020 19:53:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:976ddfd647eff5d898a8247eebd96683505517ad3e705c1ca73a8c092504d336
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41515262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1cbef7c8e6271e24f80c06efcf46d494fb5b3575c7c33bc96e6a7e2ef120b2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 13:19:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 13:19:17 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:42:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:43:17 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:18 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1033102c2fb2ed5037246c60787ba3376aaf2e983140ea88b05d2fe1dcca139`  
		Last Modified: Tue, 31 Mar 2020 13:20:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a518aadc532142e2d36b269c309d07235a326660c35df16af78cf09726dc67dc`  
		Last Modified: Tue, 31 Mar 2020 13:20:04 GMT  
		Size: 2.1 MB (2132319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f408e0d5cb38c8d8bf6c2e778d473aa0a5b82f3c69420ff18840c2fe70390c4a`  
		Last Modified: Mon, 06 Apr 2020 19:44:01 GMT  
		Size: 11.6 MB (11633125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95a05714cd0087efcd7817104cf284e0a88823599b290eaf117bd64e6960c64`  
		Last Modified: Mon, 06 Apr 2020 19:43:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e6b7e5bc2f22c3c986e055952e8670bb45920a95990f5b4ab02eaa009baca6`  
		Last Modified: Mon, 06 Apr 2020 19:43:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:d3ba4984825c204c3dc09c4fa4cc5cffcdd761eed19e785d78dbbf577ef3510e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0562eea684e4b3839767d99691be0187e1f3b1bd1e3a717e660857408763f538`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:42 GMT
ADD file:36c02e92574faba45b64cfed78a0a0359d65ad175b17128bf554a2a5c0086ff5 in / 
# Tue, 31 Mar 2020 01:32:47 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 12:58:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 12:59:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 20:23:17 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:23:21 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:23:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 20:25:50 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:25:53 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:25:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:25:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:26:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9df6bbae5eeb29e9aac2f39cff517c694cce60f01ee477abcdedcd8e8c01c38f`  
		Last Modified: Tue, 31 Mar 2020 01:45:59 GMT  
		Size: 30.5 MB (30518493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37935977f73cdb1a6219601b542235e6d8e644936b8cf25366cfde43e1ffdb5`  
		Last Modified: Tue, 31 Mar 2020 13:04:08 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f328075e02d989b14a9b2b80c6c025a52291d2fc1f692ae3e8354924a392e4`  
		Last Modified: Tue, 31 Mar 2020 13:04:08 GMT  
		Size: 2.2 MB (2224877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298cb17784c1da449adb5c22b3f5e4da7284e660bfa447905d3264595bb1b89f`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 6.7 MB (6743105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fc4775083d830cf8f5101c142affec2c507fe362d52b28df774d20f2be322a`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5b79331cc66cc391aaeac509af5f09930e6ac200f10334870ddc8bb00e6dde`  
		Last Modified: Mon, 06 Apr 2020 20:27:18 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:84492a658080293507f780e30491b19f59999451ca2d9425cc7d5a74dd40dbd4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33473205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b891634784f97556b880a94bd3454bfdb17662e0d3b99672ff1c8912b6eb6ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:09:01 GMT
ADD file:012f7224d56eafd61d4fbf99bc0a12ce4afa4a228fb04a849a9e9398ae8e0969 in / 
# Tue, 31 Mar 2020 01:09:02 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:09:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 05:09:09 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:45:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 19:46:10 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b59fc323cb12d31b5e0b5e812b5ca8436f3753a6e6cc9004edbac36ffa7be8e0`  
		Last Modified: Tue, 31 Mar 2020 01:12:39 GMT  
		Size: 25.7 MB (25706014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e90b7c17de6092271c5f2c7d25a486f43a721eade119c158e196f86e227a029`  
		Last Modified: Tue, 31 Mar 2020 05:09:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888ad2b98a72be689e3df8c4c6f48f20eca3db61f4cb1b64ee4cb087776af495`  
		Last Modified: Tue, 31 Mar 2020 05:09:46 GMT  
		Size: 1.8 MB (1821695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207f73f920ef68dfce3700a684ba3bdfd3777f0ff29fb6cb9cfa686653898cbc`  
		Last Modified: Mon, 06 Apr 2020 19:46:40 GMT  
		Size: 5.9 MB (5943283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184a104b64648c41946a15ebafd1d7a3dd82b87a2656bd345e3e39e1d25c3572`  
		Last Modified: Mon, 06 Apr 2020 19:46:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7170c7834aa4e04f288d90ce4e40063c79e8a0b0f5d0bef87b0008b68e389a7`  
		Last Modified: Mon, 06 Apr 2020 19:46:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
