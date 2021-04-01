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
$ docker pull spiped@sha256:e865ca3e11696608182fd9928bd1fccd05e41d2521333555263cd32613be37e0
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
$ docker pull spiped@sha256:2e60e33376ba7a52ac3c9855c4d38f70b07e8e808d57c787fa582d14262201d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36307454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d42346bd6448e0f9af0920ba7340f9b4afbaf464bc3fd87567ce7b7440d20c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 16:15:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 16:15:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:15:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 16:16:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 16:16:19 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 16:16:20 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 16:16:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 16:16:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 16:16:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc45f75826335ee1323a9be0a79ecfade544e9266d399a602046a4ebd747de`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e84fa40c6bd50fde8152aaee374243fa3995702540318ee50f0031739be240b`  
		Last Modified: Wed, 31 Mar 2021 16:16:48 GMT  
		Size: 2.1 MB (2128583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dc28dc62ffb258b477e485262a9beb87c472e5e8efc1b25340c43aefa76f3a`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 7.0 MB (7037371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca63f5cf91fb4e7b7b60f7e0056803a3511efaf09d51a0cf8d2993c6a6ed17a`  
		Last Modified: Wed, 31 Mar 2021 16:16:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae247ca5cfa1e3a2e1c00cb6e8a6713113aaf0334cd63663baeb40a745aafe5`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2e00324da21253f7f0beedc1d2a123fa5efbc0e732f32044159d733abe700a17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1314e5a5cb457b2a8772a9ab8d7b1c83e9190f6c1b920601a114714ef5b080e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:08 GMT
ADD file:779165b34b3be18f6c24e448997bf6497e3b27ff72954fe3cdced0ebcc77b6b8 in / 
# Tue, 30 Mar 2021 21:51:11 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:36:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 01:37:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:37:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 01:37:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 01:38:00 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 01:38:02 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 01:38:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:38:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 01:38:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cbaf854daf876ddd338771dec41777b0dfcad33c1fc8ea3512a0708333e4465`  
		Last Modified: Tue, 30 Mar 2021 21:58:44 GMT  
		Size: 24.9 MB (24873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28182091d78cadb3063bdd9ce75c263b768f3a24453ab10eeef8d29081a26b52`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa81838cd994f801fc7d925cf1700aa43b15f134a749eac7d4a4da60a15a175e`  
		Last Modified: Wed, 31 Mar 2021 01:38:24 GMT  
		Size: 1.8 MB (1839326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b00960d8e0c9e05dc7343b699974e653177c263af4f99f3f849b4062226ddf`  
		Last Modified: Wed, 31 Mar 2021 01:38:23 GMT  
		Size: 5.5 MB (5479910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0df0d7972be414ec17fc2d27808177f0e968261e2abc699a4ddea72869042`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed60abb976ac8333612b838e368cffd3ccb982d68fed535f5b555d86cb0e6ed`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a2ecd7cbd618e48f2ac7f4d3b00b9fe909835dc96b3157c7d80841126acd5562
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29787293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d0aa828b1267a40bbc50997ede10495e8260372f19aed72c57262248359a68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:38 GMT
ADD file:c1eeb99fc8ec483e175d4948a58d7f7b246b0d6b887f435a5fef07ef43699f76 in / 
# Tue, 30 Mar 2021 23:08:41 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 15:19:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 15:19:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 15:19:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 15:20:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 15:20:58 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 15:20:59 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 15:21:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 15:21:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 15:21:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee0a2cc24f2963b99b1d30dc2613f196b7c9e38337cf99332d6c4efe07f01ef2`  
		Last Modified: Tue, 30 Mar 2021 23:16:25 GMT  
		Size: 22.7 MB (22739814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8be6a509ca95801ec6352b0d77e70efad2c3e8fe0efd3dad1548741732b8b3`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c11fd226bbed81de8e0003cd6f036c206dd85afe8e6deeb9767ad0b581e22d6`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 1.8 MB (1759507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf4ccfdcc462618e5ee96b39d60d2704a6f5e08bf3d8d12e2dfb2c45a3ce0f`  
		Last Modified: Wed, 31 Mar 2021 15:21:51 GMT  
		Size: 5.3 MB (5285768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3c8b58c96829cec9b62a80a7a46b6bd22e7404d33cb7a37c479d88bdb48eb8`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3151830e9b8d885a48e1b832142170fa53238d296b4b3e0123faad10393db0`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0a4b45fae5a9c3ab28ff6bc851a0e564e32059e14176de457017dfd1c16e00a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33820038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2d8af2df852b6b33ab2e20e605cb74534629c66073a06f3f055de1fd4cb281`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:47:15 GMT
ADD file:a9b57ded2400fc7f60ea40e5ccdd3e9bf0f72acfcc47223ceb66b4fa16955059 in / 
# Tue, 30 Mar 2021 21:47:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 08:43:24 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 08:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 08:44:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 08:45:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 08:45:22 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 08:45:25 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 08:45:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 08:45:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 08:45:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fcf2156bc23db75595b822b865fbc962ed6f4521dec8cae509e66742a6a5ad3`  
		Last Modified: Tue, 30 Mar 2021 21:54:27 GMT  
		Size: 25.9 MB (25904513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cdb5faf5e1df1fdb7721b3cc208b0e5478cc605ec52b6a2400f61cba6e85ce`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b270c4bbc0b57a820e05f9f557a16d68479253c106d3e45f297281176e1a0f27`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 2.0 MB (2007905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956445c190e08fddb0ddacc2ab9fdbb2c519633cda1ff33bd0a4428a38ad13f`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 5.9 MB (5905403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5a7d98b4906f09a7b52982656cfe87cd282f920fe7691d0f6a30ce345263e2`  
		Last Modified: Wed, 31 Mar 2021 08:46:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922901517e24b86c59e9a79afa09d5fba7ba43b5eae070b1cf7cbc1da251a0d7`  
		Last Modified: Wed, 31 Mar 2021 08:46:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:c7b62ea34691dc2c5a699b708d4a0582923a757ad9b41a6b5c9ed012455e6aba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bd5250a469ba27b4d7a5c6f483a6dec8e967d14cad2362ce98bfbd924ae446`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:48 GMT
ADD file:d11c47560c0a88a83a3a0ce5af82fc17a07075e877293e4f922f126959810ea3 in / 
# Tue, 30 Mar 2021 21:39:49 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:27:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 00:27:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:27:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 00:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:28:18 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 00:28:18 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 00:28:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:28:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 00:28:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:548dde0830bd6b881c0c068db5a4e39aa720d2a0c5ac3897296a023dda7b3391`  
		Last Modified: Tue, 30 Mar 2021 21:46:41 GMT  
		Size: 27.8 MB (27788996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db59fb742889351c8257d71d9af7f8ab754780dfdb80e60bb34a5488afc26249`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2479ba868a69059ce8416072149d301726c919056b2d354373c241954b855dab`  
		Last Modified: Wed, 31 Mar 2021 00:29:13 GMT  
		Size: 2.1 MB (2132647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7d122183831a8ed76e681eeb8ead7cf5f075914d4386bf5fb20dcf081064fa`  
		Last Modified: Wed, 31 Mar 2021 00:29:20 GMT  
		Size: 11.6 MB (11633214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdfcb59f4fbfed086e7dc5075c6db916e00188a042b7612c5f03252f5eda4f6`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0645a8c57aa0c862e9773fc2240ce6dcc565e9100a5223a0f67eb77140507ccf`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:0a607e1a5fc9ebf86c4634a5bda561bd893ac0fa759d11aaa027701465a33438
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f4c96e6408daeba5bb5046d04b01073b8bf603d21a7f36a18ac577c54fd552`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 22:09:47 GMT
ADD file:b5b2f1fc18276a3928a2d904fedc2991239e065051f16680662a22627d15e809 in / 
# Tue, 30 Mar 2021 22:09:48 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 11:42:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 11:43:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 11:43:01 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 11:44:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 11:44:09 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 11:44:10 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 11:44:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 11:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 11:44:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:17fa7bb8f5ce4138c383674409fef134204b2ae72f4a997a2cebccad07e8e32b`  
		Last Modified: Tue, 30 Mar 2021 22:16:21 GMT  
		Size: 25.8 MB (25806366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a68c20179bba0326107528643f0bdfb09e5e4e12b23b94202e0a40b07b08ec`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee9cb6b3b154470e91ff1d71d60f473532f7811c34e9f9a305cb5f9b384af53`  
		Last Modified: Wed, 31 Mar 2021 11:44:37 GMT  
		Size: 1.7 MB (1712484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7e20f016e608e3dbd4989e95db2477d200c26e7139b659b5ff81af56f5849d`  
		Last Modified: Wed, 31 Mar 2021 11:44:42 GMT  
		Size: 6.4 MB (6416459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29e8d95ffa3367d7f92161d1879c4244eba457c53be1dceacf60878a6b61350`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2800304da962f86c573659de59251370b0898e93e416be1ab9a74ed6ff752d7f`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:f6cbaeb1a0ee34d3e7c450623eca946126fa422ece34b7b5ccaae82d7316e545
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39516884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01d339f442f5b9596b036ecdade36fc3df4976bd2202bb5b7dfb2ba4798b890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 22:36:03 GMT
ADD file:a544303d3ec263b38c231310d807e05249140188df5c5a5c785b2f176455ac39 in / 
# Tue, 30 Mar 2021 22:36:09 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 19:40:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 19:40:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 19:40:57 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:45:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 19:46:02 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:46:08 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:46:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:46:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c840eb5e9aed613b2af7557a4b5ad46898b8bc475a2d470c65ec7896b11282f1`  
		Last Modified: Tue, 30 Mar 2021 22:42:39 GMT  
		Size: 30.5 MB (30545907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66d37901368857c9d4854888cc81e3596f613d4ec8257b8690775870e5e4451`  
		Last Modified: Wed, 31 Mar 2021 19:48:20 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01811f1dd1f9404c028e19635d730f014630a6dc6e55e97c9b422bc8a9dd4060`  
		Last Modified: Wed, 31 Mar 2021 19:48:23 GMT  
		Size: 2.2 MB (2225118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d162ea0ebccf2afa22e63499de4dddb27ad0af7f8b57081c5be5f3f905c0bb`  
		Last Modified: Wed, 31 Mar 2021 19:48:22 GMT  
		Size: 6.7 MB (6743642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658a4880047c37829a2e4d44e876c95bca195cf5b89f8bcdf65c6a8ee32c801b`  
		Last Modified: Wed, 31 Mar 2021 19:48:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e0ea8c770ca843bdc7acbe8af1702763603347749366a3d8c401ad29ef7d6`  
		Last Modified: Wed, 31 Mar 2021 19:48:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:97d3bd125ab186461612f5227612b8bed1b7cdf339597a848150b8abb1df9748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11acca930a3acc9f10aec0e92255da2f3d7782c440d9ebe986775b5d784b5f7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 02:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 02:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 02:25:46 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 02:25:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 02:25:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 02:25:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 02:25:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c742a04892cc406ec636d3b61ae8b30ea2be9d8094b04a3e6fa844006600bb`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee293ba212f1e0d102b980847b925882c507858cf70dd83eca37c45fb14d8fb6`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 1.8 MB (1821969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048c0826dbbe30eb38c444743a578a8400ca9bb488e6dd498c2ae0c74a524ba`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 5.9 MB (5943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8fc932e810d22ad352fd6f592c4c76a7e0fc36211bb96549e2044049a0ae6c`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd24c1b830fe7b47376748fdbcf9a99c29e655cc7047927ab24e2aad8d1cf83`  
		Last Modified: Wed, 31 Mar 2021 02:26:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:965692f2f005186e45c82fbe11bd26882f64fbcbb8868d8b696d067c77dddba4
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
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a8f094524aa54d65da82ac3129b78c13a1ff5cff473d26e7953a81a96c202ab5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6d756d9322008040c5902e261b8428a4eeadbaf973e8d48fa6a7d393a33176`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:50:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 03:51:01 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 03:51:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 03:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 03:51:35 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 03:51:36 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 03:51:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08375284756efffda8b0f8680579238d367b99e6e9774c5bc2948a223609b9`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9fba38f067baa6197b369a281149dd510a1a81b8a3271a50be709bca735db`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c433c405968ee69b45b2f652261c102453e750588274755fc5de0131b9918`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 202.3 KB (202276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6fc7889befc7a0ff491331bbd30d5efd63004b5ea0da1e12bb1b849fc697b8`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1e0e8f7257294af246022ecb31dac77d4340b0787771e6d6b552b99d97616`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:654e6d7a720dfa4eb8a1d72df30b8f1e3122cba0850349dbcf246f63b93d4606
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d405b48065d7865937665d693ec98c89b327b2a5a2922eda935887d7f7d7dd0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:51:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 07:51:35 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 07:51:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 07:51:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 07:51:55 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 07:51:56 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 07:51:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:51:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d549e288a1942f308e98bd63e9a88e4b46c1fd3bf5b46f2af22e3dfde82b0bc`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aa5f33d7d1cc9f41cce3689eb319aaecec97ed85da04c9220d700f146c9e81`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e0f606528c3ab5b91505c21f3557ad732bc6d02d418edf4f63403cbe99a82`  
		Last Modified: Thu, 01 Apr 2021 07:52:32 GMT  
		Size: 223.3 KB (223283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c744159f7958c465d7ed11c8ffb2650a8a91e820729271b6c36beba8d56afae`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef80b8c05f87168506c2964fb0229d9fc6efd4fc2cc912e4b5abff7ee0a01f`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:94267d6b497d02f0f85f471c82b5b6bd0d149e12aaf359edacbbf01c941ea032
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436f12a351ea0c0ebd29c513beeb1e7e954fd1bffb8fc9aaeec88ab529a2bbca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:46:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 31 Mar 2021 19:47:04 GMT
RUN apk add --no-cache libssl1.1
# Wed, 31 Mar 2021 19:47:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:47:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 31 Mar 2021 19:47:41 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:47:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:47:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:47:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d452bef84dc63670e365215d08665984515db53171a73aac95e8fcb2e11ea8`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059bdf7279d42a1fcb055d84641ebef32bc778bca1c1d14239c4e8bd30476bd2`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96156d3c4691010d3da5a61f5368d99699eb901120314ef42751999506efe688`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 221.0 KB (220983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff346b44ef1d664ee7482a759efd0565ed8a4a05b594e069d232eee428364260`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84860a0e3e2e15db90c68d04ba424f8adfdeef75fc2e25b9719ecdd3fd36147d`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9b0cc67813eb7f0aa752ceac9a67f0a990c20bb42825249c2859fa4c8bdded4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3ca515a0fab06621288e2f56f0c5993bac9c2f08d755924e7c9bc55c818c49a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:05:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 04:05:13 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 04:05:14 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 04:05:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 04:05:24 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 04:05:24 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 04:05:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 04:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 04:05:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a77da407a39a6a710ed48a0b302a82ec9836dea247526fde76878b4d04d4b3`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128036055f163784a87fc05a861ff18406891960104c6a575ca30f8a818c353e`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96278980a8f0b6628942b7ac612213a62e6d509165baf060d771ab27163596c0`  
		Last Modified: Thu, 01 Apr 2021 04:05:40 GMT  
		Size: 205.0 KB (205039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945e86274e6ec778aa357ee0e6dfe31151c591a0db1a127e5ee5f41979c89998`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b09026e650ef5805f7c4ce3fda38c8327588b1fdafa6639994abd45f1be6b69`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:e865ca3e11696608182fd9928bd1fccd05e41d2521333555263cd32613be37e0
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
$ docker pull spiped@sha256:2e60e33376ba7a52ac3c9855c4d38f70b07e8e808d57c787fa582d14262201d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36307454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d42346bd6448e0f9af0920ba7340f9b4afbaf464bc3fd87567ce7b7440d20c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 16:15:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 16:15:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:15:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 16:16:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 16:16:19 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 16:16:20 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 16:16:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 16:16:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 16:16:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc45f75826335ee1323a9be0a79ecfade544e9266d399a602046a4ebd747de`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e84fa40c6bd50fde8152aaee374243fa3995702540318ee50f0031739be240b`  
		Last Modified: Wed, 31 Mar 2021 16:16:48 GMT  
		Size: 2.1 MB (2128583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dc28dc62ffb258b477e485262a9beb87c472e5e8efc1b25340c43aefa76f3a`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 7.0 MB (7037371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca63f5cf91fb4e7b7b60f7e0056803a3511efaf09d51a0cf8d2993c6a6ed17a`  
		Last Modified: Wed, 31 Mar 2021 16:16:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae247ca5cfa1e3a2e1c00cb6e8a6713113aaf0334cd63663baeb40a745aafe5`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2e00324da21253f7f0beedc1d2a123fa5efbc0e732f32044159d733abe700a17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1314e5a5cb457b2a8772a9ab8d7b1c83e9190f6c1b920601a114714ef5b080e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:08 GMT
ADD file:779165b34b3be18f6c24e448997bf6497e3b27ff72954fe3cdced0ebcc77b6b8 in / 
# Tue, 30 Mar 2021 21:51:11 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:36:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 01:37:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:37:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 01:37:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 01:38:00 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 01:38:02 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 01:38:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:38:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 01:38:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cbaf854daf876ddd338771dec41777b0dfcad33c1fc8ea3512a0708333e4465`  
		Last Modified: Tue, 30 Mar 2021 21:58:44 GMT  
		Size: 24.9 MB (24873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28182091d78cadb3063bdd9ce75c263b768f3a24453ab10eeef8d29081a26b52`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa81838cd994f801fc7d925cf1700aa43b15f134a749eac7d4a4da60a15a175e`  
		Last Modified: Wed, 31 Mar 2021 01:38:24 GMT  
		Size: 1.8 MB (1839326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b00960d8e0c9e05dc7343b699974e653177c263af4f99f3f849b4062226ddf`  
		Last Modified: Wed, 31 Mar 2021 01:38:23 GMT  
		Size: 5.5 MB (5479910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0df0d7972be414ec17fc2d27808177f0e968261e2abc699a4ddea72869042`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed60abb976ac8333612b838e368cffd3ccb982d68fed535f5b555d86cb0e6ed`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a2ecd7cbd618e48f2ac7f4d3b00b9fe909835dc96b3157c7d80841126acd5562
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29787293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d0aa828b1267a40bbc50997ede10495e8260372f19aed72c57262248359a68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:38 GMT
ADD file:c1eeb99fc8ec483e175d4948a58d7f7b246b0d6b887f435a5fef07ef43699f76 in / 
# Tue, 30 Mar 2021 23:08:41 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 15:19:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 15:19:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 15:19:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 15:20:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 15:20:58 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 15:20:59 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 15:21:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 15:21:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 15:21:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee0a2cc24f2963b99b1d30dc2613f196b7c9e38337cf99332d6c4efe07f01ef2`  
		Last Modified: Tue, 30 Mar 2021 23:16:25 GMT  
		Size: 22.7 MB (22739814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8be6a509ca95801ec6352b0d77e70efad2c3e8fe0efd3dad1548741732b8b3`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c11fd226bbed81de8e0003cd6f036c206dd85afe8e6deeb9767ad0b581e22d6`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 1.8 MB (1759507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf4ccfdcc462618e5ee96b39d60d2704a6f5e08bf3d8d12e2dfb2c45a3ce0f`  
		Last Modified: Wed, 31 Mar 2021 15:21:51 GMT  
		Size: 5.3 MB (5285768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3c8b58c96829cec9b62a80a7a46b6bd22e7404d33cb7a37c479d88bdb48eb8`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3151830e9b8d885a48e1b832142170fa53238d296b4b3e0123faad10393db0`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0a4b45fae5a9c3ab28ff6bc851a0e564e32059e14176de457017dfd1c16e00a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33820038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2d8af2df852b6b33ab2e20e605cb74534629c66073a06f3f055de1fd4cb281`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:47:15 GMT
ADD file:a9b57ded2400fc7f60ea40e5ccdd3e9bf0f72acfcc47223ceb66b4fa16955059 in / 
# Tue, 30 Mar 2021 21:47:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 08:43:24 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 08:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 08:44:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 08:45:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 08:45:22 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 08:45:25 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 08:45:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 08:45:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 08:45:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fcf2156bc23db75595b822b865fbc962ed6f4521dec8cae509e66742a6a5ad3`  
		Last Modified: Tue, 30 Mar 2021 21:54:27 GMT  
		Size: 25.9 MB (25904513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cdb5faf5e1df1fdb7721b3cc208b0e5478cc605ec52b6a2400f61cba6e85ce`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b270c4bbc0b57a820e05f9f557a16d68479253c106d3e45f297281176e1a0f27`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 2.0 MB (2007905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956445c190e08fddb0ddacc2ab9fdbb2c519633cda1ff33bd0a4428a38ad13f`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 5.9 MB (5905403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5a7d98b4906f09a7b52982656cfe87cd282f920fe7691d0f6a30ce345263e2`  
		Last Modified: Wed, 31 Mar 2021 08:46:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922901517e24b86c59e9a79afa09d5fba7ba43b5eae070b1cf7cbc1da251a0d7`  
		Last Modified: Wed, 31 Mar 2021 08:46:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:c7b62ea34691dc2c5a699b708d4a0582923a757ad9b41a6b5c9ed012455e6aba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bd5250a469ba27b4d7a5c6f483a6dec8e967d14cad2362ce98bfbd924ae446`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:48 GMT
ADD file:d11c47560c0a88a83a3a0ce5af82fc17a07075e877293e4f922f126959810ea3 in / 
# Tue, 30 Mar 2021 21:39:49 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:27:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 00:27:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:27:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 00:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:28:18 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 00:28:18 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 00:28:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:28:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 00:28:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:548dde0830bd6b881c0c068db5a4e39aa720d2a0c5ac3897296a023dda7b3391`  
		Last Modified: Tue, 30 Mar 2021 21:46:41 GMT  
		Size: 27.8 MB (27788996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db59fb742889351c8257d71d9af7f8ab754780dfdb80e60bb34a5488afc26249`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2479ba868a69059ce8416072149d301726c919056b2d354373c241954b855dab`  
		Last Modified: Wed, 31 Mar 2021 00:29:13 GMT  
		Size: 2.1 MB (2132647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7d122183831a8ed76e681eeb8ead7cf5f075914d4386bf5fb20dcf081064fa`  
		Last Modified: Wed, 31 Mar 2021 00:29:20 GMT  
		Size: 11.6 MB (11633214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdfcb59f4fbfed086e7dc5075c6db916e00188a042b7612c5f03252f5eda4f6`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0645a8c57aa0c862e9773fc2240ce6dcc565e9100a5223a0f67eb77140507ccf`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:0a607e1a5fc9ebf86c4634a5bda561bd893ac0fa759d11aaa027701465a33438
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f4c96e6408daeba5bb5046d04b01073b8bf603d21a7f36a18ac577c54fd552`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 22:09:47 GMT
ADD file:b5b2f1fc18276a3928a2d904fedc2991239e065051f16680662a22627d15e809 in / 
# Tue, 30 Mar 2021 22:09:48 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 11:42:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 11:43:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 11:43:01 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 11:44:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 11:44:09 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 11:44:10 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 11:44:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 11:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 11:44:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:17fa7bb8f5ce4138c383674409fef134204b2ae72f4a997a2cebccad07e8e32b`  
		Last Modified: Tue, 30 Mar 2021 22:16:21 GMT  
		Size: 25.8 MB (25806366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a68c20179bba0326107528643f0bdfb09e5e4e12b23b94202e0a40b07b08ec`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee9cb6b3b154470e91ff1d71d60f473532f7811c34e9f9a305cb5f9b384af53`  
		Last Modified: Wed, 31 Mar 2021 11:44:37 GMT  
		Size: 1.7 MB (1712484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7e20f016e608e3dbd4989e95db2477d200c26e7139b659b5ff81af56f5849d`  
		Last Modified: Wed, 31 Mar 2021 11:44:42 GMT  
		Size: 6.4 MB (6416459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29e8d95ffa3367d7f92161d1879c4244eba457c53be1dceacf60878a6b61350`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2800304da962f86c573659de59251370b0898e93e416be1ab9a74ed6ff752d7f`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:f6cbaeb1a0ee34d3e7c450623eca946126fa422ece34b7b5ccaae82d7316e545
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39516884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01d339f442f5b9596b036ecdade36fc3df4976bd2202bb5b7dfb2ba4798b890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 22:36:03 GMT
ADD file:a544303d3ec263b38c231310d807e05249140188df5c5a5c785b2f176455ac39 in / 
# Tue, 30 Mar 2021 22:36:09 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 19:40:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 19:40:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 19:40:57 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:45:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 19:46:02 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:46:08 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:46:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:46:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c840eb5e9aed613b2af7557a4b5ad46898b8bc475a2d470c65ec7896b11282f1`  
		Last Modified: Tue, 30 Mar 2021 22:42:39 GMT  
		Size: 30.5 MB (30545907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66d37901368857c9d4854888cc81e3596f613d4ec8257b8690775870e5e4451`  
		Last Modified: Wed, 31 Mar 2021 19:48:20 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01811f1dd1f9404c028e19635d730f014630a6dc6e55e97c9b422bc8a9dd4060`  
		Last Modified: Wed, 31 Mar 2021 19:48:23 GMT  
		Size: 2.2 MB (2225118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d162ea0ebccf2afa22e63499de4dddb27ad0af7f8b57081c5be5f3f905c0bb`  
		Last Modified: Wed, 31 Mar 2021 19:48:22 GMT  
		Size: 6.7 MB (6743642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658a4880047c37829a2e4d44e876c95bca195cf5b89f8bcdf65c6a8ee32c801b`  
		Last Modified: Wed, 31 Mar 2021 19:48:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e0ea8c770ca843bdc7acbe8af1702763603347749366a3d8c401ad29ef7d6`  
		Last Modified: Wed, 31 Mar 2021 19:48:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:97d3bd125ab186461612f5227612b8bed1b7cdf339597a848150b8abb1df9748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11acca930a3acc9f10aec0e92255da2f3d7782c440d9ebe986775b5d784b5f7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 02:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 02:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 02:25:46 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 02:25:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 02:25:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 02:25:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 02:25:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c742a04892cc406ec636d3b61ae8b30ea2be9d8094b04a3e6fa844006600bb`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee293ba212f1e0d102b980847b925882c507858cf70dd83eca37c45fb14d8fb6`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 1.8 MB (1821969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048c0826dbbe30eb38c444743a578a8400ca9bb488e6dd498c2ae0c74a524ba`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 5.9 MB (5943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8fc932e810d22ad352fd6f592c4c76a7e0fc36211bb96549e2044049a0ae6c`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd24c1b830fe7b47376748fdbcf9a99c29e655cc7047927ab24e2aad8d1cf83`  
		Last Modified: Wed, 31 Mar 2021 02:26:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:965692f2f005186e45c82fbe11bd26882f64fbcbb8868d8b696d067c77dddba4
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
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a8f094524aa54d65da82ac3129b78c13a1ff5cff473d26e7953a81a96c202ab5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6d756d9322008040c5902e261b8428a4eeadbaf973e8d48fa6a7d393a33176`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:50:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 03:51:01 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 03:51:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 03:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 03:51:35 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 03:51:36 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 03:51:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08375284756efffda8b0f8680579238d367b99e6e9774c5bc2948a223609b9`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9fba38f067baa6197b369a281149dd510a1a81b8a3271a50be709bca735db`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c433c405968ee69b45b2f652261c102453e750588274755fc5de0131b9918`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 202.3 KB (202276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6fc7889befc7a0ff491331bbd30d5efd63004b5ea0da1e12bb1b849fc697b8`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1e0e8f7257294af246022ecb31dac77d4340b0787771e6d6b552b99d97616`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:654e6d7a720dfa4eb8a1d72df30b8f1e3122cba0850349dbcf246f63b93d4606
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d405b48065d7865937665d693ec98c89b327b2a5a2922eda935887d7f7d7dd0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:51:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 07:51:35 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 07:51:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 07:51:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 07:51:55 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 07:51:56 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 07:51:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:51:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d549e288a1942f308e98bd63e9a88e4b46c1fd3bf5b46f2af22e3dfde82b0bc`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aa5f33d7d1cc9f41cce3689eb319aaecec97ed85da04c9220d700f146c9e81`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e0f606528c3ab5b91505c21f3557ad732bc6d02d418edf4f63403cbe99a82`  
		Last Modified: Thu, 01 Apr 2021 07:52:32 GMT  
		Size: 223.3 KB (223283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c744159f7958c465d7ed11c8ffb2650a8a91e820729271b6c36beba8d56afae`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef80b8c05f87168506c2964fb0229d9fc6efd4fc2cc912e4b5abff7ee0a01f`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:94267d6b497d02f0f85f471c82b5b6bd0d149e12aaf359edacbbf01c941ea032
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436f12a351ea0c0ebd29c513beeb1e7e954fd1bffb8fc9aaeec88ab529a2bbca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:46:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 31 Mar 2021 19:47:04 GMT
RUN apk add --no-cache libssl1.1
# Wed, 31 Mar 2021 19:47:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:47:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 31 Mar 2021 19:47:41 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:47:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:47:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:47:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d452bef84dc63670e365215d08665984515db53171a73aac95e8fcb2e11ea8`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059bdf7279d42a1fcb055d84641ebef32bc778bca1c1d14239c4e8bd30476bd2`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96156d3c4691010d3da5a61f5368d99699eb901120314ef42751999506efe688`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 221.0 KB (220983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff346b44ef1d664ee7482a759efd0565ed8a4a05b594e069d232eee428364260`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84860a0e3e2e15db90c68d04ba424f8adfdeef75fc2e25b9719ecdd3fd36147d`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9b0cc67813eb7f0aa752ceac9a67f0a990c20bb42825249c2859fa4c8bdded4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3ca515a0fab06621288e2f56f0c5993bac9c2f08d755924e7c9bc55c818c49a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:05:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 04:05:13 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 04:05:14 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 04:05:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 04:05:24 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 04:05:24 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 04:05:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 04:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 04:05:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a77da407a39a6a710ed48a0b302a82ec9836dea247526fde76878b4d04d4b3`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128036055f163784a87fc05a861ff18406891960104c6a575ca30f8a818c353e`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96278980a8f0b6628942b7ac612213a62e6d509165baf060d771ab27163596c0`  
		Last Modified: Thu, 01 Apr 2021 04:05:40 GMT  
		Size: 205.0 KB (205039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945e86274e6ec778aa357ee0e6dfe31151c591a0db1a127e5ee5f41979c89998`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b09026e650ef5805f7c4ce3fda38c8327588b1fdafa6639994abd45f1be6b69`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:e865ca3e11696608182fd9928bd1fccd05e41d2521333555263cd32613be37e0
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
$ docker pull spiped@sha256:2e60e33376ba7a52ac3c9855c4d38f70b07e8e808d57c787fa582d14262201d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36307454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d42346bd6448e0f9af0920ba7340f9b4afbaf464bc3fd87567ce7b7440d20c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 16:15:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 16:15:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:15:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 16:16:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 16:16:19 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 16:16:20 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 16:16:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 16:16:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 16:16:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc45f75826335ee1323a9be0a79ecfade544e9266d399a602046a4ebd747de`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e84fa40c6bd50fde8152aaee374243fa3995702540318ee50f0031739be240b`  
		Last Modified: Wed, 31 Mar 2021 16:16:48 GMT  
		Size: 2.1 MB (2128583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dc28dc62ffb258b477e485262a9beb87c472e5e8efc1b25340c43aefa76f3a`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 7.0 MB (7037371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca63f5cf91fb4e7b7b60f7e0056803a3511efaf09d51a0cf8d2993c6a6ed17a`  
		Last Modified: Wed, 31 Mar 2021 16:16:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae247ca5cfa1e3a2e1c00cb6e8a6713113aaf0334cd63663baeb40a745aafe5`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2e00324da21253f7f0beedc1d2a123fa5efbc0e732f32044159d733abe700a17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1314e5a5cb457b2a8772a9ab8d7b1c83e9190f6c1b920601a114714ef5b080e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:08 GMT
ADD file:779165b34b3be18f6c24e448997bf6497e3b27ff72954fe3cdced0ebcc77b6b8 in / 
# Tue, 30 Mar 2021 21:51:11 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:36:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 01:37:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:37:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 01:37:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 01:38:00 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 01:38:02 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 01:38:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:38:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 01:38:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cbaf854daf876ddd338771dec41777b0dfcad33c1fc8ea3512a0708333e4465`  
		Last Modified: Tue, 30 Mar 2021 21:58:44 GMT  
		Size: 24.9 MB (24873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28182091d78cadb3063bdd9ce75c263b768f3a24453ab10eeef8d29081a26b52`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa81838cd994f801fc7d925cf1700aa43b15f134a749eac7d4a4da60a15a175e`  
		Last Modified: Wed, 31 Mar 2021 01:38:24 GMT  
		Size: 1.8 MB (1839326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b00960d8e0c9e05dc7343b699974e653177c263af4f99f3f849b4062226ddf`  
		Last Modified: Wed, 31 Mar 2021 01:38:23 GMT  
		Size: 5.5 MB (5479910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0df0d7972be414ec17fc2d27808177f0e968261e2abc699a4ddea72869042`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed60abb976ac8333612b838e368cffd3ccb982d68fed535f5b555d86cb0e6ed`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a2ecd7cbd618e48f2ac7f4d3b00b9fe909835dc96b3157c7d80841126acd5562
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29787293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d0aa828b1267a40bbc50997ede10495e8260372f19aed72c57262248359a68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:38 GMT
ADD file:c1eeb99fc8ec483e175d4948a58d7f7b246b0d6b887f435a5fef07ef43699f76 in / 
# Tue, 30 Mar 2021 23:08:41 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 15:19:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 15:19:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 15:19:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 15:20:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 15:20:58 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 15:20:59 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 15:21:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 15:21:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 15:21:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee0a2cc24f2963b99b1d30dc2613f196b7c9e38337cf99332d6c4efe07f01ef2`  
		Last Modified: Tue, 30 Mar 2021 23:16:25 GMT  
		Size: 22.7 MB (22739814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8be6a509ca95801ec6352b0d77e70efad2c3e8fe0efd3dad1548741732b8b3`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c11fd226bbed81de8e0003cd6f036c206dd85afe8e6deeb9767ad0b581e22d6`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 1.8 MB (1759507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf4ccfdcc462618e5ee96b39d60d2704a6f5e08bf3d8d12e2dfb2c45a3ce0f`  
		Last Modified: Wed, 31 Mar 2021 15:21:51 GMT  
		Size: 5.3 MB (5285768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3c8b58c96829cec9b62a80a7a46b6bd22e7404d33cb7a37c479d88bdb48eb8`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3151830e9b8d885a48e1b832142170fa53238d296b4b3e0123faad10393db0`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0a4b45fae5a9c3ab28ff6bc851a0e564e32059e14176de457017dfd1c16e00a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33820038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2d8af2df852b6b33ab2e20e605cb74534629c66073a06f3f055de1fd4cb281`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:47:15 GMT
ADD file:a9b57ded2400fc7f60ea40e5ccdd3e9bf0f72acfcc47223ceb66b4fa16955059 in / 
# Tue, 30 Mar 2021 21:47:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 08:43:24 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 08:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 08:44:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 08:45:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 08:45:22 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 08:45:25 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 08:45:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 08:45:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 08:45:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fcf2156bc23db75595b822b865fbc962ed6f4521dec8cae509e66742a6a5ad3`  
		Last Modified: Tue, 30 Mar 2021 21:54:27 GMT  
		Size: 25.9 MB (25904513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cdb5faf5e1df1fdb7721b3cc208b0e5478cc605ec52b6a2400f61cba6e85ce`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b270c4bbc0b57a820e05f9f557a16d68479253c106d3e45f297281176e1a0f27`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 2.0 MB (2007905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956445c190e08fddb0ddacc2ab9fdbb2c519633cda1ff33bd0a4428a38ad13f`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 5.9 MB (5905403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5a7d98b4906f09a7b52982656cfe87cd282f920fe7691d0f6a30ce345263e2`  
		Last Modified: Wed, 31 Mar 2021 08:46:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922901517e24b86c59e9a79afa09d5fba7ba43b5eae070b1cf7cbc1da251a0d7`  
		Last Modified: Wed, 31 Mar 2021 08:46:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:c7b62ea34691dc2c5a699b708d4a0582923a757ad9b41a6b5c9ed012455e6aba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bd5250a469ba27b4d7a5c6f483a6dec8e967d14cad2362ce98bfbd924ae446`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:48 GMT
ADD file:d11c47560c0a88a83a3a0ce5af82fc17a07075e877293e4f922f126959810ea3 in / 
# Tue, 30 Mar 2021 21:39:49 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:27:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 00:27:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:27:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 00:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:28:18 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 00:28:18 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 00:28:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:28:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 00:28:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:548dde0830bd6b881c0c068db5a4e39aa720d2a0c5ac3897296a023dda7b3391`  
		Last Modified: Tue, 30 Mar 2021 21:46:41 GMT  
		Size: 27.8 MB (27788996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db59fb742889351c8257d71d9af7f8ab754780dfdb80e60bb34a5488afc26249`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2479ba868a69059ce8416072149d301726c919056b2d354373c241954b855dab`  
		Last Modified: Wed, 31 Mar 2021 00:29:13 GMT  
		Size: 2.1 MB (2132647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7d122183831a8ed76e681eeb8ead7cf5f075914d4386bf5fb20dcf081064fa`  
		Last Modified: Wed, 31 Mar 2021 00:29:20 GMT  
		Size: 11.6 MB (11633214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdfcb59f4fbfed086e7dc5075c6db916e00188a042b7612c5f03252f5eda4f6`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0645a8c57aa0c862e9773fc2240ce6dcc565e9100a5223a0f67eb77140507ccf`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:0a607e1a5fc9ebf86c4634a5bda561bd893ac0fa759d11aaa027701465a33438
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f4c96e6408daeba5bb5046d04b01073b8bf603d21a7f36a18ac577c54fd552`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 22:09:47 GMT
ADD file:b5b2f1fc18276a3928a2d904fedc2991239e065051f16680662a22627d15e809 in / 
# Tue, 30 Mar 2021 22:09:48 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 11:42:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 11:43:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 11:43:01 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 11:44:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 11:44:09 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 11:44:10 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 11:44:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 11:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 11:44:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:17fa7bb8f5ce4138c383674409fef134204b2ae72f4a997a2cebccad07e8e32b`  
		Last Modified: Tue, 30 Mar 2021 22:16:21 GMT  
		Size: 25.8 MB (25806366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a68c20179bba0326107528643f0bdfb09e5e4e12b23b94202e0a40b07b08ec`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee9cb6b3b154470e91ff1d71d60f473532f7811c34e9f9a305cb5f9b384af53`  
		Last Modified: Wed, 31 Mar 2021 11:44:37 GMT  
		Size: 1.7 MB (1712484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7e20f016e608e3dbd4989e95db2477d200c26e7139b659b5ff81af56f5849d`  
		Last Modified: Wed, 31 Mar 2021 11:44:42 GMT  
		Size: 6.4 MB (6416459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29e8d95ffa3367d7f92161d1879c4244eba457c53be1dceacf60878a6b61350`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2800304da962f86c573659de59251370b0898e93e416be1ab9a74ed6ff752d7f`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:f6cbaeb1a0ee34d3e7c450623eca946126fa422ece34b7b5ccaae82d7316e545
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39516884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01d339f442f5b9596b036ecdade36fc3df4976bd2202bb5b7dfb2ba4798b890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 22:36:03 GMT
ADD file:a544303d3ec263b38c231310d807e05249140188df5c5a5c785b2f176455ac39 in / 
# Tue, 30 Mar 2021 22:36:09 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 19:40:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 19:40:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 19:40:57 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:45:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 19:46:02 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:46:08 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:46:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:46:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c840eb5e9aed613b2af7557a4b5ad46898b8bc475a2d470c65ec7896b11282f1`  
		Last Modified: Tue, 30 Mar 2021 22:42:39 GMT  
		Size: 30.5 MB (30545907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66d37901368857c9d4854888cc81e3596f613d4ec8257b8690775870e5e4451`  
		Last Modified: Wed, 31 Mar 2021 19:48:20 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01811f1dd1f9404c028e19635d730f014630a6dc6e55e97c9b422bc8a9dd4060`  
		Last Modified: Wed, 31 Mar 2021 19:48:23 GMT  
		Size: 2.2 MB (2225118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d162ea0ebccf2afa22e63499de4dddb27ad0af7f8b57081c5be5f3f905c0bb`  
		Last Modified: Wed, 31 Mar 2021 19:48:22 GMT  
		Size: 6.7 MB (6743642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658a4880047c37829a2e4d44e876c95bca195cf5b89f8bcdf65c6a8ee32c801b`  
		Last Modified: Wed, 31 Mar 2021 19:48:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e0ea8c770ca843bdc7acbe8af1702763603347749366a3d8c401ad29ef7d6`  
		Last Modified: Wed, 31 Mar 2021 19:48:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:97d3bd125ab186461612f5227612b8bed1b7cdf339597a848150b8abb1df9748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11acca930a3acc9f10aec0e92255da2f3d7782c440d9ebe986775b5d784b5f7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 02:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 02:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 02:25:46 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 02:25:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 02:25:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 02:25:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 02:25:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c742a04892cc406ec636d3b61ae8b30ea2be9d8094b04a3e6fa844006600bb`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee293ba212f1e0d102b980847b925882c507858cf70dd83eca37c45fb14d8fb6`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 1.8 MB (1821969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048c0826dbbe30eb38c444743a578a8400ca9bb488e6dd498c2ae0c74a524ba`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 5.9 MB (5943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8fc932e810d22ad352fd6f592c4c76a7e0fc36211bb96549e2044049a0ae6c`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd24c1b830fe7b47376748fdbcf9a99c29e655cc7047927ab24e2aad8d1cf83`  
		Last Modified: Wed, 31 Mar 2021 02:26:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:965692f2f005186e45c82fbe11bd26882f64fbcbb8868d8b696d067c77dddba4
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
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a8f094524aa54d65da82ac3129b78c13a1ff5cff473d26e7953a81a96c202ab5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6d756d9322008040c5902e261b8428a4eeadbaf973e8d48fa6a7d393a33176`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:50:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 03:51:01 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 03:51:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 03:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 03:51:35 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 03:51:36 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 03:51:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08375284756efffda8b0f8680579238d367b99e6e9774c5bc2948a223609b9`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9fba38f067baa6197b369a281149dd510a1a81b8a3271a50be709bca735db`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c433c405968ee69b45b2f652261c102453e750588274755fc5de0131b9918`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 202.3 KB (202276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6fc7889befc7a0ff491331bbd30d5efd63004b5ea0da1e12bb1b849fc697b8`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1e0e8f7257294af246022ecb31dac77d4340b0787771e6d6b552b99d97616`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:654e6d7a720dfa4eb8a1d72df30b8f1e3122cba0850349dbcf246f63b93d4606
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d405b48065d7865937665d693ec98c89b327b2a5a2922eda935887d7f7d7dd0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:51:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 07:51:35 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 07:51:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 07:51:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 07:51:55 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 07:51:56 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 07:51:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:51:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d549e288a1942f308e98bd63e9a88e4b46c1fd3bf5b46f2af22e3dfde82b0bc`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aa5f33d7d1cc9f41cce3689eb319aaecec97ed85da04c9220d700f146c9e81`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e0f606528c3ab5b91505c21f3557ad732bc6d02d418edf4f63403cbe99a82`  
		Last Modified: Thu, 01 Apr 2021 07:52:32 GMT  
		Size: 223.3 KB (223283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c744159f7958c465d7ed11c8ffb2650a8a91e820729271b6c36beba8d56afae`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef80b8c05f87168506c2964fb0229d9fc6efd4fc2cc912e4b5abff7ee0a01f`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:94267d6b497d02f0f85f471c82b5b6bd0d149e12aaf359edacbbf01c941ea032
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436f12a351ea0c0ebd29c513beeb1e7e954fd1bffb8fc9aaeec88ab529a2bbca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:46:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 31 Mar 2021 19:47:04 GMT
RUN apk add --no-cache libssl1.1
# Wed, 31 Mar 2021 19:47:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:47:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 31 Mar 2021 19:47:41 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:47:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:47:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:47:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d452bef84dc63670e365215d08665984515db53171a73aac95e8fcb2e11ea8`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059bdf7279d42a1fcb055d84641ebef32bc778bca1c1d14239c4e8bd30476bd2`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96156d3c4691010d3da5a61f5368d99699eb901120314ef42751999506efe688`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 221.0 KB (220983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff346b44ef1d664ee7482a759efd0565ed8a4a05b594e069d232eee428364260`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84860a0e3e2e15db90c68d04ba424f8adfdeef75fc2e25b9719ecdd3fd36147d`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9b0cc67813eb7f0aa752ceac9a67f0a990c20bb42825249c2859fa4c8bdded4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3ca515a0fab06621288e2f56f0c5993bac9c2f08d755924e7c9bc55c818c49a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:05:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 04:05:13 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 04:05:14 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 04:05:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 04:05:24 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 04:05:24 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 04:05:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 04:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 04:05:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a77da407a39a6a710ed48a0b302a82ec9836dea247526fde76878b4d04d4b3`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128036055f163784a87fc05a861ff18406891960104c6a575ca30f8a818c353e`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96278980a8f0b6628942b7ac612213a62e6d509165baf060d771ab27163596c0`  
		Last Modified: Thu, 01 Apr 2021 04:05:40 GMT  
		Size: 205.0 KB (205039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945e86274e6ec778aa357ee0e6dfe31151c591a0db1a127e5ee5f41979c89998`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b09026e650ef5805f7c4ce3fda38c8327588b1fdafa6639994abd45f1be6b69`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:965692f2f005186e45c82fbe11bd26882f64fbcbb8868d8b696d067c77dddba4
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
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a8f094524aa54d65da82ac3129b78c13a1ff5cff473d26e7953a81a96c202ab5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6d756d9322008040c5902e261b8428a4eeadbaf973e8d48fa6a7d393a33176`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:50:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 03:51:01 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 03:51:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 03:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 03:51:35 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 03:51:36 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 03:51:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08375284756efffda8b0f8680579238d367b99e6e9774c5bc2948a223609b9`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9fba38f067baa6197b369a281149dd510a1a81b8a3271a50be709bca735db`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c433c405968ee69b45b2f652261c102453e750588274755fc5de0131b9918`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 202.3 KB (202276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6fc7889befc7a0ff491331bbd30d5efd63004b5ea0da1e12bb1b849fc697b8`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1e0e8f7257294af246022ecb31dac77d4340b0787771e6d6b552b99d97616`  
		Last Modified: Thu, 01 Apr 2021 03:51:59 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:654e6d7a720dfa4eb8a1d72df30b8f1e3122cba0850349dbcf246f63b93d4606
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d405b48065d7865937665d693ec98c89b327b2a5a2922eda935887d7f7d7dd0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:51:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 07:51:35 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 07:51:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 07:51:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 07:51:55 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 07:51:56 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 07:51:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:51:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d549e288a1942f308e98bd63e9a88e4b46c1fd3bf5b46f2af22e3dfde82b0bc`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aa5f33d7d1cc9f41cce3689eb319aaecec97ed85da04c9220d700f146c9e81`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e0f606528c3ab5b91505c21f3557ad732bc6d02d418edf4f63403cbe99a82`  
		Last Modified: Thu, 01 Apr 2021 07:52:32 GMT  
		Size: 223.3 KB (223283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c744159f7958c465d7ed11c8ffb2650a8a91e820729271b6c36beba8d56afae`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ef80b8c05f87168506c2964fb0229d9fc6efd4fc2cc912e4b5abff7ee0a01f`  
		Last Modified: Thu, 01 Apr 2021 07:52:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:94267d6b497d02f0f85f471c82b5b6bd0d149e12aaf359edacbbf01c941ea032
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436f12a351ea0c0ebd29c513beeb1e7e954fd1bffb8fc9aaeec88ab529a2bbca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:46:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 31 Mar 2021 19:47:04 GMT
RUN apk add --no-cache libssl1.1
# Wed, 31 Mar 2021 19:47:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:47:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 31 Mar 2021 19:47:41 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:47:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:47:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:47:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d452bef84dc63670e365215d08665984515db53171a73aac95e8fcb2e11ea8`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059bdf7279d42a1fcb055d84641ebef32bc778bca1c1d14239c4e8bd30476bd2`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96156d3c4691010d3da5a61f5368d99699eb901120314ef42751999506efe688`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 221.0 KB (220983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff346b44ef1d664ee7482a759efd0565ed8a4a05b594e069d232eee428364260`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84860a0e3e2e15db90c68d04ba424f8adfdeef75fc2e25b9719ecdd3fd36147d`  
		Last Modified: Wed, 31 Mar 2021 19:48:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9b0cc67813eb7f0aa752ceac9a67f0a990c20bb42825249c2859fa4c8bdded4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3ca515a0fab06621288e2f56f0c5993bac9c2f08d755924e7c9bc55c818c49a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:05:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Apr 2021 04:05:13 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Apr 2021 04:05:14 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 01 Apr 2021 04:05:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 01 Apr 2021 04:05:24 GMT
VOLUME [/spiped]
# Thu, 01 Apr 2021 04:05:24 GMT
WORKDIR /spiped
# Thu, 01 Apr 2021 04:05:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Apr 2021 04:05:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 04:05:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a77da407a39a6a710ed48a0b302a82ec9836dea247526fde76878b4d04d4b3`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128036055f163784a87fc05a861ff18406891960104c6a575ca30f8a818c353e`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96278980a8f0b6628942b7ac612213a62e6d509165baf060d771ab27163596c0`  
		Last Modified: Thu, 01 Apr 2021 04:05:40 GMT  
		Size: 205.0 KB (205039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945e86274e6ec778aa357ee0e6dfe31151c591a0db1a127e5ee5f41979c89998`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b09026e650ef5805f7c4ce3fda38c8327588b1fdafa6639994abd45f1be6b69`  
		Last Modified: Thu, 01 Apr 2021 04:05:39 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:e865ca3e11696608182fd9928bd1fccd05e41d2521333555263cd32613be37e0
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
$ docker pull spiped@sha256:2e60e33376ba7a52ac3c9855c4d38f70b07e8e808d57c787fa582d14262201d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36307454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d42346bd6448e0f9af0920ba7340f9b4afbaf464bc3fd87567ce7b7440d20c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 16:15:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 16:15:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:15:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 16:16:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 16:16:19 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 16:16:20 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 16:16:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 16:16:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 16:16:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc45f75826335ee1323a9be0a79ecfade544e9266d399a602046a4ebd747de`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e84fa40c6bd50fde8152aaee374243fa3995702540318ee50f0031739be240b`  
		Last Modified: Wed, 31 Mar 2021 16:16:48 GMT  
		Size: 2.1 MB (2128583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dc28dc62ffb258b477e485262a9beb87c472e5e8efc1b25340c43aefa76f3a`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 7.0 MB (7037371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca63f5cf91fb4e7b7b60f7e0056803a3511efaf09d51a0cf8d2993c6a6ed17a`  
		Last Modified: Wed, 31 Mar 2021 16:16:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae247ca5cfa1e3a2e1c00cb6e8a6713113aaf0334cd63663baeb40a745aafe5`  
		Last Modified: Wed, 31 Mar 2021 16:16:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2e00324da21253f7f0beedc1d2a123fa5efbc0e732f32044159d733abe700a17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32194651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1314e5a5cb457b2a8772a9ab8d7b1c83e9190f6c1b920601a114714ef5b080e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:08 GMT
ADD file:779165b34b3be18f6c24e448997bf6497e3b27ff72954fe3cdced0ebcc77b6b8 in / 
# Tue, 30 Mar 2021 21:51:11 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:36:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 01:37:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:37:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 01:37:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 01:38:00 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 01:38:02 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 01:38:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:38:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 01:38:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7cbaf854daf876ddd338771dec41777b0dfcad33c1fc8ea3512a0708333e4465`  
		Last Modified: Tue, 30 Mar 2021 21:58:44 GMT  
		Size: 24.9 MB (24873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28182091d78cadb3063bdd9ce75c263b768f3a24453ab10eeef8d29081a26b52`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa81838cd994f801fc7d925cf1700aa43b15f134a749eac7d4a4da60a15a175e`  
		Last Modified: Wed, 31 Mar 2021 01:38:24 GMT  
		Size: 1.8 MB (1839326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b00960d8e0c9e05dc7343b699974e653177c263af4f99f3f849b4062226ddf`  
		Last Modified: Wed, 31 Mar 2021 01:38:23 GMT  
		Size: 5.5 MB (5479910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c0df0d7972be414ec17fc2d27808177f0e968261e2abc699a4ddea72869042`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed60abb976ac8333612b838e368cffd3ccb982d68fed535f5b555d86cb0e6ed`  
		Last Modified: Wed, 31 Mar 2021 01:38:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a2ecd7cbd618e48f2ac7f4d3b00b9fe909835dc96b3157c7d80841126acd5562
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29787293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d0aa828b1267a40bbc50997ede10495e8260372f19aed72c57262248359a68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:38 GMT
ADD file:c1eeb99fc8ec483e175d4948a58d7f7b246b0d6b887f435a5fef07ef43699f76 in / 
# Tue, 30 Mar 2021 23:08:41 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 15:19:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 15:19:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 15:19:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 15:20:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 15:20:58 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 15:20:59 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 15:21:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 15:21:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 15:21:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee0a2cc24f2963b99b1d30dc2613f196b7c9e38337cf99332d6c4efe07f01ef2`  
		Last Modified: Tue, 30 Mar 2021 23:16:25 GMT  
		Size: 22.7 MB (22739814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8be6a509ca95801ec6352b0d77e70efad2c3e8fe0efd3dad1548741732b8b3`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c11fd226bbed81de8e0003cd6f036c206dd85afe8e6deeb9767ad0b581e22d6`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 1.8 MB (1759507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf4ccfdcc462618e5ee96b39d60d2704a6f5e08bf3d8d12e2dfb2c45a3ce0f`  
		Last Modified: Wed, 31 Mar 2021 15:21:51 GMT  
		Size: 5.3 MB (5285768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3c8b58c96829cec9b62a80a7a46b6bd22e7404d33cb7a37c479d88bdb48eb8`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3151830e9b8d885a48e1b832142170fa53238d296b4b3e0123faad10393db0`  
		Last Modified: Wed, 31 Mar 2021 15:21:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0a4b45fae5a9c3ab28ff6bc851a0e564e32059e14176de457017dfd1c16e00a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33820038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2d8af2df852b6b33ab2e20e605cb74534629c66073a06f3f055de1fd4cb281`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:47:15 GMT
ADD file:a9b57ded2400fc7f60ea40e5ccdd3e9bf0f72acfcc47223ceb66b4fa16955059 in / 
# Tue, 30 Mar 2021 21:47:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 08:43:24 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 08:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 08:44:06 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 08:45:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 08:45:22 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 08:45:25 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 08:45:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 08:45:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 08:45:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fcf2156bc23db75595b822b865fbc962ed6f4521dec8cae509e66742a6a5ad3`  
		Last Modified: Tue, 30 Mar 2021 21:54:27 GMT  
		Size: 25.9 MB (25904513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cdb5faf5e1df1fdb7721b3cc208b0e5478cc605ec52b6a2400f61cba6e85ce`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b270c4bbc0b57a820e05f9f557a16d68479253c106d3e45f297281176e1a0f27`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 2.0 MB (2007905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956445c190e08fddb0ddacc2ab9fdbb2c519633cda1ff33bd0a4428a38ad13f`  
		Last Modified: Wed, 31 Mar 2021 08:46:05 GMT  
		Size: 5.9 MB (5905403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5a7d98b4906f09a7b52982656cfe87cd282f920fe7691d0f6a30ce345263e2`  
		Last Modified: Wed, 31 Mar 2021 08:46:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922901517e24b86c59e9a79afa09d5fba7ba43b5eae070b1cf7cbc1da251a0d7`  
		Last Modified: Wed, 31 Mar 2021 08:46:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:c7b62ea34691dc2c5a699b708d4a0582923a757ad9b41a6b5c9ed012455e6aba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bd5250a469ba27b4d7a5c6f483a6dec8e967d14cad2362ce98bfbd924ae446`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:48 GMT
ADD file:d11c47560c0a88a83a3a0ce5af82fc17a07075e877293e4f922f126959810ea3 in / 
# Tue, 30 Mar 2021 21:39:49 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:27:22 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 00:27:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:27:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 00:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 00:28:18 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 00:28:18 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 00:28:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:28:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 00:28:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:548dde0830bd6b881c0c068db5a4e39aa720d2a0c5ac3897296a023dda7b3391`  
		Last Modified: Tue, 30 Mar 2021 21:46:41 GMT  
		Size: 27.8 MB (27788996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db59fb742889351c8257d71d9af7f8ab754780dfdb80e60bb34a5488afc26249`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2479ba868a69059ce8416072149d301726c919056b2d354373c241954b855dab`  
		Last Modified: Wed, 31 Mar 2021 00:29:13 GMT  
		Size: 2.1 MB (2132647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7d122183831a8ed76e681eeb8ead7cf5f075914d4386bf5fb20dcf081064fa`  
		Last Modified: Wed, 31 Mar 2021 00:29:20 GMT  
		Size: 11.6 MB (11633214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdfcb59f4fbfed086e7dc5075c6db916e00188a042b7612c5f03252f5eda4f6`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0645a8c57aa0c862e9773fc2240ce6dcc565e9100a5223a0f67eb77140507ccf`  
		Last Modified: Wed, 31 Mar 2021 00:29:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:0a607e1a5fc9ebf86c4634a5bda561bd893ac0fa759d11aaa027701465a33438
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f4c96e6408daeba5bb5046d04b01073b8bf603d21a7f36a18ac577c54fd552`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 22:09:47 GMT
ADD file:b5b2f1fc18276a3928a2d904fedc2991239e065051f16680662a22627d15e809 in / 
# Tue, 30 Mar 2021 22:09:48 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 11:42:49 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 11:43:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 11:43:01 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 11:44:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 11:44:09 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 11:44:10 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 11:44:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 11:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 11:44:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:17fa7bb8f5ce4138c383674409fef134204b2ae72f4a997a2cebccad07e8e32b`  
		Last Modified: Tue, 30 Mar 2021 22:16:21 GMT  
		Size: 25.8 MB (25806366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a68c20179bba0326107528643f0bdfb09e5e4e12b23b94202e0a40b07b08ec`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee9cb6b3b154470e91ff1d71d60f473532f7811c34e9f9a305cb5f9b384af53`  
		Last Modified: Wed, 31 Mar 2021 11:44:37 GMT  
		Size: 1.7 MB (1712484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7e20f016e608e3dbd4989e95db2477d200c26e7139b659b5ff81af56f5849d`  
		Last Modified: Wed, 31 Mar 2021 11:44:42 GMT  
		Size: 6.4 MB (6416459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29e8d95ffa3367d7f92161d1879c4244eba457c53be1dceacf60878a6b61350`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2800304da962f86c573659de59251370b0898e93e416be1ab9a74ed6ff752d7f`  
		Last Modified: Wed, 31 Mar 2021 11:44:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:f6cbaeb1a0ee34d3e7c450623eca946126fa422ece34b7b5ccaae82d7316e545
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39516884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01d339f442f5b9596b036ecdade36fc3df4976bd2202bb5b7dfb2ba4798b890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 22:36:03 GMT
ADD file:a544303d3ec263b38c231310d807e05249140188df5c5a5c785b2f176455ac39 in / 
# Tue, 30 Mar 2021 22:36:09 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 19:40:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 19:40:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 19:40:57 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 19:45:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 19:46:02 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 19:46:08 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 19:46:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 19:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:46:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c840eb5e9aed613b2af7557a4b5ad46898b8bc475a2d470c65ec7896b11282f1`  
		Last Modified: Tue, 30 Mar 2021 22:42:39 GMT  
		Size: 30.5 MB (30545907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66d37901368857c9d4854888cc81e3596f613d4ec8257b8690775870e5e4451`  
		Last Modified: Wed, 31 Mar 2021 19:48:20 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01811f1dd1f9404c028e19635d730f014630a6dc6e55e97c9b422bc8a9dd4060`  
		Last Modified: Wed, 31 Mar 2021 19:48:23 GMT  
		Size: 2.2 MB (2225118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d162ea0ebccf2afa22e63499de4dddb27ad0af7f8b57081c5be5f3f905c0bb`  
		Last Modified: Wed, 31 Mar 2021 19:48:22 GMT  
		Size: 6.7 MB (6743642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658a4880047c37829a2e4d44e876c95bca195cf5b89f8bcdf65c6a8ee32c801b`  
		Last Modified: Wed, 31 Mar 2021 19:48:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e0ea8c770ca843bdc7acbe8af1702763603347749366a3d8c401ad29ef7d6`  
		Last Modified: Wed, 31 Mar 2021 19:48:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:97d3bd125ab186461612f5227612b8bed1b7cdf339597a848150b8abb1df9748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11acca930a3acc9f10aec0e92255da2f3d7782c440d9ebe986775b5d784b5f7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:25:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 31 Mar 2021 02:25:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:25:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 31 Mar 2021 02:25:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 31 Mar 2021 02:25:46 GMT
VOLUME [/spiped]
# Wed, 31 Mar 2021 02:25:46 GMT
WORKDIR /spiped
# Wed, 31 Mar 2021 02:25:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 31 Mar 2021 02:25:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 02:25:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c742a04892cc406ec636d3b61ae8b30ea2be9d8094b04a3e6fa844006600bb`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee293ba212f1e0d102b980847b925882c507858cf70dd83eca37c45fb14d8fb6`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 1.8 MB (1821969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048c0826dbbe30eb38c444743a578a8400ca9bb488e6dd498c2ae0c74a524ba`  
		Last Modified: Wed, 31 Mar 2021 02:26:13 GMT  
		Size: 5.9 MB (5943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8fc932e810d22ad352fd6f592c4c76a7e0fc36211bb96549e2044049a0ae6c`  
		Last Modified: Wed, 31 Mar 2021 02:26:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd24c1b830fe7b47376748fdbcf9a99c29e655cc7047927ab24e2aad8d1cf83`  
		Last Modified: Wed, 31 Mar 2021 02:26:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
