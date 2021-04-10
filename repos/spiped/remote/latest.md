## `spiped:latest`

```console
$ docker pull spiped@sha256:5a34248e112e7089adf23e9bf371f4fc409343f1ff27c34095a55589123737f0
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
$ docker pull spiped@sha256:88e595c4b27fc66524e48dc1d678f2cbba6aa124dd3c65a2f792f8317663f051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33937513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e3676406df78b6cd8501e021dc7584709e54e21d7aef150112df4116385b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:37:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 01:37:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:37:30 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 01:38:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 01:38:40 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 01:38:41 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 01:38:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:38:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e19b3a2a37a3ecbe5a0aef01b1271a3b63c4217adaa2cc9f1292b79afe4d54`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bdb8d46506c398b7a733af7dd918073564e2c1b5610e6077653e5a22d1a8bd`  
		Last Modified: Sat, 10 Apr 2021 01:39:05 GMT  
		Size: 1.7 MB (1712464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926e043611bbb0d92306441137302078e787a32420244e12aabb683e29d80455`  
		Last Modified: Sat, 10 Apr 2021 01:39:10 GMT  
		Size: 6.4 MB (6416465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b4bc1074f6d5e2ced135b61984cf1cf7f9bfd48fcd344e8e0aeb5bd85b125`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4518d534fd104cc99e25d1836fdb49c93d46fc837842791310d48c227d8bfda`  
		Last Modified: Sat, 10 Apr 2021 01:39:04 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:aa1a30de2b923e99b6d6ea55762ce4a9d15c0eef4651c9a4712e9e2ecad39e3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33521428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff980a5b5e94897b7af54b9c04e2610d83a31e1dc070fb483f806ee4396b8dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:23:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 10 Apr 2021 02:23:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:23:46 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 10 Apr 2021 02:24:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 10 Apr 2021 02:24:02 GMT
VOLUME [/spiped]
# Sat, 10 Apr 2021 02:24:02 GMT
WORKDIR /spiped
# Sat, 10 Apr 2021 02:24:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:24:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:24:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd6c712f3969791adfeec2f43170db16367eaef66a82536b0552e4b68a5f642`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b29032a4acd3ff5105640e38c4a45b05a57dcee751656350ca162fa404dd33`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 1.8 MB (1821986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd0c44243082c25de145fdf20d06ce41b41a86768dc7b3d2b3bb73c416e488b`  
		Last Modified: Sat, 10 Apr 2021 02:24:23 GMT  
		Size: 5.9 MB (5943443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179bb3d59a006f4ddc951a6cadea2d81f4262873eea7f2167d04a821ccb67acc`  
		Last Modified: Sat, 10 Apr 2021 02:24:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dea98f9a5ff0fd3b0d022a829368fcc98453f3884e762bace5d032dbe7d093`  
		Last Modified: Sat, 10 Apr 2021 02:24:23 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
